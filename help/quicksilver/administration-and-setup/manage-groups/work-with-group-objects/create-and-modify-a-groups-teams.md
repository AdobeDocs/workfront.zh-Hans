---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和修改组的团队
description: 在“组”区域中查看由您管理的组时，可以查看与该组及其任何子组关联的团队并与之合作。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# 创建和修改组的团队

在“组”区域中查看由您管理的组时，可以查看与该组及其任何子组关联的团队并与之合作。

如果您的组上有任何组，则其管理员也可以为您的组执行这些操作。 Workfront管理员（对于任何组）也是如此。

有关拥有计划许可证的用户如何创建团队的信息，请参阅 [创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

有关Workfront管理员如何创建团队的信息，请参阅 [从“设置”(Setup)区域创建团队](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 从“组”区域查看、处理组并为组创建团队

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组** ![](assets/groups-icon.png).

1. 单击要为其创建或修改团队的组名称。
1. 在左侧面板中，单击 **团队** ![](assets/teams.png) 列出与组及其可能拥有的任何子组关联的团队。

1. 执行以下任一操作：

   * **添加团队**:单击 **新建团队**，然后使用以下选项对其进行配置：
   <!-- WRITER please check table below. I stripped out wonky conditions-->

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
       <td> <p> 系统将使用您正在查看的组填充新组合的组字段。 如果要将团队与其他组关联，请开始键入该组的名称，然后在显示时选择该名称。</p> <p>您可以通过将鼠标悬停在相应的组上并单击信息图标，确保将相应的组与团队关联 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> <p><b>注意</b>:将团队分配到组或子组后，该组或子组的任何组管理员都可以管理团队，而不是其成员。 群组管理员可以从主菜单转到“团队”区域，然后单击“切换团队”箭头 <img src="assets/switch-team-icon.png" alt="切换团队图标"> 列出分配给其管理的组的所有团队。</p> </td> 
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

   * **编辑团队**:至少选择一个团队，单击 **the** “编辑”图标 ![](assets/edit-icon.png)，然后使用以下选项对其进行配置：

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
       <td> <p>将团队与组关联。 开始键入组的名称，然后在显示时选择该名称。</p> <p>您可以通过将鼠标悬停在相应的组上并单击信息图标，确保将相应的组与团队关联 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> <p><b>注意</b>:将团队分配到组或子组后，该组或子组的任何组管理员都可以管理团队，而不是其成员。 群组管理员可以从主菜单转到“团队”区域，然后单击“切换团队”箭头 <img src="assets/switch-team-icon.png" alt="切换团队图标"> 列出分配给其管理的组的所有团队。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">所有者</td> 
       <td>选择团队的所有者。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">团队成员</td> 
       <td> <p>添加和团队成员。 开始键入用户的名称，然后在显示时选择该名称。 重复此过程以向团队添加多个用户。</p> <p><b>笔尖</b>:您可以向团队添加的用户数量没有限制。 但是，我们建议不要在一个团队中拥有过多的用户，因为该团队的工作管理可能变得过于复杂。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">描述</td> 
       <td>键入团队的描述。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">布局模板</td> 
       <td> <p>开始键入您希望团队使用的布局模板的名称，然后在显示时单击该名称。</p> <p>当您将使用此布局模板的团队指定为用户的主团队时，此团队中的所有用户都将看到此布局模板中的自定义设置。<br>他们的单个布局模板设置将覆盖主团队布局模板的设置。 </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">敏捷</td> 
       <td>指定这是否是敏捷团队。 有关敏捷团队及其工作管理方式的信息，请参阅 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建敏捷的团队</a>.</td> 
       </tr> 
       <tr> 
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

   * **删除团队**:至少选择一个团队，然后单击删除图标 ![](assets/delete.png).
   * **导出团队列表**:单击 **导出** ![](assets/export.png)，然后为导出列表选择所需的文件格式。
