---
product-area: templates
navigation-topic: templates-navigation-topic
title: 共享项目模板
description: 您可以与用户共享模板，也可以通过在模板级别使用以下共享选项来定义如何与用户共享从模板创建的项目。
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# 共享项目模板

您可以与用户共享模板，也可以通过在模板级别使用以下共享选项来定义如何与用户共享从模板创建的项目。

在Adobe Workfront中共享对象时，您允许其他用户查看、贡献或编辑该对象。

有关Workfront权限的信息，请参阅 [对象共享权限概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

有关在共享模板时可为用户授予的权限的信息，请参阅 [共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对模板的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理模板的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 共享模板 {#share-a-template}

您可以使用“模板共享”与其他用户共享您的模板。 此操作可定义谁有权访问模板。

>[!NOTE]
>
>当您将活动用户指定为“模板所有者”时，该用户将自动接收该模板的“管理”权限。 有关将某人指定为模板所有者的信息，请参阅 [编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

要共享模板，请执行以下操作：

1. 从 **主菜单** 图标 ![](assets/main-menu-icon.png)，单击 **模板**.

1. 执行下列操作之一：\
   单击模板的名称以将其打开，然后单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png)，则 **模板共享**.

   或

   从列表中选择模板，单击共享图标 ![](assets/share-icon.png)，然后单击&#x200B;**模板。**

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 在 **模板访问** 框中，选择要与其共享模板的人员、团队、角色、组或公司。

   您还可以单击 **选项** 使模板在系统范围内可用的图标：

1. 从您共享的每个实体的下拉菜单中，从以下选项中选择：

   * **查看**:具有这些权限的用户可以查看模板并使用模板创建项目，或将其附加到现有项目。

      >[!TIP]
      >
      >您的Workfront管理员必须授予您项目的“编辑”访问权限，才能创建项目。

   * **管理**:具有这些权限的用户能够编辑或删除模板。

      有关“高级设置”的信息 ![](assets/gear-icon-in-access-levels.png) 此处提供，请参阅部分 [模板共享的高级设置](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) 在文章中 [共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. 单击&#x200B;**保存**。

## 从模板共享项目 {#share-a-project-from-a-template}

通过模板项目共享，您可以定义谁有权在模板级别使用模板创建的项目。

要与用户共享将来通过模板创建的项目，请执行以下操作：

1. 执行下列操作之一：\
   单击模板的名称以将其打开，然后单击 **更多** 菜单 ![](assets/qs-more-icon-on-an-object.png)，则 **模板共享**.

   ![从模板共享项目](assets/project-sharing-on-template-nwe-2022-350x172.png)

   或

   从列表中选择模板，单击 **共享**，然后单击&#x200B;**项目。**

1. 在 **项目访问** 框中，选择与模板共享的人员、团队、角色、组或公司。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 从每个实体的下拉菜单中，从以下选项中选择：

   * **无权访问**:您可以指定哪些用户将无权访问模板。\
      仅当从模板批量共享项目时，此选项才可用。 
   * **查看**:具有这些权限的用户可以查看从模板创建的项目。
   * **Contribute**:具有这些权限的用户可以参与从模板创建的项目 
   * **管理**:具有这些权限的用户可以管理或删除从此模板创建的项目。

1. （可选）单击 **选项** 图标，以使项目在系统范围内可用。
1. 单击&#x200B;**保存**。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## 批量共享模板和模板项目

您可以同时共享多个模板以及来自多个模板的项目。

>[!NOTE]
>
>选择多个模板时，您无法查看谁已拥有对各个模板的权限。

1. 转到模板列表。
1. 选择多个模板，然后单击 ![共享](assets/share-icon.png).

   ![批量共享模板或项目](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 单击 **模板** 共享选定的模板。

   或

   单击 **项目** 共享将从选定模板创建的项目。

1. 按照本文以下章节所述，继续共享模板或项目：

   * [共享模板](#share-a-template)
   * [从模板共享项目](#share-a-project-from-a-template)
