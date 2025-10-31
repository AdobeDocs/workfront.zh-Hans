---
product-area: templates
navigation-topic: templates-navigation-topic
title: 共享项目模板
description: 您可以与用户共享模板，或者通过在模板级别使用以下共享选项定义如何将基于模板创建的项目共享给用户。
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# 共享项目模板

您可以与用户共享模板，或者通过在模板级别使用以下共享选项定义如何将基于模板创建的项目共享给用户。

在Adobe Workfront中共享对象时，您可以允许其他用户查看、参与或编辑该对象。

有关Workfront权限的信息，请参阅[对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

有关共享模板时可以向用户授予的权限的信息，请参阅[共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

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
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对模板的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理模板的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 共享模板 {#share-a-template}

您可以使用模板共享与其他用户共享您的模板。 此操作定义谁对模板具有权限。

>[!NOTE]
>
>当您将活动用户指定为模板所有者时，该用户会自动接收对模板的管理权限。 有关将某人指定为模板所有者的信息，请参阅[编辑项目模板](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)。

要共享模板：

1. 从&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)中，单击&#x200B;**模板**。

1. 执行下列操作之一：\
   单击模板名称以将其打开，然后单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**模板共享**。

   或

   从列表中选择模板，单击“共享”图标![](assets/share-icon.png)，然后单击&#x200B;**模板。**

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 在&#x200B;**模板访问**&#x200B;框中，选择要与其共享模板的人员、团队、角色、组或公司。

   您还可以单击&#x200B;**选项**&#x200B;图标以使模板在系统范围内可用：

1. 从与您共享的每个实体的下拉菜单中，从以下各项中选择：

   * **查看**：具有这些权限的用户可以查看模板，并使用模板创建项目，或将其附加到现有项目。

     >[!TIP]
     >
     >您的Workfront管理员必须向您授予项目的“编辑”权限才能创建项目。

   * **管理**：具有这些权限的用户能够编辑或删除模板。

     有关此处提供的高级设置![](assets/gear-icon-in-access-levels.png)的信息，请参阅文章[共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions)中的[模板共享高级设置](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)部分。

1. 单击&#x200B;**保存**。

## 从模板共享项目 {#share-a-project-from-a-template}

利用模板项目共享，您可以在模板级别定义谁对从模板创建的项目具有权限。

要与用户共享从模板创建的未来项目，请执行以下操作：

1. 执行下列操作之一：\
   单击模板名称以将其打开，然后单击&#x200B;**更多**&#x200B;菜单![更多图标](assets/more-icon.png)，然后单击&#x200B;**模板共享**。

   ![从模板共享项目](assets/project-sharing-on-template-nwe-2022-350x172.png)

   或

   从列表中选择模板，单击&#x200B;**共享**，然后单击&#x200B;**项目。**

1. 在&#x200B;**项目访问**&#x200B;框中，选择与模板共享的人员、团队、角色、组或公司。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 从每个实体的下拉菜单中，选择以下选项：

   * **无访问权限**：您可以指定哪些用户无权访问模板。\
     仅当从模板批量共享项目时，此选项才可用。 
   * **视图**：具有这些权限的用户可以查看从模板创建的项目。
   * **Contribute**：具有这些权限的用户可以参与从模板创建的项目 
   * **管理**：具有这些权限的用户可以管理或删除从此模板创建的项目。

1. （可选）单击&#x200B;**选项**&#x200B;图标以使项目在系统范围内可用。
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

## 从模板批量共享模板和项目

您可以同时共享多个模板以及多个模板中的项目。

>[!NOTE]
>
>如果选择多个模板，则无法查看谁已经拥有各个模板的权限。

1. 转到模板列表。
1. 选择多个模板，然后单击![共享](assets/share-icon.png)。

   ![批量共享模板或项目](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享对象。

1. 单击&#x200B;**模板**&#x200B;以共享所选模板。

   或

   单击&#x200B;**项目**&#x200B;以共享将从所选模板创建的项目。

1. 继续共享模板或项目，如本文以下部分所述：

   * [共享模板](#share-a-template)
   * [从模板共享项目](#share-a-project-from-a-template)
