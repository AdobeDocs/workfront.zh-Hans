---
title: 从设置区域创建团队
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: 作为Adobe Workfront管理员，您可以从设置区域创建团队。
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '542'
ht-degree: 4%

---

# 从设置区域创建团队

作为Adobe Workfront管理员，您可以从设置区域创建团队。 有关团队的信息，请参阅[团队概述](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)。

>[!NOTE]
>
>* 组管理员可以从“设置”区域为其管理的组创建团队。 有关详细信息，请参阅[创建和修改组的团队](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)。
>* 具有Standard或Plan许可证的用户也可以从Teams区域创建团队。 有关详细信息，请参阅[创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。

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

## 创建团队

{{step-1-to-setup}}

1. 单击&#x200B;**团队**，然后单击&#x200B;**新建团队**。

1. 在显示的&#x200B;**新团队**&#x200B;框中，指定以下信息：

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
      <td> <p>如果要将团队与组相关联，请开始键入组的名称，然后在该组出现时选择该名称。</p> <p>您可以通过将鼠标悬停在该组上并单击其旁边显示的信息图标<img src="assets/info-icon.png">，来确保将正确的组与该团队相关联。 这将显示一个工具提示，其中列出了有关组的信息，例如组及其上各组的层次结构。</p> <p><b>注意</b>：将团队分配给组或子组时，该组或子组的任何组管理员都可以管理团队，而无需成为其成员。 组管理员可以从主菜单转到团队区域，然后单击切换团队箭头<img src="assets/switch-team-icon.png" alt="“切换团队”图标">以列出分配给他们管理的组的所有团队。</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">这是敏捷团队</td> 
      <td>如果要将此新团队配置为Agile团队，请选择此项目。 有关Agile团队的详细信息，请参阅<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">创建Agile团队</a>。</td> 
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

1. 单击&#x200B;**创建团队**。

## 团队所有者

创建团队时，默认情况下您会成为团队所有者。

在创建团队的报告时，您可以查看所有团队的团队所有者，并在报告中包含“所有者名称”字段。 （有关创建报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。）
