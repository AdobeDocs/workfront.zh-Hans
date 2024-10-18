---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 批准工时表
description: 批准时间表的过程使经理能够了解其直接下属的工作时间。 审批者可以验证记录的所有时间是否分配到了正确的区域，以及期间是否记录了足够的小时数。
author: Alina
feature: Timesheets
exl-id: b27b3307-f61b-456d-8076-590d1c391b4b
source-git-commit: 9d0caff0381ee50bf8dd7060bebafb5354c0f0d8
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# 批准工时表

<!--Audited: 8/2024-->

批准时间表的过程使经理能够了解其直接下属的工作时间。 审批者可以验证记录的所有时间是否分配到了正确的区域，以及期间是否记录了足够的小时数。

Adobe Workfront提供将时间表批准配置为支持此区域的功能。

有关提交时间表的信息，请参阅[提交时间表以供审批](../../timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront计划</p></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> <p>新增：标准</p>
   <p>当前：计划 </p> 
   <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>对时间表和小时数的管理访问权限 </p> </td> 
  </tr>

</td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 指定时间表批准者

通常，时间表由职能经理或人力资源人员批准。 时间表通常不由项目经理批准。 项目经理可以批准登录项目的时间，但团队或人力资源经理应批准工时表。

创建时间表配置文件时，会定义时间表批准者。 您必须拥有计划许可证才能被指定为批准者。

有关指定时间表批准者的详细信息，请参阅文章[创建、编辑和分配时间表配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)中的[创建或编辑时间表配置文件](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md#create)部分。

## 批准工时表

您可以批准已提交且被指定为批准者的任何时间表。 在提交时间表以供审批时，该时间表会列在您&#x200B;**主页**&#x200B;区域的&#x200B;**我的审批**&#x200B;小部件中。 有关详细信息，请参阅[批准工作](../../review-and-approve-work/manage-approvals/approving-work.md)。

如果设置了以下通知设置，则提交时间表以供审批的用户会在时间表获得批准后收到一封电子邮件：

* Workfront管理员已向用户启用了时间表批准和向用户事件处理程序启用了时间表拒绝。 有关启用事件通知的信息，请参阅[事件通知类型](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)。
* 在用户配置文件页面上启用了我的时间表已批准个人通知。 有关详细信息，请参阅[修改您自己的电子邮件通知](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)。

### 从时间表区域批准时间表

{{step1-to-timesheets}}

**时间表**&#x200B;区域打开。

1. （视情况而定）如果上次访问时打开，请单击屏幕左上角的&#x200B;**返回到时间表**。

1. 选择页面右上角的&#x200B;**我的工时表批准**&#x200B;以仅查看您批准的时间表

   或

   选择时间表列表顶部的&#x200B;**我的时间表审批**&#x200B;过滤器。

   ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   >[!NOTE]
   >
   >如果您的Workfront管理员或组管理员从设置区域的列表控件或布局模板中删除了“我的时间表批准”过滤器，则“我的时间表批准”选项不会显示在时间表列表顶部或过滤器列表中。
   >
   >有关详细信息，请参阅[使用布局模板自定义筛选器、视图和分组](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （可选）单击时间表列表顶部的&#x200B;**搜索**&#x200B;图标![](assets/search-icon.png)，然后键入关键字以查找特定时间表。 您可以搜索时间范围，或所有者或审批者的姓名。
1. 单击要批准的工时表的时间范围。 此时将打开时间表。

   >[!TIP]
   >
   >等待批准的工时表的状态为[!UICONTROL 已提交]。


1. 单击&#x200B;**批准**

   或

   如果要拒绝时间表，请单击时间表左下角的&#x200B;**拒绝**。

   如果批准，时间表状态将更改为&#x200B;**已关闭**。

   如果被拒绝，时间表状态将更改为&#x200B;**已拒绝**。

### 批准主页区域中的工时表

{{step1-to-home}}

此时将打开“主页”区域。

1. 确保已将&#x200B;**我的审批**&#x200B;构件添加到您的主页区域。 有关详细信息，请参阅[新主页中的添加、编辑或删除构件](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md)。
1. 在“我的审批”构件中查找工时表审批。
1. （可选）展开“批准”或“拒绝”按钮右侧的下拉菜单以添加有关您的决策的评论，然后单击“**添加**”。
1. 单击以下按钮之一做出批准决定：

   * 批准
   * 拒绝

   审批将从&#x200B;**我的审批**&#x200B;构件中删除。


