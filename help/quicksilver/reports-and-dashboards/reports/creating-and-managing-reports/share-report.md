---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在Adobe Workfront中共享报表
description: 您的Adobe Workfront管理员在用户分配访问级别时，会授予用户查看或编辑报表的权限。 有关授予对问题的访问权限的更多信息，请参阅授予对报表、功能板和日历的访问权限。
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# 在Adobe Workfront中共享报表

您的Adobe Workfront管理员在用户分配访问级别时，会授予用户查看或编辑报表的权限。 有关授予对问题的访问权限的更多信息，请参阅 [授予对报表、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定报表的权限。 有关访问级别和权限的更多信息，请参阅 [访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

权限特定于Workfront中的一个项目，并定义可以对该项目执行哪些操作。

>[!NOTE]
>
>Workfront管理员可以添加或删除系统中所有用户的任何项目的权限，而不是这些项目的所有者。

## 访问要求

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对报表、功能板、日历的访问权限或更高权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表的权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关共享报表的注意事项

除了以下注意事项外，另请参阅 [共享报表、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* 您可以与其他个人、团队、组、工作角色或公司共享您创建的报表。 您还可以共享其他人创建并与您共享的报表。
* 您还可以与整个组织共享这些组件，或将它们公开。 将报表设为公用会生成一个可与他人共享的URL。
* 您可以共享单个报表，也可以从报表列表共享多个报表。

## 共享报表的方法

您可以通过以下方式在Workfront中共享报表：

* 手动，如 [共享报表](#share-a-report) 部分。
* 通过从包含已共享报表的功能板继承查看权限，自动执行此操作。 有关查看对象继承权限的信息，请参阅 [查看对象的继承权限](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## 共享报表 {#share-a-report}

从列表中共享一个或多个报表是相同的。

1. 转到报表列表，选择一个或多个报表，然后单击 **共享**.

   或

   单击一个报表的名称，然后单击**报表操作>****共享**.

   ![](assets/qs-report-actions-sharing.png)

1. 在显示的框中，在 **添加人员、团队、角色、组或公司……** 字段开始键入要与其共享报表的用户、团队、职务角色、组或公司的名称，然后按 **输入** 显示名称时。

1. 要调整所添加名称的访问级别，请单击该名称右侧的下拉菜单，然后选择下面的选项之一。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看它</td> 
      <td> <p>允许收件人在 <strong>报表</strong> <img src="assets/reports-in-main-menu.png"> 并运行。</p> <p>您可以单击 <strong>高级设置</strong> 指定您希望用户还是用户能够 <strong>共享</strong> 和系统里的任何人。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>允许收件人完全编辑对报表的访问权限。</p> <p>您可以单击 <strong>高级设置</strong> 指定您希望用户还是用户能够 <strong>删除</strong> 系统和 <strong>共享</strong> 和系统里的任何人。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复前面的2个步骤，将其他名称添加到列表并配置其选项。
1. （可选）单击 **齿轮** 图标 ![](assets/gear-icon-settings-with-dn-arrow.jpg) 在共享框的右上角，选择以下选项之一：

   * **将此变量公开给外部用户：** 选择此选项可生成可与他人共享的URL。 任何具有URL的人都可以访问报表，而无需获得Adobe Workfront许可证。

      >[!CAUTION]
      >
      >我们建议您在与外部用户共享包含机密信息的对象时务必谨慎。 这样，用户便无需成为Workfront用户或您组织的一员，即可查看信息。

      >[!NOTE]
      >
      >如果报表有提示，并且您公开共享它，则运行报表的用户必须登录Workfront才能使用提示运行报表。 如果他们无法登录Workfront，则将在未应用提示的情况下看到报表。 有关与提示共享报表的限制的更多信息，请参阅部分 [共享提示报表的限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) 在文章中 [向报表添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **在系统范围内使此可见：** 选择此选项，以便Workfront中有权访问报表的每个人都可以查看报表。

1. 单击&#x200B;**保存**。
