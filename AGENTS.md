---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

**workfront.en**存储库的代理指南（Adobe Workfront英语）
文档)。 此文件指向规范说明，因此任何代理 — 
无论读取哪个公约文件，都遵循相同的规则。

## 规范指令文件

- **存储库范围的规则**： [.github/copilot-instructions.md](.github/copilot-instructions.md)
 — 候选文章搜索、编辑前建议、提交消息和PR格式，
以及“聪明地填补空白”。
- **正在编写标准** （自动应用于`help/**/*.md`）：
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md)，
全部详细信息，请参见
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md)。
- **发行说明** （自动应用于`product-announcements/product-releases/**`）：
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md)。
- **预览高亮清理** （按需工作流）：
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md)。

## 不可协商的行为

1. **创建新候选文章之前先查找候选文章。** 当新内容到来时
在中，搜索`help/`并显示它可能适合的现有文章的排名列表，
然后在起草之前问它属于何处。
2. **在编辑任何帮助`.md`文章之前提出更改。** 显示提议的
比较并等待明确批准。 唯一的例外是当我说“只要修复”
它”或“不要询问，只需编辑”的按钮。 只读研究和聊天
起草总是可以的。
3. **智能地填补空白。** 当意图明确时，承诺
最佳实践回答并匹配相关文章标题，
术语和结构，而不是演示选项菜单。
4. **在每`help/`次编辑时主动应用编写标准** — 不要等待
以提醒您。

## 提交和PR约定

有关完整信息，请参阅[.github/copilot-instructions.md](.github/copilot-instructions.md)
commit-message格式(必要主题≤约50个字符；📖用于添加，✏️用于
修改)和PR结构(分支名称中的Jira ID；`# Summary`，
`# Changes`按文件，`# Context` → `## Jira`)。
