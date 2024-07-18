---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 在Adobe Workfront中共享报表
description: 在分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑报告的访问权限。 有关授予对问题的访问权限的更多信息，请参阅授予对报告、功能板和日历的访问权限。
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# 在Adobe Workfront中共享报表

在分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑报告的访问权限。 有关授予对问题的访问权限的详细信息，请参阅[授予对报告、功能板和日历的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)。

除了授予用户的访问级别之外，您还可以授予他们查看或管理您有权共享的特定报告的权限。 有关访问级别和权限的详细信息，请参阅[访问级别和权限如何协同工作](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

权限特定于Workfront中的一个项目，并定义您可以对该项目执行的操作。

>[!NOTE]
>
>Workfront管理员可以为系统中的任何项目为所有用户添加或删除权限，而无需成为这些项目的所有者。

## 访问要求

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对报告、功能板和日历的访问权</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看报表或更高权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 有关共享报表的注意事项

除了下面的注意事项外，另请参阅[共享报告、功能板和日历](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。

* 您可以与其他个人、团队、组、职位角色或公司共享您创建的报告。 您还可以共享他人创建并与您共享的报告。
* 您还可以将其与整个组织共享或公开。 将报表设为公共会生成一个可与他人共享的URL。
* 您可以共享单个报告，也可以从报告列表中共享多个报告。

## 共享报表的方法

您可以通过以下方式在Workfront中共享报表：

* 手动，如以下[共享报表](#share-a-report)部分中所述。
* 通过从包含已共享报表的功能板继承查看权限，自动进行。 有关查看对象的继承权限的信息，请参阅[查看对象的继承权限](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。

## 共享报告 {#share-a-report}

从列表中共享一个报告或多个报告是相同的。

1. 转到报告列表并选择一个或多个报告，然后单击&#x200B;**共享**。

   或

   单击一个报表的名称，然后单击**报表操作>****共享**。

   ![](assets/qs-report-actions-sharing.png)

1. 在显示的框中，在&#x200B;**添加人员、团队、角色、组或公司……**&#x200B;字段中，开始键入要与其共享报告的用户、团队、工作角色、组或公司的名称，然后在名称显示时按&#x200B;**Enter**。

1. 要调整所添加名称的访问级别，请单击名称右侧的下拉菜单，然后选择以下选项之一。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">查看它</td> 
      <td> <p>允许您的收件人访问，以便在<strong>报告</strong> <img src="assets/reports-in-main-menu.png">区域查看并运行报告。</p> <p>您可以单击<strong>高级设置</strong>，以指定您是否希望用户或用户能够<strong>与系统中的任何人共享</strong>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理它</td> 
      <td> <p>允许收件人拥有对报告的完全编辑权限。</p> <p>您可以单击<strong>高级设置</strong>，以指定您是否希望用户能够<strong>删除</strong>系统中的报告，并<strong>与系统中的任何人共享</strong>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复前面的两个步骤向列表中添加其他名称并配置其选项。
1. （可选）单击共享框右上角的&#x200B;**齿轮**&#x200B;图标![](assets/gear-icon-settings-with-dn-arrow.jpg)，然后选择以下选项之一：

   * **将此设为外部用户公开：**&#x200B;选择此选项可生成可与他人共享的URL。 具有URL的任何人都可以访问报表，而无需拥有Adobe Workfront许可证。

     >[!CAUTION]
     >
     >建议在与外部用户共享包含机密信息的对象时务必谨慎。 这样，他们便可以查看信息，而无需成为Workfront用户或您组织的一部分。

     >[!NOTE]
     >
     >如果报告有提示并公开共享，则运行该报告的用户必须登录到Workfront，才能使用提示运行报告。 如果他们无法登录Workfront，将看到未应用提示的报告。 有关共享带有提示的报告限制的更多信息，请参阅文章[向报告添加提示](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)中的[共享提示报告的限制](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports)部分。

   * **使其在系统范围内可见：**&#x200B;选择此选项以便Workfront中有权访问报告的所有人都可以查看报告。

1. 单击&#x200B;**保存**。
