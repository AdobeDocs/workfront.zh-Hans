---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# 拉取请求(PR)

在草稿或查看拉取请求标题或描述时（例如，在GitHub/GitLab中或在代理聊天中询问时），请遵循以下约定。

## 得出Jira问题

- **Source的真实情况：**&#x200B;从&#x200B;**当前Git分支名称**&#x200B;派生Jira问题ID（例如，与项目键模式匹配的区段，如`FFENT-8796`）。
- **如果分支名称包含Jira ID：**，请在PR标题中使用该ID（见下文），并将其链接到`# Context`→`## Jira`。
- **如果分支名称不包含Jira ID：**&#x200B;请将PR视为与票证无关。 **从PR标题中省略** Jira密钥（不创建票证）。 仍包括`# Context`→`## Jira`，其内容完全为： `No ticket`（无链接）。

## PR标题

**当分支名称包含Jira问题ID**&#x200B;时，同时包含&#x200B;**两者**：

1. **Jira问题ID**（例如`FFENT-8001`）。
2. 使用此模式的&#x200B;**提交类型**（请参阅下面的列表）：

`{type}/{JIRA-ID}- {short task description}`

示例：

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

在ID之后使用简洁的命令式描述。 匹配显示的间距模式：键入、斜杠、带尾随连字符的Jira键、空格，然后是说明。

**当分支名称不包含Jira问题ID**&#x200B;时，从标题中忽略该票证并使用：

`{type}- {short task description}`

示例：

`docs- Refresh Object Composite API changelog`

### 可接受的承诺类型（在`/`之前完全使用这些标签）

- **特征** — 添加了一个新功能。 添加新的TOC项或JIRA连接到另一个标记为Jira的`feat`时。
- **修复** — 修复错误
- **重构** — 重写/重构代码而不更改行为
- **性能** — 改进性能（特殊重构）
- **style** — 仅格式化/空白；无变化。 仅编辑
- **测试** — 添加或更正测试
- **文档** — 添加了新内容。 仅文档
- **生成** — 生成工具、CI、依赖关系、项目版本等。
- **操作** — 基础架构、部署、备份、恢复等。
- **杂项** — 其他（如`.gitignore`）

## PR正文 — 必需部分

完全使用&#x200B;**这些顶级部分** （Markdown标题）：

### 1. `# Summary`

简要概述&#x200B;**更改了哪些内容**&#x200B;以及&#x200B;**为什么更改**（业务或技术意图）。

### 2. `# Changes`

按&#x200B;**文件**&#x200B;组织。 对于每个接触的文件，使用带有回勾式路径的2级标题，然后使用项目符号描述编辑。

格式：

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

始终在&#x200B;**下包含** Jira`# Context`子节。

**当分支名称包含Jira ID时：**&#x200B;使用问题的可单击链接（从分支名称派生键）。

格式：

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

将密钥和URL替换为实际票证。 如果应用了多个票证，请在同一子部分中单独列出每个票证。

**当分支名称不包含Jira ID时：**&#x200B;保留`## Jira`并完全使用：

```markdown
# Context

## Jira
No ticket
```

## 示例（完整PR描述）

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## 示例（完整的PR描述，没有Jira ID的分支）

**标题：** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
