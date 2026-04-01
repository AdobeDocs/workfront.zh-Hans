---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Git提交消息

始终应用此规则。 在草稿或生成Git提交消息时（例如，在Source Control提交框中或在Agent聊天中询问时），请遵循此格式。

## 主题行（仅限第一行）

- 大约&#x200B;**50个字符或更少**。
- 总结&#x200B;**提示语气**&#x200B;中的更改（例如“添加……”、“修复……”、“重构……”）。

## 空白行

在主文前面的主题后面留一行&#x200B;**空白**。

## 正文（详细说明）

- 行以大约&#x200B;**72个字符**&#x200B;换行（包括项目符号前缀和空格）。
- 请使用&#x200B;**项目符号行**&#x200B;来解释。 每个项目符号必须刚好以以下项之一开头：
   - **📖** — 在更改&#x200B;**添加**&#x200B;新内容时使用：新文件、新分区、新功能、新标头、新行或其他新字段内容。
   - **✏️** — 在更改&#x200B;**修改**&#x200B;现有工作时使用：编辑现有行、更新现有节、重构现有代码或更改当前内容。

将&#x200B;**📖**&#x200B;或&#x200B;**✏️**&#x200B;应用于每个正文项目符号，以便清楚显示引入的内容与更改的内容。

## 模板

填写占位符（请勿在最终消息中保留尖括号）：

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## 示例

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
