---
product-area: projects
navigation-topic: convert-issues
title: 手动将问题的解决绑定到其他问题、任务或项目
description: 您可以手动将问题的解决方案与项目、任务或问题的解决方案关联起来，而无需转换问题。 问题将成为您选择的项目、任务或问题的可解析对象之一。 执行此操作时，项目、任务或问题的状态更改会触发原始问题的状态更改。
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '518'
ht-degree: 0%

---

# 手动将问题的解决绑定到其他问题、任务或项目

<!--Audited: 08/2025-->

您可以手动将问题的解决方案与项目、任务或问题的解决方案关联起来，而无需转换问题。 问题将成为您选择的项目、任务或问题的可解析对象之一。 执行此操作时，项目、任务或问题的状态更改会触发原始问题的状态更改。

>[!TIP]
>
>当您将问题的解决方法绑定到另一个对象的解决方法时，您将无法再手动编辑原始问题的状态。

有关解析和可解析对象的详细信息，请参阅[解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

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
   <td><p>参与者或更高版本</p> 
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题、任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理您链接到另一个问题、任务或项目的问题的权限</p> <p>查看您添加到现有问题的问题、任务或项目的或更高权限</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues,&nbsp;Tasks, Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue you link to another issue, task, or project</p> <p>View or higher permissions to the issue, task, or project you add to the existing issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 先决条件

在开始之前，您必须：

* 有一个问题的解决方案要与另一个问题、任务或项目的解决方案相关联

* 有其他问题、任务或项目

## 将问题的解决与另一个问题、任务或项目的解决联系起来

1. 导航到其解决方案要与另一个问题的解决方案或任务或项目的解决方案关联的问题。
1. 单击左侧面板中的&#x200B;**问题详细信息**，然后展开&#x200B;**概述**&#x200B;区域。

   ![问题详细信息图标](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. 单击&#x200B;**解析者**&#x200B;字段，并从以下解析对象类型中选择：

   * **项目**
   * **任务**
   * **问题**

   根据您选择的对象，将显示以下字段：

   * **解析项目**
   * **解析任务**
   * **正在解决问题**

1. 在&#x200B;**解决项目**、**任务**&#x200B;或&#x200B;**问题**&#x200B;字段中开始键入特定项目、任务或问题的名称，然后当它出现在列表中时单击它。

   >[!NOTE]
   >
   >您无法将问题的解决方案绑定到任务或问题所在的项目。 问题的任务或项目未显示在解析任务或解析任务字段中。


1. 单击&#x200B;**保存更改**。

   原始问题将成为您在步骤4和步骤5中选择的项目、任务或问题的可解析对象。 这意味着当解析对象（您链接到的项目、任务或问题）完成时，原始问题即完成。

   >[!NOTE]
   >
   >一个项目、任务或问题可能具有多个问题作为可解析对象。
