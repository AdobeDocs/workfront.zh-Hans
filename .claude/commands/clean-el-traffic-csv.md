---
name: clean-el-traffic-csv
description: 清理原始Experience League/Adobe Analytics流量CSV导出到仅限Workfront的页面，按页面查看次数排序。 当用户提供Experience League页面流量CSV（列，如“页面URL常规”、“独特访客”、“访问次数”、“页面查看次数”）并请求清理、过滤或处理它，或提及“文档跟踪”/“查看次数最多的文章”电子表格时使用。
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# 清理Experience League流量CSV

将原始Adobe Analytics自由格式表导出的Experience League页面流量转换为纯Workfront的干净CSV，并按页面查看排序，覆盖原始文件并将过期的副本保存到桌面。

## 输入形状

输入可以是以下两种形状之一：

1. **原始导出** — 以元数据注释行（`#===`、`# Freeform`、`# Report suite: ...`、`"# Date: <range>"`等）开头，后跟一个层次划分表（例如`Solution (v2)` → `workfront` → `Page URL Generic (v33)`→单个URL行）。 文本单元格`Page URL Generic (v33)`（或类似的`Page URL Generic ...`标签）在中途显示在第二列中。
2. **已经清除的CSV** — 第一行已经是纯标题，如`Page URL Generic (v33),Unique Visitors,Visits,Page Views`，没有元数据行或额外的行距。

在开始之前检测您具有的形状：如果行1是匹配形状2的纯标题行，请直接跳到步骤2（无日期范围可用，因此也跳过步骤7，除非用户单独提供日期范围）。

## 工作流

### 步骤0：捕获日期范围（仅原始导出，然后删除任何内容）

在顶部匹配`# Date: <range>`（例如`"# Date: Jul 1, 2026 - Jul 31, 2026"`）附近查找元数据行。 记录`<range>` （例如`Jul 1, 2026 - Jul 31, 2026`） — 稍后在步骤7中需要它。 在删除任何行之前执行此操作。

### 步骤1：将原始导出向下剥离到纯表（仅限原始导出）

1. 查找包含单元格`Page URL Generic (...)`的行（该单元格位于标准导出的第二列）。
2. 删除该行上方的每一行，包括元数据注释行和`Solution (v2)` / `workfront`小计行。
3. 删除`Page URL Generic`单元格左侧的每一列（在标准导出中，这只是列A）。
4. 在同一行（现在为标题行）上，将`Page URL Generic (...)`右侧的数字小计值替换为文本标题，顺序为： `Unique Visitors`、`Visits`、`Page Views`。 保留`Page URL Generic (...)`单元格本身不变。

结果：标头为`Page URL Generic (v33),Unique Visitors,Visits,Page Views`的纯CSV，每个URL后跟一行。

### 步骤2：仅保留Workfront行

对于每个数据行，检查URL是否包含文本子字符串`/workfront/`（两侧的斜杠）。 区域设置前缀不重要（`/en/`、`/zh-hans/`等 — 只要产品区段匹配，所有字段都会保留）。

- 如果URL **不**&#x200B;包含`/workfront/`作为路径段，则删除该行 — 这将删除其他产品，如`workfront-fusion`、`workfront-learn`、`proofhqpapi`等。（如`tutorials-workfront`这样的子字符串不&#x200B;**计** — 匹配项必须是准确的区段`/workfront/`）。
- 否则，请保留行。

### 步骤3：修剪URL

对于每个存活的行，在URL中找到`/using`，并仅保留其后`/`中包含（和包含）的部分，放弃之前和包含`/using`的所有内容。

示例： `https://experienceleague.adobe.com/zh-hans/docs/workfront/using/home` → `/home`

如果在Workfront行的URL中找不到`/using`，则保持该URL不变，并为用户标记该URL，而不是进行猜测。

### 步骤4：剥离片段/查询后缀

如果修剪后的URL包含`#`或`?`，请删除该字符及其后面的所有内容。

示例： `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### 步骤5：合并重复项

修剪后，多行现在可以共享相同的URL（例如，折叠到同一路径的两个不同的区域设置行）。 将具有相同URL的所有行合并为一行，分别求和`Unique Visitors`、`Visits`和`Page Views`。

示例： `/home,2,2,3`和`/home,5,6,7` → `/home,7,8,10`

### 步骤6：按页面查看排序

按`Page Views`降序对所有数据行排序（最大为先）。 标题行固定地位于顶部已排序数据的上方。

### 步骤7：添加日期范围行（仅在步骤0中捕获的情况下使用原始导出）

在插入它之前，请去除捕获的日期范围中的任何逗号（例如`Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`） — 原始范围具有逗号，否则会误读为该行上的CSV列分隔符。

在标题行的最上方插入一个新行，该行仅包含以逗号分隔的日期范围。

最终行顺序：日期范围行→标题行→已排序的数据行。

### 步骤8：保存

使用清理后的结果覆盖原输入文件。

### 步骤9：将日期副本保存到桌面（仅当在步骤0中捕获了日期范围时才需要原始导出）

生成日期范围的文件名安全版本：去除逗号，并将任何`\ / : * ? " < > |`替换为`-`（这些字符在Windows文件名中无效，否则可能会显示在日期范围中，具体取决于导出区域设置/格式）。

将已清理的CSV的附加副本（与步骤8的内容相同）保存到当前用户的桌面上，名为：

`Documentation tracking report <filename-safe date range>.csv`

示例：捕获的`Apr 1, 2026 - Apr 30, 2026`范围变为`Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`。

对于已清理的CSV（形状2），跳过此步骤，除非用户单独提供日期范围。

## 超出范围

发布或共享清理过的CSV（例如，到Slack）是一个单独的、尚未定义的步骤 — 在此技能中，请勿尝试将文件附加或上传到任何位置。

## 实施（原始导出）

对于原始导出，请使用此经过测试的PowerShell脚本运行步骤0-8，而不是手动编辑行 — 对于具有数百行的文件，它更快，不易出错。 将实际文件路径替换为`$path`。

运行之前，检查文件是否已锁定（例如在Excel中打开） — 如果`Set-Content`因“被其他进程使用”而失败，请要求用户将其关闭，然后重新运行。

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

对于已经干净的CSV（输入形状2），跳过标题重新定位、日期范围逻辑和步骤9 — 只需按原样对现有标题/行运行步骤2-6和8。
