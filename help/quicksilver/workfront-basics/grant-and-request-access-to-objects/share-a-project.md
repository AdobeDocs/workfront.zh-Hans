---
title: 共享项目
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 在分配访问级别时，Adobe Workfront管理员可以向您授予查看或编辑项目的权限。 有关更多信息，请参阅授予对项目的访问权限。
author: Courtney
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '1574'
ht-degree: 2%

---

# 共享项目

<!-- Audited: 1/2024 -->

在分配访问级别时，Adobe Workfront管理员可以向您授予查看或编辑项目的权限。 有关详细信息，请参阅[授予对项目的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

除了授予用户的访问级别之外，您还可以授予他们查看、贡献或管理您有权共享的特定项目的权限。

权限特定于Workfront中的一个项目，并定义您可以对该项目执行的操作。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对要共享对象的访问权限或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看要共享对象的权限或更高</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关共享项目的注意事项

除了下面的注意事项外，另请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

* 默认情况下，项目的创建者具有管理项目的权限，并被指定为项目所有者。 如果项目分配给其他所有者，则该用户也具有管理项目的权限。 当项目创建者（或所有者）与其他用户共享项目时，他们将特定权限授予这些用户，以控制他们在项目上工作时可以执行的操作。

  但是，如果项目所有者没有“计划”或“标准”许可证，则他们不具有管理项目的完全访问权限。 只有拥有Plan或Standard许可证的用户才有权管理项目。 有关详细信息，请参阅[访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

* 您可以单独共享项目，也可以一次共享多个项目。 共享项目与共享其他对象相同。 有关在Workfront中共享项目的详细信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 您可以向项目授予以下权限：

   * 视图
   * 管理
   * 贡献

* 共享项目时，除非另有指定，否则所有任务、问题和文档都将继承相同的权限。

  有关基于用户对项目的权限管理项目上任务和问题的访问权限的信息，请参阅[](../../manage-work/projects/manage-projects/edit-projects.md#access)编辑项目[一文中的](../../manage-work/projects/manage-projects/edit-projects.md)部分。

  Workfront管理员可以指定文档是否应从用户访问级别更高的对象继承权限。 有关限制文档继承权限的详细信息，请参阅[创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 您可以从项目中删除继承的权限，以便子对象不会继承它们。 有关从对象中删除继承权限的详细信息，请参阅[从对象中删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 不同许可证类型的限制

* 拥有工作人员许可证的用户无权管理项目。 对于工作人员，最高共享权限为Contribute。
* 拥有请求许可证的用户可以查看项目信息，但他们具有有限的项目访问权限。
* 当具有“查看”或“贡献”权限的用户也包含在审批流程中时，项目状态的更改会发生异常。 他们可以审批项目，这更改了项目的状态，但状态为要审批或拒绝的预定义状态。
* 为了能够复制项目，用户还必须具有在其访问级别创建项目的权限。

## 共享项目的方法 {#ways-to-share-a-project}

您可以通过以下方式共享项目：

* 通过执行以下操作之一来手动执行：

   * 正在将用户添加到项目团队。 将用户添加到项目团队时，他们将自动获得项目的“查看”权限。\
     有关将用户添加到项目团队的更多信息，请参阅[项目团队概述](../../manage-work/projects/planning-a-project/project-team-overview.md)中的“将用户添加到项目团队”部分。
   * 使用&#x200B;**共享**&#x200B;选项时单独或批量共享项目。

* 通过执行以下操作之一来自动执行：

   * 将项目置于已与其他人共享的&#x200B;**Portfolio**&#x200B;或&#x200B;**计划**&#x200B;中。 用户将获得与项目组合或项目群相同的项目权限。\
     有关将项目添加到&#x200B;**Portfolio**&#x200B;的信息，请参阅[将项目添加到项目组合](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md)。\
     有关将项目添加到&#x200B;**程序**&#x200B;的信息，请参阅[将项目添加到程序](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md)。
有关查看对象的继承权限的信息，请参阅[查看对象的继承权限](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。

   * 在用于创建项目的模板上向项目共享添加实体。 有关从模板共享项目的信息，请参阅[共享模板](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。
   * 定义项目访问模板。

     >[!TIP]
     >
     >附加或保存模板时，您可以清除模板项目共享规则。

   * 编辑项目并定义&#x200B;**当授予某人此项目的访问权限时**&#x200B;设置。 有关详细信息，请参阅[编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## 共享项目

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，从列表中选择要共享的项目。 此时将打开项目页面。

1. 单击项目名称右侧的&#x200B;**共享**。 将打开&#x200B;**共享[项目名称]**&#x200B;对话框。

   ![共享项目按钮](assets/share-project.png)

1. 在&#x200B;**将项目访问权限授予**&#x200B;字段中，开始键入要与其共享项目的用户、团队、角色、组或公司的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享项目。


1. （可选）选择&#x200B;**具有访问权限**&#x200B;下拉列表并选择项目的访问级别：

   * **只有受邀人员才能访问：**&#x200B;只有受邀参与项目的用户才能访问项目（默认）。
   * **系统中的每个人都可以查看**：系统中的所有用户都可以查看项目，而无需邀请。

1. （可选）要将所选的项目访问设置自动应用于所有新项目，请单击&#x200B;**齿轮**&#x200B;图标![选择齿轮图标](assets/gear-icon.png)，然后选中内联&#x200B;**设置为我的项目访问模板**&#x200B;的框。

   >[!NOTE]
   >
   >项目访问模板将覆盖由访问级别的Workfront管理员授予您的共享默认值。\
   >有关在访问级别中指定项目共享默认值的详细信息，请参阅[授予项目访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)

   <!--
   >this note also appears in Understanding Project Permissions-->


1. 单击用户名右侧的下拉列表，然后选择他们对于此项目的权限级别：


   * **查看**：用户可以查看和共享项目。
   * **Contribute**：用户可以进行更新、记录信息、进行细微编辑和共享项目（还包括所有查看权限）。
   * **管理**：用户具有项目的完全访问权限，但没有管理权限，这些权限是在访问级别授予的（还包括所有“查看”和“贡献”权限）。

1. （可选）单击您授予的权限级别旁边的高级选项图标以配置项目的特定权限。

   ![已配置高级权限选项](assets/advanced-permission-options.png)

1. （可选）要使用链接快速共享项目，请单击&#x200B;**复制链接**，然后将其转发给收件人。

1. 单击&#x200B;**保存**。

## 批量共享项目

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选中要共享的每个项目左侧的框，然后单击页面顶部的&#x200B;**共享**&#x200B;图标![共享](assets/share-icon.png)。 这将打开共享模式窗口。

   ![批量共享项目](assets/bulk-share-icon.png)

1. 在&#x200B;**将项目访问权限授予**&#x200B;字段中，开始键入要与其共享项目的用户、团队、角色、组或公司的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享项目。


1. （可选）选择&#x200B;**具有访问权限**&#x200B;下拉列表并选择项目的访问级别：

   * **只有受邀人员才能访问：**&#x200B;只有受邀参与项目的用户才能访问它们（默认）。
   * **系统中的每个人都可以查看**：系统中的所有用户都可以查看项目，而无需邀请。


1. 单击用户名右侧的下拉列表，然后选择他们对项目的权限级别：

   * **查看**：用户可以查看和共享项目。
   * **Contribute**：用户可以进行更新、记录信息、进行细微编辑和共享项目（还包括所有查看权限）。
   * **管理**：用户拥有对项目的完全访问权限，但没有管理权限，这些权限是在访问级别授予的（还包括所有“查看”和“贡献”权限）。

1. （可选）单击您已授予的权限级别旁边的高级选项图标以配置项目的特定权限。

   ![已配置高级权限选项](assets/advanced-permission-options.png)

1. 单击&#x200B;**保存**。


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## 项目权限选项

下表列出了用户在共享项目时可以授予的权限。 有关用户根据其许可证获得的访问权限的详细信息，请参阅[授予对项目的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>操作</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>参与</strong> </p> </th> 
   <th> <p><strong>查看</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>添加自定义表单</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>更新自定义字段</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>添加审批流程</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>批准项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>批准小时</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>创建项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>添加文档</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>添加问题</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>添加任务</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>复制项目</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>删除项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>修改计划日期</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>共享项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>在系统范围内共享</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>查看项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>更新/评论</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>更改状态</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>记录小时数</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>编辑分配</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>管理基线</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>管理风险*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>管理财务*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>添加/编辑费用*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>查看财务*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>附加模板</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>另存为模板</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>添加/编辑业务案例</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>编辑项目详细信息</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>编辑员工</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>导出至 MS 项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>重新计算财务/时间表*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>设置队列属性</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>在列表中批量编辑项目</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;无权访问财务数据的用户无法管理项目的风险和财务，即使他们拥有项目的编辑权限。 有关访问财务数据的信息，请参阅[授予对财务数据的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
