---
product-area: resource-management
navigation-topic: resource-pools
title: 创建资源池
description: 资源池是用户集合，可帮助您更轻松地在Adobe Workfront中管理资源。
author: Lisa
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: ca882fbb8b29fc728d9c688c6c671cfdf677c2cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 1%

---

# 创建资源池

{{highlighted-preview}}

资源池是用户集合，可帮助您更轻松地在Adobe Workfront中管理资源。 有关资源池的详细信息，请参阅[资源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，其中包括对管理资源池的访问权限</p> <p>编辑对用户、项目和模板的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要与资源池关联的项目和模板的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

## 创建资源池 {#create-a-resource-pool}

{{step1-to-resourcing}}

1. 单击左侧面板中的&#x200B;**资源池**。

   <span class="preview">预览环境中的示例图像：</span>
   <span class="preview">![资源池](assets/list-of-resource-pools.png)</span>

   生产环境中的示例图像：
   ![资源池](assets/resource-pools-tab-350x198.png)

1. 单击&#x200B;**新建资源池**。
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
      <td>这是有关此资源池的简短说明。 例如，您可以指定其使用目的。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>池成员</strong></td>
      <td><p> 将用户单独添加到资源池。<br>或<br>一次向资源池中添加大量用户。 您可以添加以下与用户或用户集合关联的实体之一：
        <ul>
         <li><strong>团队</strong>：团队的所有成员都已添加到资源池中。</li>
         <li><strong>组</strong>：组的所有成员都已添加到资源池中。</li>
         <li><strong>角色</strong>：与该角色关联的所有用户都已添加到资源池中。</li>
         <li><strong>公司</strong>：公司中的所有用户都已添加到资源池中。</li>
        </ul><p>提示：您只能添加活动用户、团队、<span>角色、</span>或公司。</p><br>您可能需要在对话框中向下滚动才能查看资源池中的所有用户。
        <p>注：如果将组、团队、公司或工作角色添加到资源池后，用户成为组、团队、公司的成员，或与工作角色相关联，则新成员不会自动添加到资源池中。 <br>如果用户属于您添加的团队、组、公司和工作角色，则用户只会被添加到资源池一次。<br>添加到资源池后已停用的用户在用户列表中显示为灰色，并标记为已停用。</p></p></td>
     </tr>
    </tbody>
   </table>

1. （可选）使用&#x200B;**撤消**&#x200B;链接删除通过组、团队、公司或工作角色添加的用户。 <span class="preview">（撤消功能在预览环境中暂时不可用。）</span>

   >[!NOTE]
   >
   >资源池中的用户数量没有限制。 但是，我们建议不要向资源池添加太多用户，否则资源管理可能会成为一个挑战。 用户列表仅显示资源池中的前2,000个用户，并且按字母顺序列出。

   <span class="preview">预览环境中的示例图像：</span>
   <span class="preview">![个用户已添加到资源池](assets/users-in-resource-pool.png)</span>

   生产环境中的示例图像：
   ![个用户已添加到资源池](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. （可选）单击用户名右侧的X图标可删除用户。 有关从资源池中删除用户的详细信息，请参阅[从资源池中删除用户](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)。
1. （可选）使用&#x200B;**搜索**&#x200B;选项在资源池中查找用户。
1. 单击&#x200B;**创建**。
