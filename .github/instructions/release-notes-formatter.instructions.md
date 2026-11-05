---
description: Adobe Workfront发行说明（概述、产品区域、规划和外观页面）的格式化和验证规则。
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# 发行说明格式化程序

这些文件是&#x200B;**发行说明**，而不是操作方法文章。 请&#x200B;**不**&#x200B;应用
此处为常规编写质量标准。 在编辑之前，请阅读的完整源
truth，其中包含模板和发布日历：

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## 关键规则 — 首先确定文档季度

&#x200B;> [!IMPORTANT]
> 切勿在其上使用calendar-quarter math为文档季度指定功能
> 预览或生产日期。 Doc-quarter基于哪个&#x200B;**月发布**
> 根据Workfront的内部发布 — 日历分组，该功能位于
> 从日历季度偏移。 例如，具有生产环境的功能
> 2026年8月13日的日期属于doc-quarter `26-q4`，而不是`26-q3`。 总是
> 之前请仔细查看参考文件中的2026版日历表
> 创建或编辑任何文件。 如果生产日期不在该表内，
> 要求更新日历，而不是猜测。

## 关键结构规则

- **Frontmatter**： `feature`必须正好是`Product Announcements`；
  `recommendations`必须刚好`noDisplay, noCatalog`。 从不发明
  `exl-id` — 仅当它已存在时才包含它。
- **最新功能优先**：最新的发行说明是之后的第一个H2
介绍（产品区域页面）和每个功能表的顶行（概述）
页面)。
- **概述链接**：产品区域页面必须链接到&#x200B;**他们自己的季度**
概述文件 — 一个常见错误是链接到上一季度。
- **日期标注**：每个功能H2后面都有一个`>[!NOTE]`块，其中
预览/生产快速发布/针对每个人的生产日期，与
概述表格行。 将日期格式设置为`Month Day, Year`；如果未知，请使用`TBD`。
- 用H1s写&#x200B;**季度名称**：“第一季度”、“第二季度”、“第三季度”
“第四季度”。

## 添加页面时所需的伴随更新

- **新页面（任何）**：在同一更改中将其添加到`help/quicksilver/TOC.md`
（首先概述，按字母顺序显示产品区域页面，最后显示其他增强功能）。
- **新季度的概述页面**：同时更新`help/quicksilver/home.md` —
刷新“最新版本”选项卡链接和规划活动链接，然后添加
“当年版本”选项卡的新季度。

有关完整模板，请参阅上面的SKILL.md和reference.md文件，
文件命名约定、链接格式和完整发行日历。
