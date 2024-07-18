---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: “计算自定义字段示例：在问题自定义表单上显示问题创建者的经理”
description: 使用计算自定义字段，您可以在附加到问题的自定义表单上显示问题创建者的经理姓名。 使用相同的语句，您可以为项目、问题和其他对象构建类似的计算字段。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
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

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限<br>有关从访问级别授予管理访问权限的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>。</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限</p> </td> 
   <td> <p>Contribute对表单附加到的对象的访问权限，以及对编辑自定义表单的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 在问题自定义表单上显示问题创建者的经理

以下步骤显示如何为问题自定义表单创建计算字段，您可以在其中捕获创建问题的用户经理的姓名。 当您要捕获创建任务（例如，项目、项目组合）的用户的经理姓名时，该过程是相同的。

1. 创建问题自定义表单并向其中添加计算字段。

   有关创建自定义表单并向其中添加计算字段的信息，请参阅以下文章：

   * [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 将以下文本模式代码复制并粘贴到自定义表单的&#x200B;**计算**&#x200B;字段中：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自定义字段计算区分大小写。

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存+关闭**。

   将包含计算字段的表单附加到问题时，创建问题的用户的经理将显示在该字段中。
