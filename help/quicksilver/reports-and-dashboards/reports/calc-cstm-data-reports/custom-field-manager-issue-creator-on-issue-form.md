---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 计算自定义字段示例：在问题自定义表单上显示问题创建者的经理
description: 使用计算自定义字段，您可以在附加到问题的自定义表单上显示问题创建者的经理姓名。 使用相同的语句，您可以为项目、问题和其他对象构建类似的计算字段。
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: a1ead6d0c1c85bfbe6d7302506743db8d8b3e205
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# 计算自定义字段示例：在问题自定义表单上显示问题创建者的经理

使用计算自定义字段，您可以在附加到问题的自定义表单上显示问题创建者的经理姓名。 使用相同的语句，您可以为项目、问题和其他对象构建类似的计算字段。

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront包</p> </td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证</p> </td> 
   <td>
      <p>标准</p>
      <p>规划</p></td>
  </tr> 
  <tr> 
   <td><p>访问级别配置</p></td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr> 
  <tr> 
   <td> <p>对象权限</p> </td> 
   <td> <p>分配对表单所附加对象的访问权限，并具有编辑自定义表单的访问权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在问题自定义表单上显示问题创建者的经理

以下步骤显示如何为问题自定义表单创建计算字段，您可以在其中捕获创建问题的用户经理的姓名。 当您要捕获创建任务（例如，项目、项目组合）的用户的经理姓名时，该过程是相同的。

1. 创建问题自定义表单并向其中添加计算字段。

   有关创建自定义表单并向其中添加计算字段的信息，请参阅以下文章：

   * [创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. 将以下文本模式代码复制并粘贴到自定义表单的&#x200B;**计算**&#x200B;字段中：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自定义字段计算区分大小写。

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存+关闭**。

   将包含计算字段的表单附加到问题时，创建问题的用户的经理将显示在该字段中。
