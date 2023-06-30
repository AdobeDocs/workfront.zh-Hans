---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: 共享对象
description: 在分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑对象的权限。 有关授予对象访问权限的详细信息，请参阅创建或修改自定义访问级别。
author: Alina
feature: Get Started with Workfront
exl-id: 27a1beb9-e83a-4ef6-bf5f-ad52575a993c
source-git-commit: 5b4aa5c806d0f930250e9238d460833cd1aed71a
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 0%

---

# 共享对象

在分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑对象的权限。 有关授予对象访问权限的详细信息，请参见 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

除了授予用户的访问级别之外，您还可以授予他们查看或编辑您创建或有权共享的特定对象的权限。 有关访问级别和权限的更多信息，请参阅 [访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

权限特定于Workfront中的一个项目，并定义可以对该项目执行的操作。

有关共享对象权限的信息，请参见 [对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理员可以添加或移除系统中所有用户的任何项目的权限，而无需成为这些项目的所有者。

本文介绍了如何共享以下对象： 

* 项目、任务、问题
* Portfolio、项目群
* 文档

有关如何在Workfront中共享所有其他对象的信息，另请参阅以下文章：

* 有关模板，请参阅 [共享项目模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* 有关验证，请参阅 [在Workfront Proof中共享验证](../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).
* 有关报告、功能板和日历，请参阅以下文章：

   * [在Adobe Workfront中共享报表](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [共享功能板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [共享日历报告](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

  此外，请参阅 [共享报告、功能板和日历](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) 有关共享报告、功能板和日历的一般信息。 

* 有关筛选器、视图和分组，请参阅 [共享筛选器、视图或分组](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
* 有关文档文件夹，请参阅 [共享文档文件夹](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).
* 有关计划，请参阅 [在Scenario Planner中共享计划](../../scenario-planner/share-a-plan.md).

  这需要额外的许可证。

* 有关目标，请参阅 [在Workfront目标中共享目标](../../workfront-goals/workfront-goals-settings/share-a-goal.md). 这需要额外的许可证。

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对要共享对象的访问权限或更高</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看要共享的对象的权限或更高</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 共享单个对象 {#share-a-single-object}

1. 转到要共享的对象。

   有关可以共享哪些对象的信息，请参见 [对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
1. 对于项目、任务和问题：

   单击 **共享** 对象名称旁边的按钮。

   ![](assets/new-share-button.png)

   或

   对于文档、项目组合和程序：

   单击 **更多** 图标 ![](assets/more-icon.png)在对象名称旁边，然后单击 **共享** 或 **共享。**

   ![](assets/share-a-document-350x160.png)

1. 在 **授予 `<Object Name>` 访问** 字段中，开始键入要与其共享对象的用户、团队、角色、组或公司的名称，然后在名称出现在下拉列表中时单击该名称。

   例如，如果要共享项目，请使用 **授予项目访问权限** 字段。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

   ![](assets/nwe-project-sharing-modal-350x456.png)

   >[!TIP]
   >
   >如果多个图元具有类似的名称，则它们都列在其类型下。 图元名称按字母顺序显示。 但是，图元类型的显示顺序是随机的。
   >
   >
   >![](assets/sharing-entities-named-similarly-in-sharing-box-350x179.png)   >
   >

1. （可选）对要授予对象访问权限的每个用户、团队、角色或组重复步骤3。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: esnure this stays accurate; in the editor it looks like step 4 but one step is conditioned entirely for one version or another)
   </MadCap:conditionalText>
   -->

1. 通过单击下拉菜单，然后选择要授予的权限级别，指定您在步骤3中添加的每个用户、团队、角色、组或公司的权限。

   以下选项可用：

   * **查看：** 用户可以查看和共享该项目。 
   * **Contribute****：**用户可以进行更新、记录信息、进行细微编辑和共享，以及所有“查看”权限。

     >[!TIP]
     >
     >您只能将Contribute权限授予以下对象： 
     >
     >   
     >   
     * 项目
     * 任务
     * 问题
     >   
     >

   * **管理：**用户无需管理权限（在访问级别授予管理权限）以及所有“查看”和“贡献”权限，即可完全访问对象。

     >[!NOTE]
     >
      Workfront管理员或对象创建者能够从这些实体中删除权限。

      

     ![](assets/screen-shot-2013-12-04-at-1.13.11-pm.png)

1. （可选）单击 **高级选项** 以配置对象的特定权限。

   “查看”、“管理”和“贡献”选项根据所选对象而有所不同。\
   有关权限级别的详细信息，请参阅 [对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

   ![](assets/screen-shot-2013-12-04-at-1.14.11-pm.png)

1. （可选）要使此对象对系统中的所有用户都可用，请单击 **齿轮** 图标 ![](assets/gear-icon-settings-with-dn-arrow.jpg) ，然后在下拉菜单中，单击 **使其在系统范围内可见**.

   所有用户都可以根据您设置的权限查看对象。

1. （可选且有条件）共享项目时，单击 **齿轮** 图标 ![](assets/gear-icon-settings-with-dn-arrow.jpg)，然后在下拉菜单中，单击 **设置为我的项目访问模板** 以将权限设置为模板。\
   定义一个项目的权限后，下次从头开始创建项目时，将自动应用这些相同的权限。

   >[!NOTE]
   >
   项目访问模板将覆盖由访问级别的Workfront管理员授予您的共享默认值。\
   有关在访问级别中指定项目共享默认值的详细信息，请参阅 [授予对项目的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md) .>
   >
   <!--   >
   ><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   >
   >(NOTE: (this note also appears in Understanding Project Permissions.))   >
   ></MadCap:conditionalText>   >
   >-->   >
   >

   您可以指定共享模板时将从模板创建的项目的权限。 有关更多信息，请参阅 [共享项目模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

1. （可选）要使对象公开，请单击 **将此设为公开给外部用户**.

   >[!TIP]
   >
   此选项并非对所有对象都可用。

   ![](assets/make-public-system-wide-settings-sharing-box-on-document-nwe-350x481.png)

1. （视情况而定）如果将对象公开给外部用户，请单击 **复制链接，** 然后将链接分发给外部用户。\
   任何具有链接的用户都可以查看该对象。

   >[!CAUTION]
   >
   建议在与外部用户共享包含机密信息的对象时务必谨慎。 这允许他们查看信息，而无需成为Workfront用户或组织的一部分。

1. 单击&#x200B;**保存**。

## 批量共享对象

从对象列表中，您可以同时与其他用户、团队、组、工作角色或公司共享多个对象。

>[!IMPORTANT]
>
当您批量共享对象时，对各个对象具有权限的实体的名称不显示。 批量共享对象时，添加到共享列表的实体将被添加到所选对象中。 它们不会覆盖与单个对象相关联的实体。 

要批量共享对象，请执行以下操作：

1. 导航到对象列表。
1. 在列表中选择两个或多个对象。
1. 单击 **共享** 图标 ![](assets/share-icon.png).\
   在批量共享时，已拥有对象访问权限的用户不会列为可用。

   >[!NOTE]
   >
   如果您无权共享您选择的对象，则 **共享** 按钮不可见。

1. 在 **编辑 `<Object Name>` 访问权限** 字段中，开始键入要向其授予权限的用户、团队、组、工作角色或公司的名称。

   例如，如果要共享项目，请使用 **授予项目访问权限** 字段。

   ![](assets/share-multiple-projects-people-box-nwe-350x480.png)

1. 按照一节中的步骤4-9所述继续共享选定对象 [共享单个对象](#share-a-single-object) 本文章中。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure these steps stay accurate; always look at them in the viewer; because of condiitoning, the steps numbers in the editor are different!!!!!!*****)
   </MadCap:conditionalText>
   -->

1. 单击&#x200B;**保存**。
