---
title: 使用AI自动填写请求
content-type: reference
description: 您可以使用AI自动填写请求字段。
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 使用AI自动填写请求

AI可帮助您自动填写请求字段。 它可以根据以前的请求建议字段值，或从文本（如电子邮件）中解析这些值。

您可以在提交请求之前批准或拒绝这些提交。

自动填写不会覆盖您已填写的任何字段。

## 在填写表单时获取建议

自动填写可以在您填写表单时建议字段值。 在请求字段中输入值时，Workfront会将这些值与以前的请求进行比较。 如果输入的值与以前请求中类似上下文中的其他字段值紧密相关，则Workfront会推荐这些值。

例如，如果诊所始终使用相同的计费代码，那么在输入诊所名称时，Workfront会建议在适当的字段中输入该计费代码。

要根据以前的请求使用建议，请执行以下操作：

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 开始填写字段。

   当您填写字段时，其他字段可能会显示建议。

1. 对于每个字段建议，请选择该字段下的&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

## 从文本提示获取建议

自动填写可根据文本（如电子邮件）建议字段值。 将粘贴到文本块中，Workfront会处理文本以根据文本建议字段值。

例如，如果电子邮件包含“此日期在6月1日到期”，并且请求表单中存在到期日期的字段，则Workfront将建议在6月1日使用该字段值。

此类建议还会检查以前对类似上下文的请求。 例如，如果提示提及请求是针对特定客户的，Workfront可以根据之前的请求自动查找并输入该客户的账单地址。

您可以粘贴要应用于整个表单或表单单个部分的文本。

要根据粘贴的文本提示使用建议，请执行以下操作：

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 要将文本提示应用于整个表单，请单击屏幕右上角的&#x200B;**使用AI自动填充**。

   或

   要为单个分区应用文本提示，请单击分区名称旁边的AI图标![AI图标](assets/request-prompt-icon.png)。

1. 将文本粘贴到提示框中。
1. 单击&#x200B;**填写表单**。

   Workfront会生成表单建议。
1. 对于每个字段建议，请选择该字段下的&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

