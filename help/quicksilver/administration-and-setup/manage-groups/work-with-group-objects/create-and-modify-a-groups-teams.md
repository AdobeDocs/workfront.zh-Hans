---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 创建和修改组的团队
description: 查看在组区域管理的组时，可以查看与组及其任何子组关联的团队并使用该团队。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '989'
ht-degree: 4%

---

# 创建和修改组的团队

查看在组区域管理的组时，可以查看与组及其任何子组关联的团队并使用该团队。

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

有关拥有Plan许可证的用户如何创建团队的信息，请参阅[创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。

有关Workfront管理员如何创建团队的信息，请参阅[从设置区域创建团队](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md)。

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
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从组区域查看、处理和创建组团队

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

1. 单击要为其创建或修改团队的组的名称。
1. 在左侧面板中，单击&#x200B;**团队** ![团队](assets/teams.png)列出与组及其可能具有的任何子组关联的团队。

1. 执行以下任一操作：

   * **添加团队**：单击&#x200B;**新建团队**，然后使用以下选项对其进行配置：

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
       <td> <p> 系统将使用您正在查看的组填写新团队的“组”字段。 如果要将团队与其他组相关联，请开始键入组的名称，然后在该组出现时选择该名称。</p> <p>您可以通过将鼠标悬停在该组上并单击其旁边显示的信息图标<img src="assets/info-icon.png">，来确保将正确的组与该团队相关联。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> <p><b>注意</b>：将团队分配给组或子组时，该组或子组的任何组管理员都可以管理团队，而无需成为其成员。 组管理员可以从主菜单转到团队区域，然后单击切换团队箭头<img src="assets/switch-team-icon.png" alt="“切换团队”图标">以列出分配给他们管理的组的所有团队。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">团队成员</td> 
       <td> <p>开始键入要加入团队的用户的名称，然后在下拉列表中显示的中时选择名称。 重复此过程以将多个用户添加到团队。</p> <p>您可以向团队添加的用户数量没有限制。 但是，我们建议一个团队中的用户数量不要过多，因为团队的工作管理可能过于复杂。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">描述</td> 
       <td>键入团队描述。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">日程表</td> 
       <td>为该团队选择将显示哪个日历选项卡。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">处理此项工作</td> 
       <td>将处理此项按钮更改为“开始”按钮。 当用户单击“开始”时，项目的状态会自动更新。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">完成按钮</td> 
       <td>选择单击“完成”按钮时要为项目设置的状态。</td> 
       </tr> 
      </tbody> 
     </table>

   * **编辑团队**：至少选择一个团队，单击&#x200B;****“编辑”图标![“编辑”图标](assets/edit-icon.png)，然后使用以下选项对其进行配置：

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
       <td> <p>将团队与组关联。 开始键入组的名称，然后在该组出现时选择该名称。</p> <p>您可以通过将鼠标悬停在该组上并单击其旁边显示的信息图标<img src="assets/info-icon.png">，来确保将正确的组与该团队相关联。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> <p><b>注意</b>：将团队分配给组或子组时，该组或子组的任何组管理员都可以管理团队，而无需成为其成员。 组管理员可以从主菜单转到团队区域，然后单击切换团队箭头<img src="assets/switch-team-icon.png" alt="“切换团队”图标">以列出分配给他们管理的组的所有团队。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">所有者</td> 
       <td>选择团队的所有者。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">团队成员</td> 
       <td> <p>添加和团队成员。 开始键入用户的名称，然后在该名称出现时将其选定。 重复此过程以将多个用户添加到团队。</p> <p><b>提示</b>：您可以向团队添加的用户数量没有限制。 但是，我们建议一个团队中的用户数量不要过多，因为团队的工作管理可能过于复杂。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">描述</td> 
       <td>键入团队描述。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">布局模板</td> 
       <td> <p>开始键入您希望团队使用的布局模板的名称，然后在该模板出现时单击它。</p> <p>当您将具有此布局模板的团队指定为用户的主团队时，该团队中的所有用户都将看到此布局模板中的自定义项。<br>其各自的布局模板设置将覆盖主团队布局模板的设置。 </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">敏捷</td> 
       <td>指定这是否为Agile团队。 有关Agile团队以及如何管理其工作的信息，请参阅<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建Agile团队</a>。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">处理此项工作</td> 
       <td> <p>将处理此项按钮更改为“开始”按钮。 当用户单击“开始”时，项目的状态会自动更新。</p> <p>有关如何配置“开始”按钮的详细信息，请参阅<a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">将处理它按钮替换为“开始”按钮</a>。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">完成按钮</td> 
       <td> <p>自定义完成按钮。 有关更多信息，请参阅：</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">配置任务的“完成”按钮</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">为问题配置“完成”按钮</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **删除团队**：至少选择一个团队，然后单击“删除”图标![删除图标](assets/delete.png)。
   * **导出团队列表**：单击&#x200B;**导出**![导出图标](assets/export.png)，然后选择导出列表所需的文件格式。
