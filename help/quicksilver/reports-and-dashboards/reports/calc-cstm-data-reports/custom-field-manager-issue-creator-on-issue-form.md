---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: “计算的自定义字段示例：在问题自定义窗体上显示问题创建者的经理”
description: 使用计算的自定义字段，您可以在附加到问题的自定义表单上显示问题创建者的管理员名称。 使用同一语句，您可以为项目、问题和其他对象构建类似的计算字段。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# 计算的自定义字段示例：在问题自定义窗体上显示问题创建者的经理

使用计算的自定义字段，您可以在附加到问题的自定义表单上显示问题创建者的管理员名称。 使用同一语句，您可以为项目、问题和其他对象构建类似的计算字段。

>[!TIP]
>
>有关其他客户的其他自定义文本模式示例的信息，请按照 [文本模式报告](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) 主题。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront计划*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限<br>有关从访问级别授予管理访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>对象权限</p> </td> 
   <td> <p>对附加了表单的对象的访问权限，并拥有对编辑自定义表单的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在问题自定义窗体上显示问题创建者的经理

以下步骤显示如何为问题自定义表单创建计算字段，您可以在其中捕获创建问题的用户经理的名称。 例如，当您想要捕获创建任务、项目、项目组合的用户经理的姓名时，该过程是相同的。

1. 创建问题自定义表单并向其添加计算字段。

   有关创建自定义表单并向其添加计算字段的信息，请参阅以下文章：

   * [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 将以下文本模式代码复制并粘贴到 **计算** 自定义表单的字段：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自定义字段计算区分大小写。

1. 单击 **完成**，则 **保存并关闭**.

   创建问题的用户经理在包含字段的表单附加到问题时显示在计算字段中。
