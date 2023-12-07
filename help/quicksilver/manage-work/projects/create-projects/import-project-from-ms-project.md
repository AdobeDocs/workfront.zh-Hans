---
product-area: projects
navigation-topic: create-projects
title: 从Microsoft项目导入项目
description: 您可以将项目从Microsoft项目导入Adobe Workfront，并在一个应用程序内管理所有项目。 每次从Microsoft项目导入项目时，都会在Workfront中创建一个新项目。
author: Alina
feature: Work Management
exl-id: dcc3c049-245c-4bb7-b819-b75d6d7e5b67
source-git-commit: 32966d4732221d73aa3397771e157b630f7d5760
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# 从Microsoft项目导入项目

您可以将项目从Microsoft项目导入Adobe Workfront，并在一个应用程序内管理所有项目。 每次从Microsoft项目导入项目时，都会在Workfront中创建一个新项目。

>[!IMPORTANT]
>
>并非所有Microsoft项目字段都已转移到Workfront。
>
>有关Workfront与Microsoft项目之间字段兼容性的更多信息，请参阅 [将Microsoft项目字段映射到Adobe Workfront项目](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).

## 访问要求

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新许可证： Standard </p> 
   或
   <p>当前许可证：计划 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问项目的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">授予项目访问权限</a>. 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在创建项目时，您会自动收到该项目的管理权限 </p> <p> 有关项目权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">在Adobe Workfront中共享项目</a>.</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

<!--old permissions model: 

You must have the following access to perform the steps in this article:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>When you create a project you automatically receive Manage permissions to the project </p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

## 从MS Project创建项目

您可以从主菜单的项目区域创建项目，也可以从项目组合或项目群的项目区域创建项目。

1. 转到Microsoft项目，然后在Workfront中打开要从中导入的项目。
1. 单击 **文件**，则 **另存为** 将项目另存为.xml文件。

1. 登录到Workfront。
1. 执行下列操作之一：

   * 单击 **主菜单** ![](assets/main-menu-icon.png)，单击 **项目**，然后展开 **新建项目**.
   * 转到项目组合，然后展开 **新建项目**.
   * 转到项目，然后展开 **新建项目**.
   * 如果您是组管理员，则还可以在所管理组的项目部分中创建项目。 有关更多信息，请参阅 [创建和修改组的项目](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

1. 选择 **导入MS项目** 选项。

   ![](assets/new-project-dropdown-nwe-350x358.png)

1. 单击 **选择文件**，然后浏览计算机上从Microsoft项目导出的.xml文件。
1. 导入选定的文件。

   Workfront将开始导入过程，并根据从Microsoft项目导出的文件创建新项目。

   导入过程完成后，您将被定向到新的项目页面，该页面会显示已成功完成导入的确认信息。

   >[!NOTE]
   >
   >Workfront的文件上传时间限制为15分钟。 如果文件上传时间超过此时间，我们建议您将项目拆分为多个较小的项目并单独导入它们。 在将任务导入Workfront后，请将任务从一个项目移动到另一个项目以将它们组合到一个项目中。 有关移动任务的信息，请参阅 [移动任务](../../../manage-work/tasks/manage-tasks/move-tasks.md).

1. （可选）继续在Workfront中编辑项目。 有关编辑项目的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

   通过模板创建的新项目的状态与您的Workfront管理员在项目偏好设置区域中定义的状态相对应，或与组管理员在组项目偏好设置区域中定义的状态相对应。 有关配置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
