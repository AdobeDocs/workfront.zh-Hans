---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 停用团队
description: 您可以停用不再使用的团队，同时保留关联的历史数据。 Adobe Workfront管理员可以随时从“设置”中的“团队”区域重新激活团队。
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# 停用团队

您可以停用不再使用的团队，同时保留关联的历史数据。 [!DNL Adobe Workfront] 管理员可以随时从“设置”中的“团队”区域重新激活团队。 如果停用团队，该团队将不再显示在以下区域：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>自定义表单中的Typead字段</p> </li> 
    </ul> 
    <ul> 
     <li> <p>对象共享对话框</p> </li> 
     <li> <p>[!UICONTROL用户配置文件]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Teams]区域中的主选择下拉菜单</p> </li> 
     <li> <p>[!UICONTROL Assignments] typeaehaid</p> </li> 
     <li> <p>项目中的[!UICONTROL添加到看板]展示板对话框</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

在您搜索团队时，已停用的团队不会显示，但仍将显示在 [!UICONTROL 主队] 和其他团队（如果用户在停用之前被分配给团队）。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>计划</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 停用团队

在取消激活之前分配给该团队的任何工作仍会被分配。 我们建议您在停用团队之前重新分配工作。

>[!TIP]
>
>您可以创建一个报表，以筛选仍然分配了已停用团队的任何任务或问题。

在使用请求队列时，如果停用路由规则中指派为默认团队的团队，则该团队将保持不变，并且请求仍会路由到停用的团队。 我们建议您在停用团队之前，与活动团队一起更新路由规则。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **[!UICONTROL 团队]**.
1. 单击 **[!DNL Switch team]** 图标，然后从下拉菜单中选择新团队，或在搜索栏中搜索团队。
1. 单击 **[!UICONTROL 更多]** 菜单，然后选择 **[!UICONTROL 编辑]**.

   ![](assets/edit-team-settings-350x205.png)

1. 清除 **[!UICONTROL 处于活动状态]** 复选框。
1. 单击 **[!UICONTROL 保存更改]**.

## 已知限制

已停用的团队将显示在以下区域：

* 中的“所有者”字段 [!DNL Workfront Goals]. 这需要额外的许可证 [!DNL Adobe Workfront Goals]. 有关更多信息，请参阅 [开始使用 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
