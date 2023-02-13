---
title: 从“设置”(Setup)区域创建团队
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: 作为Adobe Workfront管理员，您可以从“设置”区域创建团队。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# 从“设置”(Setup)区域创建团队

作为Adobe Workfront管理员，您可以从“设置”区域创建团队。 有关团队的信息，请参阅 [团队概述](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* 群组管理员可以从“设置”区域为他们管理的群组创建团队。 有关更多信息，请参阅 [创建和修改组的团队](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* 拥有计划许可证的用户还可以从“人员”区域创建团队。 有关更多信息，请参阅 [创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
>


## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建团队

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **团队**，然后单击 **新建团队**.

1. 在 **新建团队** 框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">团队名称</td> 
      <td>键入团队的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">组</td> 
      <td> <p>如果要将团队与群组关联，请开始键入群组的名称，然后在显示时选择该名称。</p> <p>您可以通过将鼠标悬停在相应的组上并单击信息图标，确保将相应的组与团队关联 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> <p><b>注意</b>:将团队分配到组或子组后，该组或子组的任何组管理员都可以管理团队，而不是其成员。 群组管理员可以从主菜单转到“团队”区域，然后单击“切换团队”箭头 <img src="assets/switch-team-icon.png" alt="切换团队图标"> 列出分配给其管理的组的所有团队。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">团队成员</td> 
      <td> <p>开始键入要加入团队的用户名称，然后在下拉列表中显示时选择该名称。 重复此过程以向团队添加多个用户。</p> <p>您可以向团队添加的用户数量没有限制。 但是，我们建议不要在一个团队中拥有过多的用户，因为该团队的工作管理可能变得过于复杂。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入团队的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">日历</td> 
      <td>为该团队选择将显示哪个日历选项卡。</td> 
     </tr> 
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">这是 Agile 团队</td> 
      <td>如果要将此新团队配置为敏捷团队，请选择此项目。 有关敏捷团队的更多信息，请参阅 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建敏捷的团队</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">处理此项工作</td> 
      <td>将“Work On It（处理它）”按钮更改为“Start（开始）”按钮。 当用户单击“开始”时，项目的状态将自动更新。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成按钮</td> 
      <td>在单击完成按钮时，选择要为项目设置的状态。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **创建团队**.

## 团队所有者

在创建团队时，默认情况下您会成为团队所有者。

在为团队创建报表时，您可以查看所有团队的团队所有者，并在报表中包含“所有者名称”字段。 (有关创建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
