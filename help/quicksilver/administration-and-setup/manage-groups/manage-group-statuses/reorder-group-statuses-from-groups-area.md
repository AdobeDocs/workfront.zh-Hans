---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 重新排序组状态
description: 作为组管理员，您可以更改所管理组的项目、任务和问题状态的顺序。
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

作为组管理员，您可以更改所管理组的项目、任务和问题状态的顺序。

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

>[!NOTE]
>
>* Workfront管理员可以在系统级别对状态重新排序。 这不会影响组中状态的顺序。
>
>  但是，新创建的顶级组中的状态将继承系统级状态的顺序。 （新子组继承了组内向上一级的状态顺序。）
>
>* 您可以对锁定状态重新排序。 有关锁定状态的信息，请参阅[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)。
>

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划* </td> 
   <td>任何</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.groups"> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a>和<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果需要了解您拥有的计划或许可证类型，请与Workfront管理员联系。

## 默认状态顺序

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
     <p>已停止</p> 
     <p> 暂停 </p> 
     <p> 规划中 </p> 
     <p> 完成 </p> 
     <p> 已请求 </p> 
     <p> 已审批 </p> 
     <p> 被拒绝 </p> 
     <p> 想法 </p> 
   </td> 
   <td> 
     <p>新建</p> 
     <p>正在进行中</p> 
     <p>完成</p> 
   </td> 
   <td> 
     <p>新建</p> 
     <p>正在进行中</p> 
     <p>重新打开</p> 
     <p>等待反馈</p> 
     <p>暂停</p> 
     <p>无法复制</p> 
     <p>已关闭</p> 
     <p>已解决</p> 
     <p>确认完成</p> 
     <p>不会解决</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## 重新排序您管理的组中任务和项目的状态

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 在左侧面板中，单击&#x200B;**组**，然后单击组的名称。
1. 在左侧面板中，单击&#x200B;**状态**。
1. 在显示的状态列表上方，单击&#x200B;**项目**&#x200B;或&#x200B;**任务**&#x200B;选项卡。

1. 按所需的顺序拖放状态。

   新的状态顺序会自动保存。

1. 要测试新的状态顺序，请转到与组关联的任务或项目，单击右上角的状态，并确保显示的状态符合您配置的顺序。

## 重新排序问题的状态

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![](assets/main-menu-icon.png)，然后单击&#x200B;**设置** ![](assets/gear-icon-settings.png)。

1. 在左侧面板中，单击&#x200B;**组**，然后单击组的名称。
1. 在左侧面板中，单击&#x200B;**状态**。
1. 单击&#x200B;**问题**&#x200B;选项卡。
1. （可选）选择问题类型（**错误报告**、**更改顺序**、**问题**&#x200B;或&#x200B;**请求**）。

   >[!NOTE]
   >
   >* 不能自定义主列表的状态顺序。
   >* 我们建议您采用相同的方式对每个问题类型的状态排序。 有关问题类型的详细信息，请参阅[配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 按所需的顺序拖放状态。

   新的状态顺序会自动保存。

1. 要测试新的状态顺序，请转到与组关联的问题，单击右上角的状态，并确保显示的状态符合您配置的顺序。
