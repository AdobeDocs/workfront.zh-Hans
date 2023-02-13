---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 重新排序组状态
description: 作为组管理员，您可以更改您管理的组的项目、任务和问题状态的顺序。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 6%

---

# 重新排序组状态

作为组管理员，您可以更改您管理的组的项目、任务和问题状态的顺序。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

如果您管理的组上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员（对于任何组）也是如此。

>[!NOTE]
>
>* Workfront管理员可以重新排序系统级别的状态。 这不会影响组内状态的顺序。
>
>  但是，新创建的顶级组中的状态将继承系统级别状态的顺序。 （新子组会继承组一级中状态的顺序。）
>
>* 您可以重新排序锁定的状态。 有关锁定状态的信息，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
>


## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划* </td> 
   <td>任意</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 状态的默认顺序

默认情况下，状态按以下顺序显示：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">项目</th> 
   <th width="33.33%">任务</th> 
   <th width="33.33%">问题</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
     <p>目前</p> 
     <p>废弃</p> 
     <p> 保持 </p> 
     <p> 计划 </p> 
     <p> 完成 </p> 
     <p> 已请求 </p> 
     <p> 已批准 </p> 
     <p> 被拒绝 </p> 
     <p> 想法 </p> 
   </td> 
   <td> 
     <p>新</p> 
     <p>进行中</p> 
     <p>完成</p> 
   </td> 
   <td> 
     <p>新</p> 
     <p>进行中</p> 
     <p>重新打开</p> 
     <p>等待反馈</p> 
     <p>保持</p> 
     <p>无法复制</p> 
     <p>已关闭</p> 
     <p>已解决</p> 
     <p>确认完成</p> 
     <p>不会解决</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## 对您管理的组中的任务和项目的状态重新排序

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组**，然后单击群组的名称。
1. 在左侧面板中，单击 **状态**.
1. 在显示的状态列表上方，单击 **项目** 或 **任务** 选项卡。

1. 按所需的顺序拖放状态。

   新状态顺序会自动保存。

1. 要测试新状态顺序，请转到与组关联的任务或项目，单击右上角的状态，并确保显示的状态按您配置的顺序。

## 重新排列问题状态

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组**，然后单击群组的名称。
1. 在左侧面板中，单击 **状态**.
1. 单击 **问题** 选项卡。
1. （可选）选择问题类型(**错误报告**, **更改顺序**, **问题**&#x200B;或 **请求**)。

   >[!NOTE]
   >
   >* 您无法自定义主控列表的状态顺序。
   >* 我们建议您按相同方式对每个问题类型的状态进行排序。 有关问题类型的更多信息，请参阅 [配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).


1. 按所需的顺序拖放状态。

   新状态顺序会自动保存。

1. 要测试新状态顺序，请转到与组关联的问题，单击右上角的状态，并确保显示的状态按您配置的顺序。
