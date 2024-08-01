---
product-area: resource-management
navigation-topic: resource-pools
title: 从资源池中删除用户
description: 虽然资源池中的用户可以数量没有限制，但用户列表仅显示前2000个用户（按字母顺序列出）。
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: dfafeaeeca5805c84ff646d8a7a98120d34d44d9
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# 从资源池中删除用户

{{highlighted-preview}}

虽然资源池中的用户可以数量没有限制，但用户列表仅显示前2000个用户（按字母顺序列出）。

我们建议您删除已停用或已移动角色或部门的用户，以确保所有资源池中始终具有准确的用户列表。

有关资源池的详细信息，请参阅[资源池概述](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)。

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
   <td> <p>编辑对资源管理的访问权限，其中包括对管理资源池的访问权限</p> <p>查看或更高的用户访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>(NOTE:&nbsp;I don't think this is needed for removing users from the pool)</p> <p>Manage permissions for the projects, templates, and users you associate the Resource Pools with</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

## 从资源池中删除用户

当资源池中不再需要某些用户时，可以从资源池中删除这些用户。

要从资源池中删除用户，请执行以下操作：

{{step1-to-resourcing}}

1. 单击左侧面板中的&#x200B;**资源池**。
1. 选择资源池并单击&#x200B;**编辑**。
或\
   单击资源池的名称。

1. 在&#x200B;**在此资源池**&#x200B;中搜索字段中开始键入要删除的用户名。\
   或\
   如果要删除与这些实体关联的所有用户，请开始键入公司、工作角色、团队或组的名称。

   <span class="preview">预览环境中的示例图像：<span>
   ![从资源池中删除用户](assets/remove-users-from-resource-pool.png)

   生产环境中的示例图像：
   ![在资源池中搜索](assets/search-inside-new-resource-pool-350x314.png)

1. 单击用户级别的“x”图标可从资源池中删除用户。 它们会从显示的所有列表中删除。\
   或\
   要删除与工作角色、组、团队或公司关联的所有用户，请在工作角色、组、团队级别或公司级别单击&#x200B;**删除**。 这将从资源池中删除与该工作角色、组、团队或公司关联的所有用户。

1. 单击&#x200B;**保存**。
