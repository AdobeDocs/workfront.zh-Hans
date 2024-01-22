---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 从对象中删除权限
description: 您可以删除其他用户对您有权共享的对象拥有的权限。 从对象中删除权限对于所有可共享的对象都是相同的。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 0%

---

# 从对象中删除权限

<!--Audited: 01/2024-->

您可以删除其他用户对您有权共享的对象拥有的权限。 从对象中删除权限对于所有可共享的对象都是相同的。

与共享对象类似的注意事项适用于从对象中删除权限。 有关更多信息，请参阅部分 [有关共享对象的注意事项](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) 在文章中 [对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## 访问要求

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

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。 有关更多信息，请参阅 [Workfront文档的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 从对象的共享列表中删除实体 {#remove-entities-from-the-sharing-list-of-an-object}

您可以从对象的共享列表中删除实体（用户、工作角色、团队、组、公司）。 这将删除他们对对象的权限。

1. 转到要删除权限的对象。

   有关哪些对象可以共享的信息，请参见 [对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. （视情况而定）对于项目、项目组合和文档，执行以下操作：

   1. 单击 **更多** 图标 ![](assets/more-icon.png)单击对象名称旁边的，然后单击 **共享** 或 **共享。**

      ![](assets/share-a-document-350x160.png)

   1. 单击 **x** 在对象访问框中，在用户、团队、组、公司、工作角色的名称旁移除它们。

      ![](assets/remove-permissions-on-portfolio.png)

   1. 在 **&lt;用户名>的Workfront访问权限将从此删除** 下拉菜单中，选择是希望仅从所选对象中删除其访问权限，还是从与其关联的所有子对象中删除其访问权限。

1. （视情况而定）对于项目、任务和问题，执行以下操作：

   1. 单击 **共享** 对象名称的右侧。

      ![](assets/new-share-button.png)
   1. 查找要从对象中移除的用户、角色、团队、组或公司。
   1. 单击 **移除**.
在 **从删除&lt;用户名>** 下拉菜单中，选择是希望仅从所选对象中删除其访问权限，还是从与其关联的所有子对象中删除其访问权限。

      ![](assets/remove-permissions-on-project-nwe-350x479.png)

   存在以下情况：

   * 如果仅从对象中删除实体，则该实体会丢失其对对象的权限以及其对子对象的继承权限。 如果先前已单独向他们授予了子项目的权限，则在选择此选项时，他们将保留与它关联的所有子对象的相同权限。
   * 如果从对象和所有子对象中移除实体，则该实体会丢失其对该对象以及所有子对象的权限，即使先前已授予了他们对每个子对象的单独权限。

1. 单击&#x200B;**保存**。

## 批量删除多个对象的权限

在列表中批量选择实体时，一次可以从多个对象中删除这些实体（用户、工作角色、团队、组、公司）。

>[!NOTE]
>
>当您批量选择所选对象时，无法查看这些对象具有何种访问实体。 在删除所选对象的权限之前，必须知道要从共享中移除哪个实体。

1. 转到要共享的对象列表。

   有关哪些对象可以共享的信息，请参见 [对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 在列表中选择多个对象，然后单击 **共享** 图标 ![](assets/share-icon.png)位于列表顶部。
1. 在中键入要删除其访问权限的用户、角色、团队、组或公司的名称 **编辑 `<Object Name>` 访问** 字段。
1. 从访问下拉菜单中，选择 **无权访问**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. 在 `<User Name>`的Workfront访问权限将从此下拉菜单中删除，请选择是希望仅从所选对象中删除其访问权限，还是从与其关联的所有其他子对象中删除其访问权限。\
   存在以下情况：

   * 如果仅从对象中删除实体，则该实体会丢失其对对象的权限以及其对子对象的继承权限。 如果先前已单独向他们授予了子项目的权限，则在选择此选项时，他们将保留与它关联的所有子对象的相同权限。 
   * 如果从对象和所有子对象中移除实体，则该实体会丢失其对该对象以及所有子对象的权限，即使先前已授予了他们对每个子对象的单独权限。

   **示例：** 选择是仅删除您在列表中选择的任务还是删除附加到任务的问题和文档的权限。

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. （可选）要批量更改多个对象的权限，请为所选实体选择另一个共享级别。

   例如，如果他们具有管理权限，请改为选择Contribute或View。

1. 单击&#x200B;**保存**。

## 删除继承的权限

继承的权限可以从对象中删除，这样所有者就可以明确标识谁将获得对子对象的访问权限，而不管用户是否有权访问父对象。

>[!IMPORTANT]
>
>只有具有“管理”权限的用户才能删除继承的权限。

要删除继承的权限，请执行以下操作：

1. 转到您拥有管理权限的对象。 例如，转到任务。
1. 转至对象访问框，如 [从对象的共享列表中删除实体](#remove-entities-from-the-sharing-list-of-an-object) 部分。
1. 选择 **x** 旁边 **继承权限** ，以移除该处列出的所有用户。

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   这可确保向父对象（例如项目）授予权限的任何人都不会默认拥有此任务的权限。 您必须在任务的共享列表中列出单个实体，以授予对任务的权限。

   >[!TIP]
   >
   >您无法从继承的权限列表中删除单个实体。 您只能对列出的所有实体禁用继承权限。

1. 单击 **保存**. 

## 将对象设为私有

如果已在系统范围内共享对象，或者已通过将对象设为公共对象与外部用户共享对象，则可以通过删除系统范围或公共权限来再次将其设为私有对象。 

有关使对象在系统范围内或公开可用的详细信息，请参见 [共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

要将对象设为私有：

1. 转到要设为私有的对象。\
   例如，导航到报表。
1. 单击 **报表操作**，则 **共享**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. 单击 **删除公开访问权限** 删除外部用户查看报告的权限。
1. 单击 **删除系统范围访问权限** 以停止与所有Workfront用户共享。 
1. 单击&#x200B;**保存**。
