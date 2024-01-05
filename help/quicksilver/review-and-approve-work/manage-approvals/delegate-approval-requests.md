---
product-area: projects
navigation-topic: approvals
title: 委托审批请求
description: 委托审批请求允许您分配另一个用户来审批您的请求一段时间，例如，如果您将在休假时不在办公室。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: 45c0af640daa7bf0c4cb342e55a88a98a745cfc3
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 0%

---

# 委托审批请求

您可以在外出时临时委派分配给您的工作。 您可以委派任务和问题分配，也可以委派审批请求。 本文介绍了如何委托审批请求。 有关委派任务和问题分配的信息，请参阅 [管理任务和问题委派](../../manage-work/delegate-work/how-to-delegate-work.md).

您可以委托以下类型的审批，而不管该审批是如何分配给您的（无论是直接分配给您，还是分配给您所属的团队或您的工作角色）：

* 项目审批
* 任务审批
* 问题审批

您无法委派时间表、文档或验证审批。

>[!NOTE]
>
>为了确保与您计划委派审批的日期不会出现任何不一致，我们建议用户配置文件的时区与计划的时区相匹配。 有关更多信息，请参阅以下文章：
>
>* [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> <p>审核或更高</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划或许可证类型，请与Workfront管理员联系。

## 了解委托审批的用户访问权限

在指定的审批期间，您向其委托审批请求的用户具有以下能力：

* 可以批准或拒绝未做出决策的现有审批请求
* 可以批准和拒绝在指定时间段内收到的新批准请求
* 被授予对等待审批对象的查看权限

  >[!NOTE]
  >
  > Adobe Workfront管理员可以限制用户访问某些对象类型。 当用户无权访问某个对象类型并且该类型的审批委托给用户时，用户对该对象没有“查看”权限。 但是，用户仍然可以批准或拒绝来自 **主页** 页面，如中所述 [审批工作](../../review-and-approve-work/manage-approvals/approving-work.md).\
  例如，用户A属于组A。Workfront管理员已限制组A的访问权限，以便该组中的用户无法查看Workfront中的任务。 如果任务审批请求委托给用户A，则用户A无法查看与审批关联的任务。 但是，用户A可以从主页批准或拒绝审批请求。

  有关Workfront管理员如何限制对“设置”中对象类型的访问的信息，请参阅  [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

审批委托停止或被取消后，指定为审批者的用户：

* 不再具有审批需要审批的项目的工作的权限
* 继续拥有对工作项的查看权限\
  通过审批委派被授予对象查看权限的用户仍保留该查看权限，即使审批委派停止或被撤回后也是如此。 要移除在委托审批期间用户有权访问的任何对象的“查看”访问权限，您必须转到该对象并直接从该对象移除访问权限。

## 委托主页区域中的审批请求

* [将您的审批委派给其他用户](#delegate-your-approvals-to-another-user)
* [更新或停止审批委托](#update-or-stop-an-approval-delegation)
* [查看委托的审批](#view-delegated-approvals)

### 将您的审批委派给其他用户 {#delegate-your-approvals-to-another-user}

您可以委托以下类型的审批，而不管该审批是如何分配给您的（无论是直接分配给您，还是分配给您所属的团队或您的工作角色）：

* 项目审批
* 任务审批
* 问题审批

您无法委派时间表、文档或验证审批。

委派审批时请考虑以下事项：

* 当您委托审批时，将委托所有审批。 您不能委托单个审批请求。
* 您只能将审批委派给一个用户；不能同时将审批委派给多个用户。\
  所有项目、任务和问题的所有审批都委托给您指定的用户。
* 最多5个用户可以同时将审批委派给同一用户。 换言之，不能将单个用户同时指定为5个以上用户的临时批准者。
* 有关批准的活动显示在更新选项卡上。 必须启用“Show System Updates（显示系统更新）”。 委托审批的用户和被委托审批的用户都会收到有关审批活动的电子邮件通知。

要将审批委派给其他用户，请执行以下操作：

1. 单击 **主页** 图标 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   * 请将其替换为用于说明贵组织的自定义图像。 在这种情况下，图标的外观将与本文中显示的有所不同。
   * 将链接到该页面的页面替换为其他页面。 在此例中，单击 **主菜单** ![](assets/main-menu-icon.png) （位于页面的右上角），然后单击 **主页**.

   或

   单击 **主菜单** 图标> **您的姓名** > **空闲时间** 在左侧面板中。

1. （可选，视情况而定）在“主页”(Home)区域中，单击 **筛选** 下拉菜单，然后单击 **审批**.

1. （视情况而定）单击 **委托我的审批**

   或

   如果您的系统管理员或组管理员启用了任务和问题委派，请单击 **委派**，然后单击 **委托审批**.

   ![](assets/delegate-approvals-nwe.png)

1. 在“委托我的审批”部分指定以下信息：

   * **名称**：开始键入要将审批委派到的用户的名称，然后单击下拉菜单中显示的名称。
   * **开始日期**：选择批准开始转发的日期。 转发从您选择的日期的凌晨12:00开始。\
     开始日期必须是当前日期或将来日期。
   * **结束日期**：执行下列操作之一：

      * 选择要停止转发的审批日期。 转发在您选择的日期晚上11:59结束。
      * 选择 **无结束日期** 以配置Workfront无限期地委托审批。

1. 单击&#x200B;**保存**。

### 更新或停止审批委托 {#update-or-stop-an-approval-delegation}

1. 单击 **主页** 图标 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   * 请将其替换为用于说明贵组织的自定义图像。 在这种情况下，图标的外观将与本文中显示的有所不同。
   * 将链接到该页面的页面替换为其他页面。 在此例中，单击 **主菜单** ![](assets/main-menu-icon.png) （位于页面的右上角），然后单击 **主页**.

1. 单击 **筛选** 下拉菜单，然后单击 **审批**.

1. （视情况而定）单击 **编辑委派**

   或

   如果您的系统管理员或组管理员启用了任务和问题委派，请单击 **编辑委派**，然后单击 **委托审批**.

1. （视情况而定）执行以下任一操作：

   * 要更新现有的审批委托：更改显示的信息，然后单击 **保存**.

   * 要停止现有委派：请单击 **停止委派**，然后单击 **停止委派** 以确认。

     ![](assets/stop-delegation-nwe.png)

### 查看委托的审批 {#view-delegated-approvals}

您只能在工作列表中查看以下类型的批准委托：

* 项目审批
* 任务审批
* 问题审批

要查看委托的审批，请执行以下操作：

1. 单击 **主页** 图标 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   * 请将其替换为用于说明贵组织的自定义图像。 在这种情况下，图标的外观将与本文中显示的有所不同。
   * 将链接到该页面的页面替换为其他页面。 在此例中，单击 **主菜单** ![](assets/main-menu-icon.png) （位于页面的右上角），然后单击 **主页**.

1. 单击 **筛选** 下拉菜单，然后单击 **审批**.\
   默认情况下，所有审批都显示在列表中，包括分配给您的审批和分配给您的审批。

   ![](assets/delegated-to-me-nwe-350x93.png)
