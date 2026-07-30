---
name: release-notes-formatter
description: 格式化并验证Workfront发行说明，确保一致性、正确结构和正确链接。 仅用于产品版本目录中的发行说明文件，或者用户提及发行说明、产品版本或季度版本时。 不适用于操作方法文章或常规文档。
source-git-commit: fa39320af72acf6d2ceaf201480baf78a07ae76e
workflow-type: tm+mt
source-wordcount: '1692'
ht-degree: 3%

---


# 发行说明格式化程序

在`help/quicksilver/product-announcements/product-releases/`目录中格式化并验证Adobe Workfront发行说明。

## 页面类型

从文件路径和内容中标识页面类型：

| 页面类型 | 文件模式 | 模板 |
|-----------|-------------|----------|
| **概述** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **产品区域** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **计划** | `planning-release-activity-{YY}-q{N}.md` | 类似于产品区域 |
| **外观** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#look-and-feel](reference.md#look-and-feel-page-template) |

## 步骤0：确定季度（比其他任何操作先进行此操作）

>[!IMPORTANT]
>
>切勿在文档季度的“预览”或“生产”日期使用日历季度数学为其指定功能。 Doc-quarter是根据Workfront的内部版本 — 日历分组（与日历季度偏移），该功能的&#x200B;**每月版本**&#x200B;提供的功能 — 请参见此文件末尾附近的[2026版日历](#2026-release-calendar)表。 例如，生产日期为2026年8月13日的功能属于doc-quarter `26-q4`，而不是`26-q3`，因为8月月度发行版本映射到`26-q4`。
>
>进一步向下的“季度映射”（写入形式/月）表用于在标题中写出季度名称（例如，第3季度的“第三季度”） — 它自己&#x200B;**不足**&#x200B;来确定某个功能属于哪个季度的文件。 在创建或编辑任何文件之前，请始终对发布日历表进行交叉检查。
>
>如果某个功能的生产日期未显示在“发布日历”表中（例如，该日期超出该表的日期范围），请询问用户更新的日历，而不是猜测。

## 格式化工作流

### 步骤1：验证Frontmatter

所有发行说明页面的必填字段：

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

规则：
- `feature`必须刚好`Product Announcements`
- `recommendations`必须刚好`noDisplay, noCatalog`
- 从不创建`exl-id` — 仅包含已存在的一个
- 不要将`draft: Probably`添加到实际页面（仅限模板）

### 步骤2：按页面类型验证结构

#### 产品区域页面

1. **H1**： `{Written Quarter} {Area} enhancements`
   - 示例：`# Second Quarter 2026 Administrator enhancements`
   - 季度必须写成：“第一季度”、“第二季度”、“第三季度”、“第四季度”

2. **简介段落**：说明区域以及概览的链接
   - 必须链接到&#x200B;**正确季度的**&#x200B;概览文件
   - 常见错误：链接到上一季度（例如，`26-q1`而不是`26-q2`）

3. 每个功能&#x200B;**H2**：将功能标题作为标题
   - **最新功能在前** — 最新的发行说明必须作为介绍段落之后的第一个H2显示
   - 较旧的功能将按反时间顺序列出

4. 在每个H2之后&#x200B;**日期标注块**：

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **正文**：功能描述，然后链接到帮助文档

#### 概述页面

1. **H1**： `{Written Quarter} release overview`

2. **在计划发行月份介绍段落**

3. 带有发布计划表的&#x200B;**`>[!IMPORTANT]`块**

4. **H2`Adobe Workfront enhancements`**，包含锚点链接的项目符号列表：

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. 带有HTML功能表的&#x200B;**H3每个产品区域**（请参阅[reference.md](reference.md#overview-feature-table)）
   - 在每个表中，**最新功能排在前** — 最新行显示在表的顶部（标题行之后）

&#x200B;6. **尾随部分** (H2)：其他区域的发行说明、桌面校对查看器更新、公告、API版本、维护更新、培训更新

### 步骤3：验证链接

- 产品区域页面中的&#x200B;**概述链接**：必须指向同一季度
  - 正确： `26-q2-release-activity/26-q2-release-overview.md`
  - 错误： `26-q1-release-activity/26-q1-release-overview.md`
- 概览中的&#x200B;**锚点链接**：必须匹配H3 ID（小写、连字符）
- 概览表中的&#x200B;**功能链接**：必须使用`class="MCXref xref" xrefformat="{para}"`
- **帮助文档链接**：必须以`/help/quicksilver/`开头

### 步骤4：验证日期

- 格式： `{Month} {Day}, {Year}`（例如，“2026年3月12日”）
- 将`TBD`用于未知日期
- 产品区域页面`>[!NOTE]`块中的日期必须与相应的概述表行匹配
- 预览日期应早于生产日期

### 步骤5：常见修复

设置格式时应用以下修复：

| 问题 | 修复 |
|-------|-----|
| 概述链接季度错误 | 更新以匹配文件自己的季度 |
| 缺少`>[!NOTE]`日期块 | 在H2功能标题后添加块 |
| 日期格式不一致 | 标准化为`Month Day, Year` |
| `>[!NOTE]`前缺少空白行 | 添加空白行 |
| 编号说明行中的额外空格 | 修剪尾随空格 |
| 产品区域页面中的HTML | 保留为Markdown（HTML仅适用于概览表） |
| 缺少`exl-id` | 将其排除 — 不生成一个 |

### 步骤6：更新目录

每当您创建&#x200B;**新**&#x200B;发行说明页面（概述或产品区域）时，请将其添加到同一更改中的`help/quicksilver/TOC.md`。 不在目录中的页面将不会显示在已发布的导航中，即使概述表格中的链接指向该页面也是如此。

添加的位置：

- 目录在标题下每季度有一个节，如`* 2026 Q3 Release {#release-26-q3}`。 如果季度标题尚不存在（新季度的第一页），请将其添加到上一季度的上方，这样最新季度就会位于最上方。
- 在该季度标题下，按以下顺序列出页面：
  1. 首先&#x200B;**概述** (`Third Quarter 2026 release overview`)。
  2. **产品区域页面**&#x200B;按区域名称（管理员、文档、企业运营、项目、报表、请求）的字母顺序排列。
  3. **其他增强功能**&#x200B;最后进行（始终在按字母顺序排列的产品区域之后）。

每个TOC条目都是一个使用页面标题和绝对存储库路径的Markdown链接：

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

将缩进（六个空格）与周围的条目匹配。 将页面H1逐字用作链接文本 — 例如`Documents enhancements`、`Requesting enhancements`（不是`Requests`） — 以便TOC标签与之前的季度匹配。

要避免的常见错误：

- 创建产品区域页面，而不将其添加到目录。
- 从新的产品区域页面链接到其他季度的概述（步骤3）。
- 在上一个季度的标题下插入新季度的页面。

### 步骤7：更新主页

每当您创建&#x200B;**新季度的概述页面**（即，这是新季度的第一页，而不仅仅是添加到现有季度的新产品区域页面）时，请在同一更改中更新`help/quicksilver/home.md`：

- 在`>[!TAB Latest release]`部分中，将版本概述链接替换为新季度的概述链接。
- 也在该部分中，更新Adobe Workfront Planning发布活动链接以指向新季度的计划文件(`planning-release-activity-{YY}-q{N}.md`)（如果存在）。
- 在当前年度的`>[!TAB {YYYY} releases]`选项卡中，将新季度的概述链接添加到列表顶部，并位于上一季度的条目上方。

仅将产品区域页面添加到已列出概述页面的季度时，请勿触及`home.md`。

要避免的常见错误：

- 创建新季度的概述页面而不更新`home.md`的“最新版本”选项卡（它将继续指向旧季度）。
- 忘记还要将新季度添加到当年选项卡列表。

## 文件命名约定

| 类型 | 模式 | 示例 |
|------|---------|---------|
| 概述 | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| 产品区域 | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| 目录 | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

标准区域概要： `admin-and-setup`、`documents`、`projects`、`reports`、`requests`、`other`

## 季度映射

>[!NOTE]
>
>此表用于写出季度名称（例如，H1或标题中）。 它无法确定某个功能所属的季度文件 — 请针对该问题使用下面的[2026版日历](#2026-release-calendar)表，因为doc-quarter与calendar-quarter发生偏移。

| 季度 | 书面形式 | Months |
|---------|-------------|--------|
| Q1 | 第一季度 | 1月3日 |
| Q2 | 第二季度 | 4月6日 |
| Q3 | 第三季度 | 7月9日 |
| Q4 | 第四季度 | 10月至12月 |

**重要 — 在文件名（`26-q3`、`26-q4`等）中使用的文档季度 距此日历映射偏移一个月。** 它遵循Workfront的内部发布日历分组，其中每个文档季度=前两个月度发布+季度发布月份。 例如，文档季度`26-q3`涵盖2026年5月/6月/7月月度版本（季度版本`2026.07`），文档季度`26-q4`涵盖2026年8月/9月/10月月度版本（季度版本`2026.10`）。 在根据上面的日历季度表假定文件的季度之前，请务必查看下面的发布日历（或请求更新日历）。

## 2026版日程表

Source： “2026年每月发布日历”（Adobe corp wiki，AWF空间 — `wiki.corp.adobe.com`，空间密钥AWF，标题“2026年每月发布日历”）。 WebFetch无法访问此页面（需要Adobe SSO）；当需要的日期超出了此处捕获的日期时，需要请求用户粘贴更新的PDF/表。

| 发行月份 | 最终预览 | 生产 | 每月发布 | 季度发布 | 文档季度 |
|---|---|---|---|---|---|
| 2025年11 | 2025年10月30日 | 2025年11月13日 | 2025.11 | 2026.01 | 26-q1 |
| 2025年12月 | 2025年11月27日 | 2025年12月11日 | 2025.12 | 2026.01 | 26-q1 |
| 2026年1月 | 2025年12月23日 | 2026年1月15日 | 2026.01 | 2026.01 | 26-q1 |
| 2026年2月 | 2026年1月29日 | 2026年2月12日 | 2026.02 | 2026.04 | 26-q2 |
| 2026年3月 | 2026年2月26日 | 2026年3月12日 | 2026.03 | 2026.04 | 26-q2 |
| 2026年4月 | 2026年4月2日 | 2026年4月16日 | 2026.04 | 2026.04 | 26-q2 |
| 2026年5月 | 2026年4月30日 | 2026年5月14日 | 2026.05 | 2026.07 | 26-q3 |
| 2026年6月 | 2026年5月28日 | 2026年6月11日 | 2026.06 | 2026.07 | 26-q3 |
| 2026年7月 | 2026年7月7日 | 2026年7月16日 | 2026.07 | 2026.07 | 26-q3 |
| 2026年8月 | 2026年7月30日 | 2026年8月13日 | 2026.08 | 2026.10 | 26-q4 |
| 2026年9月 | 2026年9月3日 | 2026年9月17日 | 2026.09 | 2026.10 | 26-q4 |
| 2026年10 | 2026年10月1日 | 2026年10月15日 | 2026.10 | 2026.10 | 26-q4 |
| 2026年11 | 2026年10月29日 | 2026年11月12日 | 2026.11 | 2027.01 | 27-q1 |
| 2026年12月 | 2026年11月26日 | 2026年12月10日 | 2026.12 | 2027.01 | 27-q1 |
| 2027年1月 | 2027年1月5日 | 2027年1月14日 | 2027.01 | 2027.01 | 27-q1 |

有关使用此表的说明：

- **最终预览**&#x200B;是该月版本的预览中功能可能显示的最后日期 — 将它用于概述页面的“功能可能显示在预览环境中的最后日期”项目符号（仅限季末月份）。
- **Production**&#x200B;是该月发布的正式每个人都要参加的日期。
- 对于季度结束月份（与“季度版本”列匹配的月份），概述页面的计划表列出该月份的版本&#x200B;**两次**：一次在“每月版本”列列出&#x200B;**生产日期（快速版本发布日期）前一天，另一次在“季度版本”列列出**&#x200B;实际生产日期。 一个季度的非最终月份在每月列表和任何“快速发布”参考中使用相同的生产日期，无需调整。
- 此表仅列出到2027年1月。 当需要较晚的日期时，请要求用户提供更新的日程表，而不是猜测。

季度产量报告通常会在当季最后一个月的第二个整周的周四发布。

## 验证核对清单

查看发行说明文件时，请验证：

- [ ] Frontmatter的所有必填字段都具有正确的值
- [ ] H1与页面类型格式匹配
- [ ]概述链接指向正确的季度
- [ ]每个功能都有一个`>[!NOTE]`日期块（产品区域页面）
- [ ]日期格式一致(`Month Day, Year`)
- [ 概述中的]功能表行与产品区域页面内容匹配
- [ ]没有断开的内部链接
- [ 概述中的]个锚点链接与H3节ID匹配
- [ ]功能以最新先的方式排序（包括产品区域页面和概述表）
- [ ]个新发行说明页面在`help/quicksilver/TOC.md`中按正确的季度列出，概览在前，产品区域按字母顺序（其他在后）排列
- [ ]如果创建了新季度的概述页面，则`help/quicksilver/home.md`“最新版本”选项卡和当前年份选项卡指向该页面

## 其他资源

- 有关完整的HTML模板和示例，请参阅[reference.md](reference.md)
