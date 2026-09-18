---
title: 共享Workfront规划字段
description: 您可以与其他人共享Workfront Planning记录的字段，以确保在使用Adobe Workfront Planning时进行协作。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b529b3aded4ab92015683a0ddccd152bc2cc798c
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 2%
---

# 共享Workfront规划字段

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

您可以与其他人共享Workfront Planning记录的字段，以确保在使用Adobe Workfront Planning时进行协作。

字段共享让工作区管理员能够控制对单个字段的访问。 记录类型中的每个字段都有自己的共享对话框，其中访问权限可以设置为无权访问、查看字段值或管理字段值。

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
<p>带规划包的任何Workfront或工作流</p> 
或
<p>任何Workfront Planning作为独立产品包</p> 
 </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>“任一”</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>“任一”</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>当您同时具有Workflow和Planning包时，必须将工作流和Planning许可证类型添加到访问级别</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>管理字段的权限以更改字段值</p>  
   <p>向记录类型分配或更高权限以继承字段的管理权限</p>  
   </td> 
  </tr>
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关共享字段的注意事项

* 您可以与用户、工作角色、组、团队或公司共享字段。
* 您只能共享记录类型表格视图中的字段。
* 您无法共享以下类型的字段：

  * 系统字段（例如，创建者、记录ID）
  * 主要字段
  * 查找字段。 它们始终继承其源对象字段的权限。
* 对字段的访问权限来自组合以下设置：

  * **继承权限**：默认情况下，字段继承某人对该记录类型的相同访问权限。 您可以关闭继承权限，并授予用户比记录类型更低的字段访问权限。
  * 工作区中的&#x200B;**每个人都可以查看**&#x200B;或&#x200B;**只有受邀人员才能访问**&#x200B;选择。 您可以允许拥有工作区权限的每个人查看该字段，也可以仅向单个实体授予权限。

  如果同一人适用多个规则，则他们会从其中一个规则中获取可用的最高权限。

* 根据记录类型权限，用户可以获得以下字段权限：

  * 查看记录类型权限授予用户查看字段值的权限
  * Contribute或Manage记录类型权限授予用户管理字段值的权限

* 只有工作区所有者和管理员可以调整字段权限。 Workspace管理器始终保留对所有字段的管理访问权限，且无法降低。
* 字段共享控制对值的访问，而不是字段设置。 只有工作区管理员才能更改字段的配置。
* 将某人添加到字段的共享列表不会授予他们工作区或记录类型访问权限。 如果他们缺少该访问权限，则会显示一个警告图标，指示权限仅在他们被添加到记录类型后才会生效。
* 具有受限权限的字段会在字段显示位置强制执行。 这包括所有视图、记录详细信息页面、请求表单、连接和查找字段、画布功能板、API和MCP工具。
* 任何能够访问公共视图的人都可以完全查看和只读公共视图。
  <!--Not sure if this is right - right now, it allows me to duplicate with the values in the new record - checking with Lilit: * When you duplicate a record, the restricted values are not copied to the new records.-->
* 受限制的字段值更改不会记录在记录的历史记录中。
* 字段的权限更改不会触发通知。
* 对于全局记录类型，字段权限适用于所有辅助工作区，并且无法本地调整。

<!--
From Claude: 
Additional permissions for fields - maybe add this to the Overview article for all of the sharing?? - help/quicksilver/planning/access/sharing-permissions-overview.md 

Here's how record type / workspace access maps to field-level access in the document:

Field permission levels (only two, plus none):

No Access – field is completely hidden
View field values – can see the value, can't edit
Manage field values – can view and edit

Default inheritance from record type role

Record type / workspace access    Default field permission
View    View field values
Contribute    Manage field values
Manage (workspace manager)    Manage field values (locked — cannot be reduced)

So by default, a field simply mirrors whatever role someone has on the record type — Viewers get read-only, Contributors and Managers get edit rights. Workspace managers are a special case: whenever they're added to a field's sharing list, "Manage field values" is pre-selected and the "View field values" option is disabled, since their edit access can never be taken away.

Wildcard (fallback) setting
Separate from inheritance, each field has a wildcard default:

Everyone in the workspace can view (default)
Only invited people can access

How the final permission is calculated

If inherited permissions are enabled: a person's access = the highest of (inherited from record type, wildcard, individually granted permission).
If inherited permissions are disabled: a person's access = the highest of (wildcard, individually granted permission) — record type role no longer factors in.
If inheritance is disabled, wildcard is "Only invited people can access," and the person isn't individually added → they get No Access.

Other permission notes

Individually granting access to someone doesn't grant them workspace/record-type access — it just sits inactive (with a warning icon) until they're separately added to the workspace.
For Global Record Types, field permissions are set once and apply to all secondary workspaces; secondary/team workspace managers cannot override them locally.

-->

## 共享字段

作为工作区管理员，您可以调整各个字段的权限。

{{step1-to-planning}}

1. 打开工作区，然后打开要共享其字段的记录类型。

1. 在表视图中，将鼠标悬停在字段列标题的名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享字段**。

   将打开&#x200B;**共享**&#x200B;框。

1. （可选）在&#x200B;**授予访问权限**&#x200B;区域，默认情况下选中&#x200B;**工作区中的每个人都可以查看**&#x200B;选项。 对工作区和记录类型具有&#x200B;**查看**&#x200B;或更高权限的所有用户对该字段具有相同的权限。

1. （可选）单击&#x200B;**从**&#x200B;继承的权限选项下的用户头像，以查看从工作区继承权限的用户、团队、组、公司或工作角色。

   展开继承的权限时，将显示用户对记录类型的权限。

   >[!TIP]
   >
   >您无法从继承的权限列表中删除单个实体。 列出来自团队、组、公司或工作角色的用户，而不是与他们共享工作区和记录类型时他们关联的实体。

1. （可选且视情况而定）如果要与特定实体共享字段，并授予他们与记录类型不同的字段访问权限，请执行以下操作：

   1. 从&#x200B;**继承权限**&#x200B;中取消选择&#x200B;**启用**&#x200B;选项。 默认情况下，该复选框处于选中状态。

      选项更改为&#x200B;**关闭**。

      >[!TIP]
      >
      >Workspace管理员继续对记录类型和字段具有管理权限。

   1. 在&#x200B;**授予访问权限**&#x200B;框中，添加要授予不同于工作区或记录类型的权限级别的用户、团队、组、公司或工作角色。

      与用户共享字段时，该字段中还会显示其主要工作角色及其电子邮件。 您必须为访问级别中的“用户”对象启用“查看联系信息”设置，才能查看用户的电子邮件。

   1. 选择以下权限级别之一：

      * 查看字段值
      * 管理字段值

      >[!IMPORTANT]
      >
      ><!-- * If users have Contribute or Manage permissions to the workspace and the record type, you can give them Manage permissions to the field. The View permission is dimmed.-->
      >* 如果用户拥有记录类型的Contribute或更高权限，则无法授予用户较低的字段权限。
      >
      >* 您无法向不在工作区中的用户授予权限。 无权访问工作区和记录类型的用户无法访问任何字段。 当他们获得工作区和记录类型的权限时，将能够访问字段。

1. 单击&#x200B;**保存**。

   该字段现在已与其他用户共享。

   <!--
    Not possible for fields: 
    The users you shared the field with receive both an in-app and email notification about having been given permissions to the field.
    For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md).
    -->

## 删除字段的权限

您可以从字段中删除用户的权限。 但是，他们至少将保留对工作区的查看权限和记录类型，这也会为他们至少授予对字段的查看权限。

如果您希望他们对工作区中的记录类型或字段没有权限，则必须从工作区中删除其访问权限。

您无法从继承的权限中删除用户。

{{step1-to-planning}}

1. 打开要停止共享其字段的工作区，然后单击记录类型卡片。 这将打开记录类型页面。
1. 在表视图中，将鼠标悬停在字段列标题的名称上，单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**共享字段**。

   将打开&#x200B;**共享**&#x200B;框。
1. 查找要删除其权限的用户、组、团队、公司或工作角色，展开其名称右侧的权限下拉菜单，然后单击&#x200B;**删除**。

1. 单击&#x200B;**保存**。

   用户不再具有该字段的指定权限。 但是，他们仍拥有记录类型和工作区的权限，除非您同时从这些权限中移除他们。

   对于已从访问字段中删除的用户，不会通知他们不再具有这些权限。
