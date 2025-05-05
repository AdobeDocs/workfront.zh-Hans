---
title: 从设置区域编辑团队设置
description: 作为Adobe Workfront管理员，您可以从设置区域编辑团队设置。 您可以将用户添加到团队、设置团队的布局模板以及设置当团队完成工作项时如何记录状态。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 3%

---

# 从“设置”区域编辑团队设置

作为Adobe Workfront管理员，您可以从设置区域编辑团队设置。 您可以将用户添加到团队、设置团队的布局模板以及设置当团队完成工作项时如何记录状态。

有关团队的信息，请参阅[团队概述](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)。

>[!NOTE]
>
>* 组管理员可以编辑他们管理的组的团队设置。 有关详细信息，请参阅[创建和修改组的团队](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)。
>* 具有Standard或Plan许可证的用户可以从团队区域编辑团队设置。 有关详细信息，请参阅[编辑团队设置](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 编辑团队的设置

{{step-1-to-setup}}

1. 单击左侧面板中的&#x200B;**团队**。
1. 选择一个团队，然后单击&#x200B;**编辑** ![编辑图标](assets/edit-icon.png)。

1. 进行以下任何更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">团队名称</td> 
      <td>键入团队的名称。</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">为活动 </td> 
       <td>默认情况下，为新团队和现有团队启用此选项。 禁用此选项可取消激活团队。 有关详细信息，请参阅<a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">停用团队</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">组</td> 
      <td> <p>将团队与组关联。 开始键入组的名称，然后在该组出现时选择该名称。</p> <p><b>注意</b>：将团队分配给组或子组时，该组或子组的任何组管理员都可以管理团队，而无需成为其成员。 组管理员可以从主菜单转到团队区域，然后单击切换团队箭头<img src="assets/switch-team-icon.png" alt="“切换团队”图标">以列出分配给他们管理的组的所有团队。</p> <p>您可以通过将鼠标悬停在该组上并单击其旁边显示的信息图标<img src="assets/info-icon.png">，来确保将正确的组与该团队相关联。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者</td> 
      <td>选择团队的所有者。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">团队成员</td> 
      <td> <p>添加和团队成员。 开始键入用户的名称，然后在该名称出现时将其选定。 重复此过程以将多个用户添加到团队。</p> 
      <p><b>提示</b>：您可以向团队添加任意数量的用户。 但是，我们建议您不要在一个团队中添加过多数字，因为团队的工作管理可能过于复杂。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入团队描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">布局模板</td> 
      <td> <p>开始键入您希望团队使用的布局模板的名称，然后在该模板出现时单击它。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">敏捷</td> 
      <td>指定这是否为Agile团队。 有关Agile团队以及如何管理其工作的信息，请参阅<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建Agile团队</a>。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
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

1. 单击&#x200B;**保存更改**。
