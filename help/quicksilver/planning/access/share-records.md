---
title: 共享记录
description: 您可以使用“共享”按钮共享记录，以便在Adobe Workfront Planning中提高协作能力。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# 共享记录

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以调整人员对记录类型中单个记录的权限。

您可以通过以下方式共享Adobe Workfront Planning记录：

* 共享记录链接。

  有关详细信息，请参阅[使用链接共享记录](/help/quicksilver/planning/records/share-records.md)。

* 通过共享工作区和记录类型，与其他用户共享工作区中的所有记录。

  有关更多信息，请参阅以下文章：

   * [共享工作区](/help/quicksilver/planning/access/share-workspaces.md)

   * [共享记录类型](/help/quicksilver/planning/access/share-record-types.md)

* 使用&#x200B;**共享**&#x200B;选项共享记录。

  本文介绍如何使用&#x200B;**共享**&#x200B;选项与他人共享记录。

>[!IMPORTANT]
>
>有权访问工作区的用户将自动获得对工作区中所有记录的至少“查看”权限。
>共享视图不会授予用户对记录的权限。 只有共享工作区才能授予用户记录类型和记录的权限。
>
>有关在Workfront Planning中共享对象的一般信息，另请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。


## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
   <td><p>任何</p> 
   <p><b>注释</b></p>
   <p>只有拥有Standard许可证的人员才能获得记录的管理权限。 所有其他许可证只能具有“查看”权限，并且它们的“管理”选项为灰色。</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
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

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享记录时的注意事项

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* 您可以与以下实体共享记录：人员、组、团队、公司或工作角色。
* 默认情况下，当您与用户共享工作区时，他们也将获得工作区中记录的相同权限。
* 从工作区中删除实体时，所有共享权限都将从记录类型及其中的所有记录中删除。
* 用户对该记录的访问权限通过以下3个设置的组合来确定：

   * 从记录类型和工作区继承的权限
   * 在记录共享对话框中单独添加的权限
   * 以下权限：

      * **工作区中的每个人都可以查看**：这将使工作区<!-- is this OK to say "workspace? should it be "record"??-->中的每个人都可以查看记录
      * **只有受邀人员才能访问**：默认情况下选中此选项，允许限制特定人员对记录的访问。

* 您可以向记录授予以下级别的权限：

   * 视图
   * 管理

* 与用户共享记录时，默认情况下会以与记录类型相同的权限添加用户。

  例如：

   * 如果他们具有记录类型的查看权限，他们将获得记录的查看权限
   * 如果他们拥有记录类型的Contribute或Manage权限，他们将获得该记录的Manage权限

* 作为工作区管理员，您可以与不属于工作区的用户共享记录。 在这种情况下，添加的实体旁边会显示一条警告，通知他们无权访问工作区。 您可以继续将用户添加到记录（该记录还会将用户添加到工作区），或停止将用户添加到记录（该记录不会将用户添加到工作区）。

* 当您与对工作区具有管理权限的用户共享记录时，他们也将默认获得该记录的管理权限。 “查看”权限将灰显。

* 如果您没有将人员添加到工作区的权限，您将只看到并添加已添加到工作区的用户、团队、组、角色和公司。 您无法添加尚未成为工作区一部分的任何其他实体。

* 您可以禁用单个记录的继承权限，在这种情况下，您可以授予他们针对单个记录的权限，或者，如果他们属于&#x200B;**工作区中的每个人都可以查看**&#x200B;选项，则他们可以获得权限。<!-- is this OK to say "workspace? should it be "record"??-->

* 如果同一用户申请了多个共享权限，他们将获得这些权限的最高权限。

  例如，如果记录与具有查看权限的用户共享，并且与具有管理访问权限的用户共享，则他们可获得该记录的管理权限。

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* 如果公式字段或来自已连接记录的查找字段基于您无权访问的记录上的字段，您将看到正确的计算，其中哪些是您无法访问记录的因素。

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## 共享记录权限

如果您具有工作区的管理权限，则可以调整单个记录的权限。

{{step1-to-planning}}

1. 打开要共享其记录的工作区。
1. 单击要共享其记录的记录类型。

1. 执行下列操作之一：

   * 在表视图中，将鼠标悬停在记录名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享**。
   * 从任何视图中，单击记录的名称，然后单击记录详细信息页面右上角的&#x200B;**共享**。

   将打开&#x200B;**共享**&#x200B;框。

   ![具有继承权限的记录的权限：](assets/permissions-for-records-with-inherited-permissions-on.png)

1. （可选）在&#x200B;**谁具有访问权限**&#x200B;区域中，默认情况下选中&#x200B;**工作区中的每个人都可以查看**&#x200B;选项。  所有对工作区和记录类型具有查看或更高权限的用户都可以查看记录。

1. （可选）单击&#x200B;**继承的权限**&#x200B;选项下的用户数，以查看从工作区继承权限的用户、团队、组、公司或工作角色。

   >[!TIP]
   >
   >您无法从继承的权限列表中删除单个实体。

1. （可选且视情况而定）如果要与特定实体共享记录类型，并授予他们与工作区已存在的记录类型不同的访问权限，请执行以下操作：

   1. 从&#x200B;**继承权限**&#x200B;下拉菜单中选择&#x200B;**禁用**。

   >[!TIP]
   >
   >Workspace管理员继续对记录类型和记录具有管理权限。

   1. （可选）选择&#x200B;**只有受邀人员才能从**&#x200B;谁有访问权限&#x200B;**区域访问**。

   1. 在&#x200B;**授予对此记录类型的访问权限**&#x200B;字段中，添加要授予不同于工作区或记录类型的权限级别的用户、团队、组、公司或工作角色。
   1. 选择以下权限级别之一：

      * 视图
      * 管理

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* 除了团队、组、公司和职位角色之外，您只能与已添加到Adobe Admin Console的用户共享。 您无法添加仅限Workfront的用户。 有关信息，请参阅[在Adobe Admin Console中管理用户](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)。
   >* 如果用户具有工作区和记录类型的“贡献”或“管理”权限，他们将保留记录的“管理”权限。 “查看”权限灰显
   >* 如果用户具有Contribute或更高权限，则无法授予用户较低的记录权限。
   > 有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

1. 要向没有工作区访问权限的用户授予查看记录的权限，请在&#x200B;**授予此视图**&#x200B;的访问权限字段中，开始键入用户、组、团队、公司或工作角色的名称，然后当该名称显示在列表中时单击它。

   您选择的实体已添加到记录和工作区，具有&#x200B;**查看**&#x200B;权限。

   系统管理员始终获得与他们共享的记录的管理权限，并且用户是系统管理员的指示。

1. （可选）单击&#x200B;**复制链接**&#x200B;以将指向记录的链接复制到剪贴板并与他人共享。 该链接将打开记录的详细信息页面。
1. 单击&#x200B;**保存**。

   现在，该记录已与其他用户共享。
   <!--Checking with Lilit on this: The users you shared the record with receive both an in-app and email notification about having given permissions to the following entities:

   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them. -->

1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问记录类型页面并在选定视图中显示该页面。 他们必须有权查看记录类型。 有关详细信息，另请参阅[使用链接共享记录](/help/quicksilver/planning/records/share-records.md)。

## 删除对记录的权限(**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;***&#x200B;这是从记录类型复制的，需要为记录编辑它，但等待LILIT的SLACK响应&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**)

您可以从记录中删除用户的权限。 但是，他们至少将保留对记录工作区的查看权限，这也会为他们提供对记录类型的至少查看权限。 如果您希望他们无权访问工作区中的记录类型，则必须从工作区中删除他们的访问权限。

{{step1-to-planning}}

1. 打开要停止共享其记录类型的工作区，然后单击记录类型信息卡。 这将打开记录类型页面。

1. 从任何视图的选项卡中，单击记录类型右上角的&#x200B;**共享**。
1. 单击&#x200B;**共享记录类型**。

   将打开&#x200B;**共享**&#x200B;框。
1. 查找要删除其权限的用户、组、团队、公司或工作角色，展开其名称右侧的权限下拉菜单，然后单击“**删除**”。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![删除记录类型共享下拉列表上的选项](assets/remove-option-on-record-type-sharing-drop-down.png)

1. 单击&#x200B;**保存**。

   人员不再具有对记录类型的指定权限。 但是，他们仍具有工作区的权限，除非您同时从工作区权限中删除他们。

   对于已从访问视图中删除的用户，不会通知他们不再具有此访问权限。
