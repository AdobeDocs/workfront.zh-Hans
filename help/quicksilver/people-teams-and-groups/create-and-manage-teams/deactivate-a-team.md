---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: 停用或删除团队
description: 您可以停用不再使用的团队，同时保留关联的历史数据。 Adobe Workfront管理员可以随时从“设置”的团队区域重新激活团队。
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# 停用或删除团队

您可以停用不再使用的团队，同时保留关联的历史数据。 [!DNL Adobe Workfront]管理员可以随时从“设置”中的“团队”区域重新激活团队。 如果取消激活某个团队，则该团队将不再显示在以下区域中：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>自定义表单中的预输入字段</p> </li> 
    </ul> 
    <ul> 
     <li> <p>对象的“共享”对话框</p> </li> 
     <li> <p>[!UICONTROL 用户配置文件]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL 团队]区域中的主选择下拉菜单</p> </li> 
     <li> <p>[!UICONTROL Assignments]预输入</p> </li> 
     <li> <p>项目中的[!UICONTROL 添加到Kanban]展示板对话框</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

当您搜索团队时，已停用的团队不会显示，但如果用户在停用之前被分配到团队，则仍会显示在[!UICONTROL 主团队]和其他团队中。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td>
  </tr>
  <tr>
   <td>访问级别配置</td>
   <td><p>要停用团队，不需要配置。</p>
   <p>要删除团队，您必须是系统管理员。</p></td>
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 取消激活团队

在停用之前分配给团队的任何工作仍会得到分配。 我们建议您在停用团队之前重新分配工作。

>[!TIP]
>
>您可以创建一个报告，以筛选仍未分配已停用团队的任何任务或问题。

使用请求队列时，如果您停用在路由规则中指定为默认团队的团队，则团队会保留，请求仍会被路由到已停用的团队。 我们建议在停用团队之前，使用活动团队更新路由规则。

{{step1-to-team}}

1. 单击&#x200B;**[!DNL Switch team]**&#x200B;图标，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   ![](assets/edit-team-settings.png)

1. 清除团队设置中的&#x200B;**[!UICONTROL 处于活动状态]**&#x200B;复选框。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 停用团队的已知限制

已停用的团队在以下区域显示：

* [!DNL Workfront Goals]中的“所有者”字段。 这需要[!DNL Adobe Workfront Goals]的额外许可证。 有关详细信息，请参阅[开始使用 [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md)。

## 删除团队

只有系统管理员可以删除团队。 如果您是团队所有者（但不是管理员）并尝试删除团队，您将看到一条错误消息。

要删除团队，请执行以下操作：

{{step1-to-team}}

1. 单击&#x200B;**[!DNL Switch team]**&#x200B;图标，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 删除]**。

   ![](assets/edit-team-settings.png)

1. 单击确认消息上的&#x200B;[!UICONTROL **确认**]&#x200B;以永久删除团队。 无法恢复已删除的团队。
