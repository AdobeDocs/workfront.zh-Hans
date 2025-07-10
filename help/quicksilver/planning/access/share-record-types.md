---
title: 共享记录类型
description: 在使用Adobe Workfront Planning时，您可以与其他人共享记录类型以确保协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 4fafdcea97874e791104260375617e3989af1870
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# 共享记录类型

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

在Adobe Workfront Planning中处理记录时，您可以与其他人共享记录类型以确保协作。

>[!IMPORTANT]
>
>有权访问工作区的用户将自动获得对工作区中所有记录类型的至少“查看”权限。
>>共享视图不授予用户记录类型的权限。 只有共享工作区才能授予用户记录类型的权限。
>
>* 有关在Workfront Planning中共享对象的一般信息，另请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。
>* 有关详细信息，请参阅本文中的[共享记录类型时的注意事项](#considerations-when-sharing-record-types)部分。

## 访问要求

+++ 展开以查看访问要求。

<!--at GA, check that the Workfront plans article linked below has Planning info-->

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>必须将用户添加到Adobe Admin Console才能获得Workfront Planning视图的权限。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  <p>管理记录类型的权限</p>  
   <p>只有对工作区具有管理权限的用户才能共享对记录类型的管理权限</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>版面模板</p></td> 
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning区域的布局模板。</p>
<p><span class="preview">在预览环境中，标准用户和系统管理员默认启用Planning区域。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享记录类型时的注意事项

* 默认情况下，向工作区授予权限会向用户提供工作区中记录类型的相同权限。

  此外，您可以调整单个记录类型的权限。

  但是，您不能向人员授予比他们对工作区具有的权限更高的记录类型权限。
* 您可以授予用户比他们在工作区中拥有更低的记录类型权限。 例如，他们可以拥有工作区的“贡献”权限，以及记录类型的“查看”权限。
* 具有工作区的“管理”权限的用户始终保持对工作区中所有记录类型的“管理”访问权限。 无法降低其对记录类型的权限，即使已关闭继承权限也是如此。

* 目前，当您共享记录类型时，可以实现以下目标：

   * 当您首次与用户共享记录类型并且他们没有任何工作区权限时，向用户提供工作区的查看权限。

     这还为他们提供了对工作区中所有记录类型的查看权限。

     授予他们记录类型的权限时，共享框中会显示已添加到工作区的权限。
   * 禁用“继承权限”后，使记录类型仅对工作区中的每个人（工作区管理员除外）可见。

     具有工作区的“管理”权限的用户始终对记录类型具有“管理”权限，即使您关闭记录类型的“继承”权限也是如此。
   * 降低人们对记录类型的权限。 您无法根据某人在工作区中的权限来增加其对记录类型的权限。

     例如，如果某人拥有工作区的“Contribute”权限，则您可以将其权限更改为要查看的特定记录类型。 但是，如果他们具有工作区的查看权限，则无法向他们授予对任何记录类型的Contribute权限。

* 无法删除工作区中人员的记录类型的访问权限。 如果每个人都至少拥有工作区的查看权限，则每个人都至少对所有记录类型具有查看权限。

* 您可以在内部与以下实体共享记录类型：

  Workfront用户、组、团队、公司和职位角色
* 您无法与Workfront之外的用户从外部共享记录类型。
* 要向没有工作区权限高于查看权限的用户授予记录类型的权限，您必须首先以高于查看的权限与他们共享工作区。 工作区的较高权限随后将应用于记录类型。

## 共享记录类型的权限

如果您具有工作区的管理权限，则可以调整对工作区的各个记录类型的权限。

{{step1-to-planning}}

1. 打开要共享其记录类型的工作区，然后单击记录类型卡片。

   这将打开记录类型页面。

1. 从任何视图的选项卡中，单击记录类型右上角的&#x200B;**共享**。
1. <span class="preview">单击&#x200B;**共享记录类型**。</span>

   将打开&#x200B;**共享**&#x200B;框。

   ![具有继承权限的记录类型的权限：](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. （可选）在&#x200B;**谁具有访问权限**&#x200B;区域中，默认情况下选中&#x200B;**工作区中的每个人都可以查看**&#x200B;选项。  所有对工作区具有“查看”或更高权限的用户都可以查看记录类型。

1. （可选）单击&#x200B;**继承的权限**&#x200B;选项下的用户数，以查看从工作区继承权限的用户、团队、组、公司或工作角色。

   >[!TIP]
   >
   >您无法从继承的权限列表中删除单个实体。


1. （可选且视情况而定）如果要与特定实体共享记录类型，并授予他们与工作区已存在的记录类型不同的访问权限，请执行以下操作：

   1. 从&#x200B;**继承权限**&#x200B;下拉菜单中选择&#x200B;**禁用**。

   >[!TIP]
   >
   >Workspace管理员继续拥有记录类型的管理权限。

   1. 在&#x200B;**授予对此记录类型的访问权限**&#x200B;字段中，添加要授予不同于工作区权限级别的用户、团队、组、公司或工作角色。
   1. 选择权限级别。

   >[!IMPORTANT]
   >
   >* 除了团队、组、公司和职位角色之外，您只能与已添加到Adobe Admin Console的用户共享。
   >* 您永远不能授予用户在记录类型上比他们在工作区上更大的权限。
   >* 您不能授予比“管理”更小的用户记录类型权限（如果他们具有工作区的管理权限）。
   >* 如果用户具有工作区的“贡献”权限，则可以授予他们较少的记录类型权限。
   > 有关详细信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

1. 要向没有工作区访问权限的用户授予查看记录类型的权限，请在&#x200B;**授予此视图的访问权限**&#x200B;字段中，开始键入用户、组、团队、公司或工作角色的名称，然后当该名称显示在列表中时单击它。

   您选择的实体已添加到记录类型中，并添加到具有&#x200B;**查看**&#x200B;权限的工作区。

   系统管理员始终获得记录与其共享的类型的管理权限，并且有迹象表明用户是系统管理员。

1. （可选）单击&#x200B;**复制链接**&#x200B;以将指向记录类型的链接复制到剪贴板并与他人共享。
1. 单击&#x200B;**保存**。

   记录类型现在已与其他用户共享。

1. 与他人共享复制的链接。 接收链接的用户必须是活动用户并登录到Workfront才能访问记录类型页面并在选定视图中显示该页面。 他们必须有权查看记录类型。

## 删除对记录类型的权限

您可以从记录类型中删除用户的权限。 但是，他们至少将保留对工作区的查看权限，这也会为他们提供对记录类型的查看权限。 如果您希望他们无权访问工作区中的记录类型，则必须从工作区中删除他们的访问权限。

{{step1-to-planning}}

1. 打开要停止共享其记录类型的工作区，然后单击记录类型信息卡。 这将打开记录类型页面。

1. 从任何视图的选项卡中，单击记录类型右上角的&#x200B;**共享**。
1. <span class="preview">单击&#x200B;**共享记录类型**。</span>

   将打开&#x200B;**共享**&#x200B;框。
1. 查找要删除其权限的用户、组、团队、公司或工作角色，展开其名称右侧的权限下拉菜单，然后单击“**删除**”。<!--check the screen shot below - the UI text for View might not be accurate-->

   ![删除记录类型共享下拉列表上的选项](assets/remove-option-on-record-type-sharing-drop-down.png)

1. 单击&#x200B;**保存**。

   人员不再具有对记录类型的指定权限。 但是，他们仍具有工作区的权限，除非您同时从工作区权限中删除他们。

   对于已从访问视图中删除的用户，不会通知他们不再具有此访问权限。

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

