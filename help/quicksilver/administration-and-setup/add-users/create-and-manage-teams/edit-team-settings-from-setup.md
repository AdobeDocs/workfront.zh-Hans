---
title: 从“设置”(Setup)区域编辑团队的设置
description: 作为Adobe Workfront管理员，您可以从“设置”区域编辑团队的设置。 您可以向团队添加用户、设置团队的布局模板，以及设置团队完成工作项目时状态的记录方式。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 2%

---

# 从“设置”(Setup)区域编辑团队的设置

作为Adobe Workfront管理员，您可以从“设置”区域编辑团队的设置。 您可以向团队添加用户、设置团队的布局模板，以及设置团队完成工作项目时状态的记录方式。

有关团队的信息，请参阅 [团队概述](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* 群组管理员可以编辑其所管理群组的团队设置。 有关更多信息，请参阅 [创建和修改组的团队](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* 拥有计划许可证的用户可以从“人员”区域编辑团队的设置。 有关更多信息，请参阅 [编辑团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
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

## 编辑团队的设置

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **团队** 中。
1. 选择团队，然后单击 **编辑** ![](assets/edit-icon.png).

1. 进行以下任一更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">团队名称</td> 
      <td>键入团队的名称。</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">活动 </td> 
       <td>默认情况下，新团队和现有团队会启用此选项。 禁用它以停用团队。 有关更多信息，请参阅 <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">停用团队</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">组</td> 
      <td> <p>将团队与组关联。 开始键入组的名称，然后在显示时选择该名称。</p> <p><b>注意</b>:将团队分配到组或子组后，该组或子组的任何组管理员都可以管理团队，而不是其成员。 群组管理员可以从主菜单转到“团队”区域，然后单击“切换团队”箭头 <img src="assets/switch-team-icon.png" alt="切换团队图标"> 列出分配给其管理的组的所有团队。</p> <p>您可以通过将鼠标悬停在相应的组上并单击信息图标，确保将相应的组与团队关联 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者</td> 
      <td>选择团队的所有者。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">团队成员</td> 
      <td> <p>添加和团队成员。 开始键入用户的名称，然后在显示时选择该名称。 重复此过程以向团队添加多个用户。</p> 
      <p><b>笔尖</b>:您可以向团队添加任意数量的用户。 但是，我们建议不要在一个团队中添加过多数量，因为该团队的工作管理可能会变得过于复杂。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入团队的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">布局模板</td> 
      <td> <p>开始键入您希望团队使用的布局模板的名称，然后在显示时单击该名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">敏捷</td> 
      <td>指定这是否是敏捷团队。 有关敏捷团队及其工作管理方式的信息，请参阅 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建敏捷的团队</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">处理此项工作</td> 
      <td> <p>将“Work On It（处理它）”按钮更改为“Start（开始）”按钮。 当用户单击“开始”时，项目的状态将自动更新。</p> <p>有关如何配置“开始”按钮的更多信息，请参阅 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将“Work On It（处理它）”按钮替换为“Start（开始）”按钮</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成按钮</td> 
      <td> <p>自定义完成按钮。 有关更多信息，请参阅：</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">为任务配置完成按钮</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">针对问题配置完成按钮</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存更改**.
