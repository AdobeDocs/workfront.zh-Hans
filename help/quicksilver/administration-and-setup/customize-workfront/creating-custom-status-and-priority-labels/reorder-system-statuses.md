---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: 重新排序系统层和组状态
description: 作为Workfront管理员，您可以更改系统中每个人或单个组的项目、任务和问题状态的顺序。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 7%

---

# 重新排序系统级别和组状态

作为Workfront管理员，您可以更改系统中每个人或单个组的项目、任务和问题状态的顺序。

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![状态](assets/statuses.png)

>[!NOTE]
>
>* 在系统级别对状态重新排序不会影响组内状态的顺序。
>
>  但是，新创建的顶级组中的状态将继承系统级状态的顺序。 （新子组继承了组内向上一级的状态顺序。）
>
>* 您可以对锁定状态重新排序。 有关锁定状态的信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)。
>* 组管理员还可以对其组中使用的状态重新排序。 有关详细信息，请参阅[重新排序组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md)。
>

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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
    <ul> 
     <li>目前</li> 
     <li>已停止</li> 
     <li> 暂停 </li> 
     <li> 规划中 </li> 
     <li> 完成 </li> 
     <li> 已请求 </li> 
     <li> 已审批 </li> 
     <li> 被拒绝 </li> 
     <li> 想法 </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>新建</li> 
     <li>正在进行中</li> 
     <li>完成</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>新建</li> 
     <li>正在进行中</li> 
     <li>重新打开</li> 
     <li>等待反馈</li> 
     <li>暂停</li> 
     <li>无法复制</li> 
     <li>已关闭</li> 
     <li>已解决</li> 
     <li>确认完成</li> 
     <li>不会解决</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 对全系统或组的任务和项目状态重新排序

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**项目首选项>状态**。
1. （视情况而定）如果要对组的状态重新排序，请在右上角的框中开始键入组的名称，然后在组出现时单击该名称。

   ![系统状态](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. 在显示的状态列表上方，单击&#x200B;**项目**&#x200B;或&#x200B;**任务**&#x200B;选项卡。

1. 按所需的顺序拖放状态。

   新的状态顺序会自动保存。

1. 要测试新的状态顺序，请转到任务或项目，单击右上角的状态，并确保显示的状态符合您配置的顺序。

## 重新排序问题的状态

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**设置**![齿轮设置图标](assets/gear-icon-settings.png)。

1. 单击&#x200B;**项目首选项>状态。**
1. （视情况而定）如果要对组的状态重新排序，请在右上角的框中开始键入组的名称，然后在组出现时单击该名称。

   ![组](assets/issue-statuses-group-name.png)的问题状态

1. 单击&#x200B;**问题**&#x200B;选项卡。
1. （可选）选择问题类型（**错误报告**、**更改顺序**、**问题**&#x200B;或&#x200B;**请求**）。

   >[!NOTE]
   >
   >* 不能自定义主列表的状态顺序。
   >* 我们建议您采用相同的方式对每个问题类型的状态排序。 有关问题类型的详细信息，请参阅[配置请求类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md)。

1. 按所需的顺序拖放状态。

   新的状态顺序会自动保存。

1. 要测试新的状态顺序，请转到问题，单击右上角的状态，并确保显示的状态符合您配置的顺序。
