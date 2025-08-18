---
user-type: administrator
product-area: system-administration;user-management
keywords: 添加，用户，组，添加，其他，分配，管理员，删除，用户，查看，角色，成员，导出，成员资格，数据
navigation-topic: create-and-manage-groups
title: 查看和管理组的成员资格
description: 作为Adobe Workfront管理员，您可以查看、添加、删除、导出、激活和停用您管理的任何组的成员。 您还可以编辑其用户档案，将更新添加到其用户档案，并将他们分配为组的附加组管理员。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: 2096cfa0fd4d0e7eeb85dbf00668dc1dd7fb1d99
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 1%

---

# 查看和管理组的成员资格

作为Adobe Workfront管理员，您可以查看、添加、删除、导出、激活和停用您管理的任何组的成员。 您还可以编辑其用户档案，将更新添加到其用户档案，并将他们分配为组的附加组管理员。

如果您的组之上存在任何组，则其管理员还可以为您的组执行这些操作。 Workfront管理员也是如此（适用于任何组）。

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
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看和管理组的成员资格

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组**。

   在显示的列表中，Workfront管理员可以查看所有组和子组。 组管理员只能看到他们管理的组和子组。

1. 单击要编辑的组的名称。
1. 在显示的页面上，在左侧菜单中选择&#x200B;**组成员**，执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">将用户添加到组</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">单击<strong>添加成员</strong> <img src="assets/add-icon-plus-in-circle.png">，开始键入用户名，然后在此用户名出现时将其选定。</li> 
        <li value="2"> <p>对要添加的任何其他用户重复此操作。</p> <p>如果决定不添加该用户，可以单击名称右侧的X。</p> </li> 
        <li value="3">完成后，单击<strong>完成</strong>。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">从组中移除用户</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击<strong>删除成员</strong><img src="assets/remove-icon---x-in-circle.png">。</li> 
        <li value="2"> <p>在显示的警告消息中单击<strong>删除</strong>。</p> <p>通过单击<strong>搜索列表中的人员和组</strong>，在框中键入他们的姓名，然后在出现该名称时单击该名称，可以找到要从列表中删除的用户。</p> <p><b>注释</b>：  
          <ul> 
           <li>如果此组是要删除的用户的主组，则必须首先在该用户配置文件中分配另一个主组。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">主组概述</a>和<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户配置文件</a>。</li> 
           <li>如果该组只有一个组管理员，并且您需要将其从组中移除，则需要先将另一个组管理员分配给该组。</li> 
           <li>用户既可以单独属于子组，也可以属于父组。 从子组中删除某人时，该人员仍然是父组的一部分。 同样，当您从父组中移除它们时，它们仍将是子组的一部分。 如果您不希望用户具有父组所允许的访问权限，则必须从子组和父组中移除该用户（如果这些用户分别列在两个位置）。</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑用户的配置文件信息</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击<strong>编辑</strong> <img src="assets/edit-icon.png">。</li> 
        <li value="2"> <p>更改用户的配置文件信息。</p> <p>有关可以进行的更改的信息，请参阅<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户配置文件</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出用户成员资格数据</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击<strong>导出</strong> <img src="assets/export.png">。</li> 
        <li value="2"> <p>将数据导出为PDF、Excel或制表符分隔文件。</p> <p>有关导出数据的详细信息，请参阅<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">导出数据</a>。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看和编辑成员的组角色</td> 
      <td> <p><strong>组角色</strong>列列出了每个成员的角色。 作为组管理员，您可以双击成员的角色来进行更改。</p> <p>对于不是组管理员的组成员，此列不可编辑。</p> <p>组管理员始终位于列表顶部。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">向组成员发送评论</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">至少选择一个组成员，然后在工具栏中单击<strong>将更新发送给用户</strong>。</li> 
        <li value="2"><p>键入要发送给用户的评论以及用户配置文件的更新区域。</p>
        <p>有关详细信息，请参阅<a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">向其他用户发送私信</a>。</p></li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中激活用户</td> 
      <td>选择一个或多个非活动用户，然后单击<strong>激活用户</strong>以在Workfront中激活这些用户。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中取消激活用户</td> 
      <td>选择一个或多个活动用户，然后单击<strong>停用用户</strong><img src="assets/deactivate-user.png">以在Workfront中停用他们。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">按列排序</td> 
      <td>单击列的标题可按该列中的内容对列表进行排序。</td> 
     </tr> 
    </tbody> 
   </table>
