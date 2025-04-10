---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 从对象中删除权限
description: 您可以删除其他用户对您有权共享的对象拥有的权限。 从对象中删除权限对于所有可共享的对象都是相同的。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: ce7b475dbd11f9cfd7fcf9879c0f34bf993f9113
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# 从对象中删除权限

<!--Audited: 01/2024-->

您可以删除其他用户对您有权共享的对象拥有的权限。 从对象中删除权限对于所有可共享的对象都是相同的。

与共享对象类似的注意事项适用于从对象中删除权限。 有关详细信息，请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)一文中的[有关共享对象的注意事项](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider)部分

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。


要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront许可证*</td> 
   <td> <p>新许可证：参与者或更高版本</p>
   或  
   <p>当前许可证：请求或更高版本</p>
   <p><b>注释</b></p>

<p>某些对象需要比请求更高的访问权限。 </p>

<p>例如，对于新许可证，参与者可以共享问题，但只有Standard许可证用户可以共享项目。</p>

<p>对于当前许可证，请求者可以共享问题，但只有工作人员或规划人员可以共享项目。</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对要共享对象的访问权限或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看要共享对象的权限或更高</p> <p>管理权限以移除对对象的继承权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关详细信息，请参阅Workfront文档的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从对象的共享列表中删除实体 {#remove-entities-from-the-sharing-list-of-an-object}

您可以从对象的共享列表中删除实体（用户、工作角色、团队、组、公司）。 这将删除他们对对象的权限。

1. 转到要删除权限的对象。

   有关哪些对象可以共享的信息，请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

1. （视情况而定）对于项目、项目组合和文档，执行以下操作：

   1. 单击对象名称旁边的&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**共享**&#x200B;或&#x200B;**共享。**

      ![共享](assets/share-a-document-350x160.png)

   1. 单击用户、团队、组、公司、工作角色名称旁边的&#x200B;**x**，在对象访问框中将其删除。

      ![删除权限](assets/remove-permissions-on-portfolio.png)

   1. 在&#x200B;**[用户名]的Workfront访问权限将从此**&#x200B;下拉菜单中移除，选择是希望从所选对象中移除其访问权限，还是从与其关联的所有子对象中移除其访问权限。

1. （视情况而定）对于项目、任务和问题，执行以下操作：

   1. 单击对象名称右侧的&#x200B;**共享**。

      ![共享](assets/new-share-button.png)
   1. 查找要从对象中移除的用户、角色、团队、组或公司。
   1. 单击&#x200B;**删除**。
在**从**&#x200B;中删除&lt;用户名>下拉菜单中，选择是希望从所选对象中删除其访问权限，还是从与其关联的所有子对象中删除其访问权限。

      ![移除](assets/remove-permissions-on-project-nwe-350x479.png)

   存在以下情况：

   * 如果仅从对象中删除实体，则该实体会丢失其对对象的权限以及其对子对象的继承权限。 如果先前已单独向他们授予了子项目的权限，则在选择此选项时，他们将保留与它关联的所有子对象的相同权限。
   * 如果从对象和所有子对象中移除实体，则该实体会丢失其对该对象以及所有子对象的权限，即使先前已授予了他们对每个子对象的单独权限。

1. 单击&#x200B;**保存**。

<!--
## Remove permissions from several objects in bulk

You can remove entities (users, job roles, teams, groups, companies) from several objects at a time when you bulk select them in a list.

>[!NOTE]
>
>You cannot view what access entities have for all the objects selected when you select them in bulk. You must know which entity you want to remove from the sharing of the objects selected before removing their permissions.

1. Go to the list of objects that you want to share.

   For information about which objects can be shared, see [Overview of sharing permissions on objects](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Select several objects in the list, then click the **Share** icon ![share icon](assets/share-icon.png)at the top of the list. 
1. Type the name of the user, role, team, group, or company for which you want to remove the access in the **Edit `<Object Name>` access to** field. 
1. From the access drop-down menu, select **No Access**.

   ![remove in bulk](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. In the `<User Name>`'s Workfront access will be removed from this drop-down menu, select whether you want their access to be removed just from the objects that you have selected, or from all other children objects associated with it.  
   The following scenarios exist:

   * If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they were previously granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;
   * If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they were previously given individual permission on each child object.

   **Example:** Select whether to remove permissions to just the tasks you selected in a list, or to the issues and documents attached to the tasks as well.

   ![access](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. (Optional) To change permissions in bulk for several objects, select another level of sharing for the selected entity.

   For example, if they have Manage permissions, select Contribute or View instead. 

1. Click **Save**.

-->

## 删除继承的权限

继承的权限可以从对象中删除，这样所有者就可以明确标识谁将获得对子对象的访问权限，而不管用户是否有权访问父对象。

>[!IMPORTANT]
>
>只有具有“管理”权限的用户才能删除继承的权限。

要删除继承的权限，请执行以下操作：

1. 转到您拥有管理权限的对象。 例如，转到任务。
1. 按照本文中[从对象](#remove-entities-from-the-sharing-list-of-an-object)的共享列表中删除实体一节中的说明转到对象访问框。
1. 选择要禁用的&#x200B;**继承权限**&#x200B;旁边的&#x200B;**关闭**。

   这可确保向父对象（例如项目）授予权限的任何人都不会默认拥有此任务的权限。 您必须在任务的共享列表中列出单个实体，以授予对任务的权限。

   >[!TIP]
   >
   >您无法从继承的权限列表中删除单个实体。 您只能对列出的所有实体禁用继承权限。

1. 单击&#x200B;**保存**。 

## 将对象设为私有

如果已在系统范围内共享对象，或者已通过将对象设为公共对象与外部用户共享对象，则可以通过删除系统范围或公共权限来再次将其设为私有对象。 

有关使对象在系统范围内或公开可用的详细信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

要将对象设为私有：

1. 转到要设为私有的对象。\
   例如，导航到报表。
1. 单击&#x200B;**报告操作**，然后单击&#x200B;**共享**。

   ![设为私有](assets/report-permissions-make-private-nwe-350x477.png)

1. 单击齿轮图标，然后取消选中&#x200B;**将此设为外部用户公开**。
1. 在&#x200B;**拥有访问权限**&#x200B;下拉菜单中，单击&#x200B;**只有受邀人员才能访问**，以停止与所有Workfront用户共享它。
1. 单击&#x200B;**保存**。
