---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: 对象权限共享概述
description: 您可以共享或删除您创建的对象或与您共享对象的权限。
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 05f8dc8770c185720520fc631e19c75b925a70bf
workflow-type: tm+mt
source-wordcount: '1182'
ht-degree: 1%

---

# 对象权限共享概述

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
与系统中的某人共享对象时，您可以授予收件人以下任意权限：查看、贡献和管理。

您不必是Adobe Workfront管理员，即可共享您有权访问的对象的权限，但您对对象的权限可在Workfront管理员设置的访问级别内使用。

您可以共享或删除您创建的对象或与您共享对象的权限。 如果您不是对象的创建者，则除了要共享对象的权限之外，您还必须对要在访问级别中共享的对象具有“共享”访问权限。 有关访问级别的信息，请参阅[新访问级别概述](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)或[访问级别概述](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)。

>[!NOTE]
>
>Workfront管理员可以为系统中的任何项目为所有用户添加或删除权限，而无需成为这些项目的所有者。

## 可在Workfront中共享的对象

您可以在Workfront中与其他用户共享以下对象：

* **项目**：有关详细信息，请参阅[在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。

* **模板**：有关详细信息，请参阅[共享项目模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md)。

* **Portfolio**：有关详细信息，请参阅[共享项目组合](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md)。

* **程序**：有关信息，请参阅[共享程序](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md)。

* **任务**：有关信息，请参阅[共享任务](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)。

* **问题**：有关信息，请参阅[共享问题](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)。

* **文档**：有关信息，请参阅[共享文档](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md)。

* **文档文件夹**：有关信息，请参阅[共享文档文件夹](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

* **验证**：有关信息，请参阅[在Workfront中共享验证](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

* **报告、仪表板和日历**：有关信息，请参阅[共享报告、仪表板和日历](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md)。 此外，请参阅以下文章：

   * [在Adobe Workfront中共享报表](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [共享功能板](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [共享日历报告](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **筛选器、视图和分组**：有关信息，请参阅[共享筛选器、视图或分组](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md)。

* **计划**：有关信息，请参阅[在Scenario Planner](../../scenario-planner/share-a-plan.md)中共享计划。

  这需要额外的许可证。

* **目标**：有关信息，请参阅[在Workfront目标中共享目标](../../workfront-goals/workfront-goals-settings/share-a-goal.md)。

  这需要额外的许可证。

## 有关共享对象的注意事项

* 您只能共享您对对象的相同级别或更低级别的权限。

  例如，如果您拥有对象的Contribute权限，则无法向其他用户授予对该对象的“管理”权限。

* 您无法共享权限级别高于用户访问级别的对象。

  例如，如果用户拥有其访问级别的“查看项目”访问权限，则您无法授予他们项目的“管理”权限。
* 至少具有查看对象权限的用户可以与其他人共享该对象。
* 您可以与活动用户、工作角色、团队、组或公司共享对象。

  >[!NOTE]
  >
  >您只能与其他活动用户共享计划或目标。 这需要额外的许可证。
  >
  >
  >有关更多信息，请参阅：
  >
  >* [在Scenario Planner](../../scenario-planner/share-a-plan.md)中共享计划
  >* [在Workfront目标中共享目标](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## 共享限制

您最多可以与100个实体（用户、团队、组、工作角色、公司）共享对象。 我们建议您与组、团队或公司共享对象，而不是与个人用户共享对象，以避免此限制。

## 共享对象的权限

下表说明了共享对象时可以选择的权限级别。 并非所有对象都具有所有这些设置。 您可以向其他实体授予查看或管理对象的权限。 如果要共享项目、任务或问题，还可以向其授予Contribute的权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>查看</strong></td> 
   <td> <p>您可以对对象执行以下操作：</p> 
    <ul> 
     <li><p>查看对象</p></li> 
     <li><p>将文档添加到对象</p></li> 
     <li><p>将问题添加到对象（如果它是任务或项目）</p></li> 
     <li><p>查看有关对象的财务信息</p></li> 
     <li> <p>共享对象<br></p> <p>当您共享对象时，您可以授予其他用户您仅对对象拥有的相同权限级别，而不是更高的级别。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>参与</strong></td> 
   <td> <p>您可以对对象执行以下操作：</p> 
    <ul> 
     <li>查看权限包含的所有操作。</li> 
     <li>向其添加费用</li> 
     <li>向其添加任务（如果它是一个项目）</li> 
     <li>编辑其上的自定义Forms</li> 
     <li>记录对象的小时数</li> 
     <li>在其中进行分配</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>管理</strong></td> 
   <td> <p>您可以对对象执行以下操作：</p> 
    <ul> 
     <li>查看和Contribute权限中包含的所有操作</li> 
     <li>删除它</li> 
     <li>管理其中的财务信息</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>向外部用户公开</strong></td> 
   <td> <p>没有Workfront帐户的任何人都可以通过单击指向该对象的链接来查看它。 并非所有对象都适用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>在系统范围内可见。</strong></td> 
   <td> <p>该对象可在搜索中找到，并可由具有Workfront帐户的用户查看。</p><p><b>注意</b>：具有参与者或请求者许可证的用户无法查看项目，即使启用了此设置也是如此。 </td> 
  </tr> 
 </tbody> 
</table>

## 了解继承的权限和对象的层次结构

### 从父对象继承的权限 {#permissions-inherited-from-parent-objects}

Workfront中的权限是分层继承的。 这意味着，如果您授予用户对父对象的权限，则默认情况下这些用户将获得与其关联的子对象的相同权限。

例如，如果您授予用户Contribute项目权限，则该用户拥有与该项目关联的所有任务和问题（子对象）的Contribute权限。

继续上面的示例，您不能限制对子对象的权限。 如果您不希望用户拥有与项目关联的子对象的Contribute权限，则必须手动从对象中删除继承的权限，然后调整单个用户的权限，包括任何高级设置。 

有关Workfront中对象的层次和相互依赖关系的详细信息，请参阅文章[Adobe Workfront对象概述](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[对象相互依赖关系和层次](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects)部分。

>[!NOTE]
>
>Workfront管理员可以禁用访问级别中文档的继承权限。 有关禁用访问级别中文档的继承权限的详细信息，请参阅[创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

### 通过组织成员资格获得的权限  {#permissions-acquired-through-organizational-memberships}

如果您将管理权限授予对象上的用户组，并将查看权限授予该组中同一对象上的单个用户，则该用户将具有通过该对象的组成员资格授予的最高级别的权限（管理）。 

如果要将较低权限授予已属于具有较高权限级别的组织单位（组、团队、工作角色或公司）的用户，则必须从组织单位中删除权限，并单独添加具有较低权限级别的用户。


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 共享对象

有关如何共享对象的信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

## 从对象中删除权限

有关如何从对象中删除权限的信息，请参阅[从对象中删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 请求对象的权限

当有人向您发送指向您没有查看权限的对象的链接时，或者当您对对象拥有较低权限并且希望请求更高级别的权限时，您可以请求对对象的权限。 

您可以向拥有对象共享权限的任何人请求对对象的访问权限。 

有关请求对象权限的详细信息，请参阅[请求访问对象](../../workfront-basics/grant-and-request-access-to-objects/request-access.md)。
