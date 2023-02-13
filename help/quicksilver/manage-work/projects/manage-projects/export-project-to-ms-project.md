---
product-area: projects
navigation-topic: manage-projects
title: 将项目导出到Microsoft项目
description: 您可以将Adobe Workfront项目导出到Microsoft项目。
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 将项目导出到Microsoft项目

您可以将Adobe Workfront项目导出到Microsoft项目。 

>[!IMPORTANT]
>
>* 并非所有Workfront字段都在Microsoft项目文件中传输。\
   >  有关Workfront与Microsoft项目之间字段兼容性的更多信息，请参阅文章 [将Microsoft项目字段映射到Adobe Workfront项目](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* 我们建议您限制将项目从一个应用程序转移到另一个应用程序的次数。 
>


## 访问要求

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>  <p>Current license: Light or higher</p>
   Or
   <p>Legacy license: Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问项目</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问项目的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予对项目的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 查看项目的或更高权限</p> <p>有关项目权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>.</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将项目从Workfront导出到Microsoft项目

您可以从项目页面或项目列表或报表中从Workfront导出项目。

1. 转到要导出的项目，然后单击 **更多** 图标 ![](assets/qs-more-menu.png) 项目名称的权限

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报表并选择一个项目，然后单击更多图标 ![](assets/qs-more-menu.png) 列表顶部。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 单击 **导出MS项目**.

   项目将作为XML文件下载到您的计算机，并准备好导入到Microsoft项目中。 
