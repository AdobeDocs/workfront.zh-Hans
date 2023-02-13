---
user-type: administrator
product-area: system-administration;user-management
keywords: 添加，用户，组，添加，其他，分配，管理员，删除，用户，视图，角色，成员，导出，成员，数据
navigation-topic: create-and-manage-groups
title: 查看和管理群组成员关系
description: 作为Adobe Workfront管理员，您可以查看、添加、删除、导出、激活和停用您管理的任何群组成员。 您还可以编辑其配置文件、将更新添加到其配置文件，并将其分配为组的其他组管理员。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 219e5fa3-cf25-477d-82f6-046e3ff30989
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# 查看和管理群组成员关系

作为Adobe Workfront管理员，您可以查看、添加、删除、导出、激活和停用您管理的任何群组成员。 您还可以编辑其配置文件、将更新添加到其配置文件，并将其分配为组的其他组管理员。

如果您的组上有任何组，则其管理员也可以为您的组执行这些操作。 Workfront管理员（对于任何组）也是如此。

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
   <td> <p>计划 </p> <p>您必须是组的组管理员或Workfront管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">组管理员</a> 和 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;如果您需要了解您拥有的计划或许可证类型，请联系您的Workfront管理员。

## 查看和管理群组成员关系

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **群组**.

   在显示的列表中，Workfront管理员可以查看所有组和子组。 群组管理员只能查看他们管理的群组和子群组。

1. 单击要编辑的群组的名称。
1. 在显示的页面上，使用 **组成员** ，请执行以下任一操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">将用户添加到群组</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">单击 <strong>添加成员</strong> <img src="assets/add-icon-plus-in-circle.png">，开始键入用户的名称，然后在显示时将其选中。</li> 
        <li value="2"> <p>对要添加的任何其他用户重复此操作。</p> <p>如果您决定不添加该用户，可以单击名称右侧的X。</p> </li> 
        <li value="3">单击 <strong>完成</strong> 完成。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">从群组中删除用户</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击 <strong>删除成员</strong><img src="assets/remove-icon---x-in-circle.png">.</li> 
        <li value="2"> <p>单击 <strong>删除</strong> 在显示的警告消息中。</p> <p>通过单击 <strong>在列表中搜索人员和群组</strong>，在框中键入其名称，然后在出现时单击该名称。</p> <p><b>注释</b>:  
          <ul> 
           <li>如果此组是要删除的用户的主页组，则必须首先在用户的配置文件中分配另一个主页组。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-groups/groups-overview/home-groups.md" class="MCXref xref">主页组概述</a> 和 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>.</li> 
           <li>如果群组只有一个群组管理员，并且您需要将其从群组中删除，则需要先将另一个群组管理员分配给该群组。</li> 
           <li>用户可以单独属于某个子组以及父组。 从子组中删除某个人时，这些人仍属于父组。 同样，当从父组中删除它们时，它们将保留在子组的一部分。 如果您不希望用户具有允许父组访问的权限，则必须同时从子组和父组中删除该用户（如果这两个位置分别列在两处）。</li> 
          </ul> </p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">编辑用户的配置文件信息</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击 <strong>编辑</strong> <img src="assets/edit-icon.png">.</li> 
        <li value="2"> <p>更改用户的用户档案信息。</p> <p>有关可以进行的更改的信息，请参阅 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">编辑用户的配置文件</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">导出用户成员资格数据</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击 <strong>导出</strong> <img src="assets/export.png">.</li> 
        <li value="2"> <p>将数据导出为PDF、Excel或制表符分隔的文件。</p> <p>有关导出数据的更多信息，请参阅 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">导出数据</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">查看和编辑成员的组角色</td> 
      <td> <p>的 <strong>组角色</strong> 列列出每个成员的角色。 作为组管理员，您可以双击成员的角色以更改它。</p> <p>对于非群组管理员的群组成员，此列不可编辑。</p> <p>组管理员始终位于列表顶部。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">向群组成员发送评论</td> 
      <td> 
       <ol style="list-style-type: lower-alpha;"> 
        <li value="1">选择一个或多个用户名，然后单击 <strong>更新</strong> <img src="assets/comment-icon.png">.</li> 
        <li value="2">键入评论。</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中激活用户</td> 
      <td>选择一个或多个不活动的用户，然后单击 <strong>激活用户</strong> 在Workfront中激活它们。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在Workfront中停用用户</td> 
      <td>选择一个或多个活动用户，然后单击 <strong>停用用户</strong><img src="assets/deactivate-user.png"> 在Workfront停用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">按列排序</td> 
      <td>单击列的标题可按该列中的内容对列表进行排序。</td> 
     </tr> 
    </tbody> 
   </table>
