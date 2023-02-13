---
product-area: user-management;portfolios
navigation-topic: grant-and-request-access-to-objects
title: 从对象删除权限
description: 您可以删除其他用户对您有权访问“共享”的对象的权限。 对于可共享的所有对象，从对象中删除权限是相同的。
author: Alina
feature: Get Started with Workfront
exl-id: 8e191b5e-31df-4291-8b9d-9ca69be27561
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '1076'
ht-degree: 0%

---

# 从对象删除权限

您可以删除其他用户对您有权访问“共享”的对象的权限。 对于可共享的所有对象，从对象中删除权限是相同的。 

与共享对象类似的注意事项也适用于从对象中删除权限。 有关更多信息，请参阅 [有关共享对象的注意事项](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#consider) 在文章中 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or  
   <p>Legacy license: Request or higher</p>
   <p><b>NOTE</b></p>

   <p>Some objects require a higher access than Request. </p>
   
   <p>For example, for the current license, a Contributor can share issues, but only Standard-license users can share a project.</p>
   
   <p>For the legacy license, a Requestor can share issues, but only Workers or Planners can share a project.</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you want to share</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions or higher to the objects you want to share</p> <p>Manage permissions to remove inherited permissions on objects</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront许可证*</td> 
   <td> <p>请求或更高版本</p>
   <p><b>注释</b></p>

某些对象需要比请求更高的访问权限。 例如，请求者可以共享问题，但只有工作人员或规划者才能共享项目。

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对要共享对象的访问权限或更高权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看您要共享的对象的权限或更高权限</p> <p>管理权限以删除对象的继承权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 从对象的共享列表中删除实体 {#remove-entities-from-the-sharing-list-of-an-object}

您可以从对象的共享列表中删除实体（用户、作业角色、团队、组、公司）。 这会删除他们对对象的权限。

1. 转到要共享的对象。

   有关哪些对象可以共享的信息，请参阅 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 单击 **更多** 图标 ![](assets/more-icon.png)在对象名称旁边，单击 **共享** 或&#x200B;**共享。**

   ![](assets/share-a-document-350x160.png)

1. 单击 **x** 用户、团队、组、公司、作业角色的名称旁边，以在对象访问框中删除这些角色。

   ![](assets/remove-permissions-on-project-nwe-350x479.png)

1. 在 `<User Name>`的Workfront访问权限将从此下拉菜单中删除，选择您希望仅从您选择的对象中删除其访问权限，还是从与其关联的所有子对象中删除。\
   存在以下情形：

   * 如果仅从对象中删除实体，则该实体将丢失其对该对象的权限，以及其对子对象的继承权限。 如果先前已单独授予子项目的权限，则当您选择此选项时，它们将保留与其关联的所有子对象的相同权限。 
   * 如果从对象和所有子对象中删除实体，则该实体将丢失其对对象和所有子对象的权限，即使先前已为每个子对象分别授予它们权限。 

1. 单击&#x200B;**保存**。

## 批量删除多个对象的权限

在列表中批量选择实体（用户、作业角色、团队、组、公司）时，您可以一次从多个对象中删除它们。 

>[!NOTE]
>
>批量选择所有选定对象时，您无法查看这些对象具有哪些访问实体。 在删除所选对象的权限之前，您必须知道要从共享所选对象中删除的实体。

1. 转到要共享的对象列表。

   有关哪些对象可以共享的信息，请参阅 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. 在列表中选择多个对象，然后单击 **共享** 图标 ![](assets/share-icon.png)列表顶部。
1. 键入要在中删除其访问权限的用户、角色、团队、组或公司的名称 **编辑 `<Object Name>` 访问** 字段。
1. 从访问下拉菜单中，选择 **无权访问**.

   ![](assets/no-access-option-removing-permissions-bulk-tasks-nwe-350x166.png)

1. 在 `<User Name>`的Workfront访问权限将从此下拉菜单中删除，选择您希望仅从您选择的对象中删除其访问权限，还是从与其关联的所有其他子对象中删除。\
   存在以下情形：

   * 如果仅从对象中删除实体，则该实体将丢失其对该对象的权限，以及其对子对象的继承权限。 如果先前已单独授予子项目的权限，则当您选择此选项时，它们将保留与其关联的所有子对象的相同权限。 
   * 如果从对象和所有子对象中删除实体，则该实体将丢失其对对象和所有子对象的权限，即使先前已为每个子对象分别授予它们权限。

   **示例：** 选择是仅删除您在列表中选择的任务的权限，还是删除附加到任务的问题和文档的权限。

   ![](assets/remove-permissions-bulk-drop-down-for-attached-objects-nwe-350x96.png)

1. （可选）要批量更改多个对象的权限，请为选定实体选择其他级别的共享。

   例如，如果用户具有“管理”权限，请选择“Contribute”或“查看”。

1. 单击&#x200B;**保存**。

## 删除继承的权限

可以从对象中删除继承的权限，以便所有者能够明确地识别谁将有权访问子对象，而不管用户是否有权访问父对象。

>[!IMPORTANT]
>
>只有具有“管理”权限的用户才能删除继承的权限。

要删除继承的权限，请执行以下操作：

1. 转到您具有“管理”权限的对象。 例如，转到任务。
1. 按照 [从对象的共享列表中删除实体](#remove-entities-from-the-sharing-list-of-an-object) 章节。
1. 选择 **x** 下一页 **继承权限** ，以删除该处列出的任何人。

   ![](assets/remove-inherited-permissions-on-project-nwe-350x475.png)

   这可确保在默认情况下，没有为父对象（例如项目）授予权限的人拥有此任务的权限。 必须在任务的共享列表中列出单个实体，才能授予任务的权限。

   >[!TIP]
   >
   >您无法从“继承的权限”列表中删除单个实体。 您只能禁用所有列出实体的“继承权限”。

1. 单击 **保存**. 

## 将对象设为私有对象

如果您在系统范围内共享了对象，或者通过将对象设为公用与外部用户共享了对象，则可以通过删除系统范围或公共权限将其再次设为私有。 

有关使对象在系统范围内或公开可用的详细信息，请参阅 [共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

将对象设为私有对象：

1. 转到要设为私有的对象。\
   例如，导航到报表。
1. 单击 **报表操作**，则 **共享**.

   ![](assets/report-permissions-make-private-nwe-350x477.png)

1. 单击 **删除公共访问权限** 删除外部用户查看报表的权限。
1. 单击 **删除系统范围的访问** 停止与所有Workfront用户共享。 
1. 单击&#x200B;**保存**。
