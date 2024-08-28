---
title: 使用AI助手修订计算字段公式
content-type: reference
description: 您可以使用AI Assistant解决计算字段中的无效自定义表达式中的错误。
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: d261fd9eb9b8b649ebe413e35161543db1db8412
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# 使用AI助手生成或修订计算字段公式

您可以使用AI Assistant根据提供的提示生成公式。 您还可以解决计算字段中的无效自定义表达式中的错误。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td><p>新增：Prime或Ultimate</p>
       <p>或</p>
       <p>当前：不可用</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：不可用</p></td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 生成计算字段表达式

## 修订计算字段表达式

在自定义表单生成器中创建计算字段时，如果公式无效，则该字段下会显示错误消息。

![无效表达式错误](assets/invalid-expression.png)

AI助手可以帮助您将公式修订为有效的计算字段表达式。

要修订无效的计算字段表达式，请执行以下操作：

1. 单击屏幕右上角附近的&#x200B;**AI助手**&#x200B;图标![AI助手图标](assets/ai-assistant-icon.png)。
1. 在“AI助手”面板底部附近的提示区域中，输入以下提示：
   `Rewrite this formula to remove the invalid expression error`
1. 从自定义表单生成器中复制无效的表达式，并将其粘贴到提示区域。
1. 按&#x200B;**Enter**。

   AI Assistant可能需要一些时间来生成修订公式，具体取决于公式的大小或复杂程度。
1. 在AI助手面板中查看修订的公式。
1. （可选）从“AI助手”面板复制修订的公式，并将其粘贴到自定义表单生成器的计算字段中。

>[!NOTE]
>
>我们建议测试计算字段以确保其检索到预期结果。

有关Workfront中计算字段的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。
