---
title: 共享模板
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: 作为Adobe Workfront管理员，您可以在分配其访问级别时授予用户查看或编辑模板的访问权限。 用户必须具有计划许可证才能访问编辑模板。
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: b4e90918c5f499638d0cf5355dc75c3ceca48293
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 2%

---

# 共享模板

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用。</span>

作为Adobe Workfront管理员，您可以在分配其访问级别时授予用户查看或编辑模板的访问权限。 用户必须具有计划许可证才能访问编辑模板。

有关授予对模板的访问权限的详细信息，请参阅[授予对模板的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)。

除了您授予的访问级别之外，用户还可以从共享这些模板的其他用户那里获得查看或管理特定模板的权限。

>[!NOTE]
>
>权限级别在访问级别中起作用。 例如，如果用户的访问级别仅允许他们查看模板，则他们将无法获得管理模板的权限。

权限特定于Workfront中的一个项目，并定义您可以对该项目执行的操作。

## 共享模板时的注意事项

* 除了下面的注意事项外，另请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。
* 默认情况下，模板的创建者以及模板所有者具有模板的管理权限。 有关将用户指定为模板所有者的信息，请参阅[编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)。
* 共享模板时，您可以共享以下内容：

   * 模板

     有关如何共享模板的详细信息，请参阅[共享项目模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md)。

     您可以向模板授予以下权限：

      * 查看
      * 管理

        ![](assets/view-on-template-262x221.png) ![](assets/manage-on-template-225x280.png)

     在预览中<span class="preview">：
     ![](assets/template-permissions.png)
  </span>

   * 使用该模板创建的未来项目。 您可以为从模板创建的项目授予与对单个项目相同的权限级别。 

     有关如何从模板级别共享项目的信息，请参阅[共享项目模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md)。

* 共享模板或使用该模板创建的项目时，默认情况下，用户将继承与模板或项目关联的所有子对象的相同权限。

  有关Workfront中对象层次结构的详细信息，请参阅  [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

* 在共享模板时，除非另有指定，否则所有模板任务和文档以及使用该模板创建的未来项目上的问题都将继承相同的权限。

  有关基于用户对项目的权限管理项目上模板任务和问题的访问权限的信息，请参阅[编辑项目模板](../../manage-work/projects/create-and-manage-templates/edit-templates.md)一文中的[访问](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access)部分。

* Workfront管理员可以指定文档是否应从用户访问级别更高的对象继承权限。 有关限制文档继承权限的详细信息，请参阅[创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 您无法单独共享模板任务。 共享模板也会共享模板任务。 从模板共享项目也会共享未来的项目任务。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## 模板共享的高级设置

下表显示了允许用户查看或管理模板时，您可以授予用户哪些权限。 有关共享模板的说明，请参阅[共享项目模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md)一文中的[共享模板](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share)部分。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>操作</th> 
   <th>管理</th> 
   <th>查看</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>复制</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>删除</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>编辑模板详细信息</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>查看模板</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>共享</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>在系统范围内共享</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>添加文档</p> <p>提示：有时候，人们在将文档添加到项目模板时以为自己正在将文档添加到项目中。 通过禁用此设置，可以为收件人阻止这种情况。</p> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
 </tbody> 
</table>

要了解您授予用户使用模板创建的项目的权限，请参阅[在Adobe Workfront中共享项目](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。
