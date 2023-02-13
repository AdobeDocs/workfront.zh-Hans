---
title: 授予对文档的访问权限
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别定义用户对Workfront中文档的访问权限。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 授予对文档的访问权限

作为Adobe Workfront管理员，您可以使用访问级别定义用户对文档的访问权限，如 [访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

此访问也适用于文档文件夹。

有关使用自定义访问级别管理用户对Workfront中其他对象类型的访问权限的信息，请参阅 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。&gt; 。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用自定义访问级别配置用户对文档的访问权限

1. 开始创建或编辑访问级别，如 [创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. 单击齿轮图标 ![](assets/gear-icon-settings.png) 在 **查看** 或 **编辑** 按钮，然后选择要在 **优化设置**.

   ![document_access.png](assets/document-access.png)

   您可以允许用户对他们有权访问的项目、任务和问题执行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">创建</td> 
      <td>上传文档。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">删除</td> 
      <td> <p>删除上传的文档。</p> <p>的 <b>创建</b> 选项在启用此选项时自动启用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">共享</td> 
      <td>与特定用户、工作角色、团队共享文档。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">公开共享文档</td> 
      <td>与外部用户共享文档(没有Workfront许可证)。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在系统范围内共享</td> 
      <td> <p>使文档可供Workfront实例中的每个人使用。</p> <p>如果出现以下情况，系统中的任何人都可以看到以这种方式共享的文档：</p> 
       <ul> 
        <li> <p>您会向他们发送一个链接，指向上传文档的页面。</p> </li> 
        <li> <p>他们在Workfront搜索</p> </li> 
       </ul> <p>的 <b>共享</b> 选项在启用此选项时自动启用。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >在为特定类型的对象配置访问级别设置时，该配置不会影响用户对级别较低的对象的访问。 例如，您可以限制用户删除其访问级别中的项目，但这并不限制用户删除排名低于项目的文档。有关对象层次结构的详细信息，请参阅部分 [对象的相互依赖和层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. （可选）要限制来自较高排名对象的文档的继承权限，请单击 **设置其他限制**，然后选择 **从不从项目、任务、问题等继承文档访问权限**.
1. （可选）要在您正在处理的访问级别中为其他对象和区域配置访问设置，请继续阅读 [配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)，例如 [授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 和 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. 完成后，单击 **保存**.

   创建访问级别后，您可以将其分配给用户。 有关更多信息，请参阅 [编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 按许可证类型访问文档

有关每个访问级别中的用户可以对文档执行的操作的更多信息，请参阅部分 [文档](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) 在文章中 [可用于每种对象类型的功能](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## 访问共享文档

将文档上传到Workfront后，您可以通过向其他用户授予文档权限来与他们共享该文档，如 [共享文档](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

当您与其他用户共享任何对象时，收件人对该对象的权限取决于两件事的组合：

* 您为收件人授予的对象权限
* 对象类型的收件人访问级别设置
