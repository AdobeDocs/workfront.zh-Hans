---
product-area: resource-management
navigation-topic: resource-pools
title: 创建资源池
description: 资源池是用户集合，可帮助您在Adobe Workfront中更轻松地管理资源。 有关资源池的更多信息，请参阅资源池概述。
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '589'
ht-degree: 1%

---

# 创建资源池

资源池是用户集合，可帮助您在Adobe Workfront中更轻松地管理资源。 有关资源池的详细信息，请参阅 [资源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，其中包括对管理资源池的访问权限</p> <p>编辑对用户、项目和模板的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要将资源池与之关联的项目和模板的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建资源池 {#create-a-resource-pool}

1. 以有权编辑资源池的用户身份登录。\
   有关更多信息，请参阅 [创建资源池](#create-a-resource-pool).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。

1. 单击 **资源化**.
1. 单击 **资源池** 中。\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. 单击 **新资源池**.
1. 指定以下内容：

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名称</strong></td>
      <td>这是资源池的名称。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>描述</strong></td>
      <td>这是有关此资源池的简要说明。 例如，您可以指定应该用于什么目的。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>池成员</strong></td>
      <td><p> 将用户逐个添加到资源池。<br>或 <br>一次向资源池添加大量用户。 您可以添加以下与用户或用户集合关联的实体之一：
        <ul>
         <li><strong>团队</strong>:团队的所有成员都将添加到资源池。</li>
         <li><strong>群组</strong>:组的所有成员都将添加到资源池。</li>
         <li><strong>角色</strong>:与该角色关联的所有用户都将添加到资源池。</li>
         <li><strong>公司</strong>:公司中的所有用户都将添加到资源池。</li>
        </ul><p>提示：您只能添加活动用户、团队、 <span>角色，</span> 或公司。</p><p>注意：如果用户成为组、组、公司的成员，或在将组、组、公司或作业角色添加到资源池后与作业角色关联，则新成员不会自动添加到资源池中。 <br>如果用户属于您添加的团队、组、公司和作业角色，则同时，该用户将只被添加到资源池一次。<br>添加到资源池后被停用的用户在用户列表中显示为灰显，并标记为已停用。</p></p></td>
     </tr>
    </tbody>
   </table>

1. （可选）使用 **撤消** 用于删除通过群组、团队、公司或工作角色添加的用户的链接。

   >[!NOTE]
   >
   >资源池中可以拥有的用户数量没有限制。 但是，我们建议不要向资源池添加太多用户，因为如果不这样做，资源管理可能会成为一项挑战。 用户列表仅显示资源池中的前2,000个用户，并按字母顺序列出这些用户。

   ![Resource_pools_NEW___UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. （可选）单击用户名右侧的X图标以删除用户。 有关从资源池中删除用户的详细信息，请参阅 [从资源池中删除用户](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md).
1. （可选）使用 **搜索** 选项，以在资源池中查找用户。
1. 单击&#x200B;**创建**。
