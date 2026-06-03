---
title: 共享记录
description: 您可以使用“共享”按钮共享记录，以便在Adobe Workfront Planning中提高协作能力。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 9ffad1aa-3c96-40fa-9c62-7a3e00699f18
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/NTytTWD-zq3PVhXn4n-GHinvQxna1wfnAXjaeYBgTEY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: c33c023ab33a3b0c8369e6fae091d0ec877aa4e2
workflow-type: tm+mt
source-wordcount: 1720
ht-degree: 2%

---

<!--update metadata with real information at release-->

# 共享记录

<!--
this will NOT be available in Preview ever - find a way to add this in this article that is prominent
-->

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>\
<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以在Adobe Workfront Planning中调整人员对记录类型中单个记录的权限。

您可以通过以下方式共享Adobe Workfront Planning记录：

* 共享记录链接。

  有关详细信息，请参阅[使用链接共享记录](/help/quicksilver/planning/records/share-records.md)。

* 通过共享工作区和记录类型，与其他用户共享工作区中的所有记录。

  有关更多信息，请参阅以下文章：

   * [共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

   * [共享记录类型](/help/quicksilver/planning/access/share-record-types.md)

* 使用&#x200B;**共享**&#x200B;选项共享单个记录或批量共享多个记录。

  本文介绍如何使用&#x200B;**共享**&#x200B;选项与他人共享记录。

>[!IMPORTANT]
>
>* 有权访问工作区的用户将自动获得对工作区中所有记录的至少“查看”权限。
>* 共享视图不会授予用户对记录的权限。 只有共享工作区才能授予用户记录类型和记录的权限。
>
>有关在Workfront Planning中共享对象的一般信息，另请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>任何Workfront和Planning包</p> 
或
<p>任何工作流和计划包</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>“任一”</p> 
   <p><b>注释</b></p>
   <p>只有拥有Standard许可证的人员才能获得记录的管理权限。 所有其他许可证只能具有“查看”权限，并且它们的“管理”选项为灰色。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  <p>管理对工作区、记录类型和记录的权限</p>  
   <p><b>重要</b></p>
   <p>只有对工作区具有管理权限的用户才能共享记录</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> 必须为具有轻度或参与者许可证的用户分配一个包括Planning的布局模板。
   <p>默认情况下，标准用户和系统管理员已启用Planning区域。</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享记录时的注意事项

<!--
maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information
-->

<!--checking on the below with Lilit-->

* 您可以与以下实体共享记录：人员、组、团队、公司或工作角色。
* 如果限制对记录的权限，则用户将不能再查看该记录以及该记录所在系统中任何位置的查找字段值。
* Workfront检查连接中的记录权限，最多深层检查5条记录，确保用户只能看到与其共享的记录。
* 您可以向记录授予以下级别的权限：

   * 视图
   * 管理
* 当用户共享工作区和记录类型时，默认情况下，他们也会获得工作区中记录的相同权限。
当用户具有工作区或记录类型的Contribute权限时，他们将获得该记录类型的记录的管理权限。
* 从工作区中删除实体时，所有共享权限都将从记录类型及其中的所有记录中删除。
* 您无法与没有工作区或记录类型权限的用户共享记录。

  如果您与不在工作区中的用户共享记录，则这些用户会自动添加到工作区中。
* 用户对该记录的访问权限通过以下3个设置的组合来确定：

   * 从记录类型和工作区继承的权限
   * 在记录共享框中单独添加的权限
   * 工作区中的&#x200B;**每个人都可以查看**&#x200B;设置。

     这使工作区中的每个用户都可以查看记录

     <!--
      Cannot do this on a record: 
      * **Only invited people can access**: This is selected by default and allows restricting access to the record to specific people. 
      -->

* 与用户共享记录时，默认情况下会以与记录类型相同的权限添加用户。

  例如：

   * 如果他们具有记录类型的查看权限，他们将获得记录的查看权限
   * 如果他们拥有记录类型的Contribute或Manage权限，他们将获得该记录的Manage权限

* 当用户对工作区和记录类型具有“管理”或“贡献”权限，并且您将其添加到记录权限时，“查看”权限将灰显。 他们保留对记录的相同权限，就像对记录类型一样，您不能为他们授予较低的记录权限。

* 您可以禁用单个记录的继承权限，在这种情况下，您可以向选定的用户授予对单个记录的权限，或者，如果他们属于工作区，则他们也可以获得权限，因为&#x200B;**工作区中的每个人都可以查看**&#x200B;选项。

* 如果同一用户申请了多个共享权限，他们将获得最高级别的这些权限。

  例如，如果记录与具有“查看”权限的用户共享，并且与具有“管理”访问权限的用户共享，则他们将获得该记录的“管理”权限。

* 如果公式字段或来自已连接记录的查找字段基于您无权访问的记录上的字段，您将看到正确的计算，其中哪些是您无法访问记录的因素。

  <!--
   Not possible: 
   * As a workspace manager, you can share a record with a user that does not have permissions to the record type or the workspace. In this case, there is a warning next to the added entity notifying you that they don't have access to the workspace or the record type.  You can continue adding the user to the record which will also add them to the record type and workspace, or cancel the sharing.
   -->

  <!--
   ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too
   -->

<!--
Lilit is checking on this, it is not working correctly
-->

<!--
   check on this: I cannot disable inherited permissions when this setting is ON and this documented in a TIP below: When they have View permissions to the workspace or the record type, they retain View permissions to the records. You can grant them Manage permissions to the record by disabling Inherited permissions and selecting the Only invited people can access setting.
   -->

<!-- 
   not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.
   -->

<!--
   Too granular??
   If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 
   If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions 
   -->

<!--
   not sure if any of the Share record types points might match here - ask Lilit??
   -->

## 共享记录

作为工作区管理员，您可以调整单个记录的权限。

{{step1-to-planning}}

1. 打开工作区，然后打开要共享其记录的记录类型。

1. 执行下列操作之一：

   * 在表视图中，将鼠标悬停在记录名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享**。
   * 从表格视图中，选择一个或多个记录，然后单击列表底部蓝色工具栏上的&#x200B;**共享**。
   * 从任何视图中，单击记录的名称，然后单击记录详细信息页面右上角的&#x200B;**共享**。

   将打开&#x200B;**共享**&#x200B;框。

   ![具有继承权限的记录的权限：](assets/permissions-for-records-with-inherited-permissions-on.png)

   >[!WARNING]
   >
   >您无法共享添加到不同工作区中的记录的权限。 批量共享记录时，必须在同一工作区中创建所有记录。

1. （可选）在&#x200B;**谁具有访问权限**&#x200B;区域中，默认情况下选中&#x200B;**工作区中的每个人都可以查看**&#x200B;选项。  对工作区和记录类型具有&#x200B;**查看**&#x200B;或更高权限的所有用户对该记录具有相同的权限。

1. （可选）单击&#x200B;**从**&#x200B;继承的权限选项下的用户头像，以查看从工作区继承权限的用户、团队、组、公司或工作角色。<!--logged bug to move "Permissions" to lowercase-->

   展开继承的权限时，将显示用户对记录类型的权限。

   >[!TIP]
   >
   >您无法从继承的权限列表中删除单个实体。 列出来自团队、组、公司或工作角色的用户，而不是与他们共享工作区和记录类型时他们关联的实体。

1. （可选且视情况而定）如果要与特定实体共享记录，并授予他们与工作区已存在的记录类型不同的访问权限，请执行以下操作：

   1. 从&#x200B;**继承权限**&#x200B;中取消选择&#x200B;**启用**&#x200B;选项。 默认情况下，该复选框处于选中状态。

      选项更改为&#x200B;**关闭**。

      >[!TIP]
      >
      >Workspace管理人员和记录创建者继续拥有对记录类型和记录的管理权限。

      <!-- 
      This is no longer possible for a record: 
      (Optional) Select **Only invited people can access** from the **Who has access** area. You must indicate individual users, groups, teams, or companies to share the records with. 
      >[!TIP]
      >
      >You cannot disable or enable Inherited permissions when this setting is selected.
      -->

   1. 在&#x200B;**授予对此记录的访问权限**&#x200B;字段中，添加要授予不同于工作区或记录类型的权限级别的用户、团队、组、公司或工作角色。

      与用户共享记录时，其主要工作角色和电子邮件也会显示在字段中。 您必须为访问级别中的“用户”对象启用“查看联系信息”设置，才能查看用户的电子邮件。

   1. 选择以下权限级别之一：

      * 视图
      * 管理

      >[!IMPORTANT]
      >
      >* 如果用户具有工作区和记录类型的“贡献”或“管理”权限，您可以为他们授予记录的“管理”权限。 “查看”权限将灰显。
      >* 如果用户拥有记录类型的Contribute或更高权限，则无法授予用户较低的记录权限。
      >有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
      >* 您无法向不在工作区中的用户授予权限。 无权访问工作区和记录类型的用户无法访问任何记录。

   <!--   
   Not possible:
   1. To give users who do not have permissions to the workspace access to view a record, in the **Grant access to this view** field, start typing the name of a user, a group, team, company, or job role, then click it when it displays in the list. 
      The entity you selected is added to the record and also to the record type and the workspace with **View** permissions. 
      System administrators always receive Manage permissions to records shared with them, and there is an indication that a user is a System administrator.
   -->

1. （可选）单击&#x200B;**复制链接**&#x200B;以将指向记录的链接复制到剪贴板并与他人共享。 该链接将打开记录的详细信息页面。
1. 单击&#x200B;**保存**。

   现在，该记录已与其他用户共享。

   您与其共享记录的用户会收到有关已获得记录权限的应用程序内通知和电子邮件通知。

   <!--
   not possible anymore: 
   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them.
   -->

   有关信息，请参阅[Adobe Workfront计划通知：文章索引](/help/quicksilver/planning/notifications/notifications-information.md)。


1. （可选）将复制的链接与其他人共享。

   接收链接的用户必须是活动用户并登录到Workfront才能访问记录类型页面并在选定视图中显示该页面。

   他们必须有权查看记录类型。

   有关详细信息，另请参阅[使用链接共享记录](/help/quicksilver/planning/records/share-records.md)。


## 删除记录的权限

您可以从记录中删除用户的权限。 但是，他们至少将保留对工作区的查看权限，这也会为他们提供对记录类型的查看权限。

如果您希望他们无权访问工作区中的记录类型或记录，则必须从工作区中删除他们的访问权限。

您无法从继承的权限中删除用户。

{{step1-to-planning}}

1. 打开要停止共享其记录的工作区，然后单击记录类型卡。 这将打开记录类型页面。
1. 执行下列操作之一：

   * 在表视图中，将鼠标悬停在记录名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享**。
   * 从表格视图中，选择一个或多个记录，然后单击列表底部蓝色工具栏上的&#x200B;**共享**。

     您必须选择在同一工作区中创建的记录。
   * 从任何视图中，单击记录的名称，然后单击记录详细信息页面右上角的&#x200B;**共享**。

   将打开&#x200B;**共享**&#x200B;框。
1. 查找要删除其权限的用户、组、团队、公司或工作角色，展开其名称右侧的权限下拉菜单，然后单击&#x200B;**删除**。

   ![删除记录权限](assets/remove-option-on-record-sharing-drop-down.png)

1. 单击&#x200B;**保存**。

   用户不再具有指定的记录权限。 但是，除非您还从这些权限中移除记录类型和工作区，否则他们仍有权访问这些记录类型和工作区。

   对于已从访问记录中删除的用户，不会通知他们不再具有这些权限。
