---
product-area: projects
navigation-topic: convert-issues
title: 手动将问题的解决绑定到其他问题、任务或项目
description: 您可以手动将问题的解决方案与项目、任务或问题的解决方案关联起来，而无需转换问题。 问题将成为您选择的项目、任务或问题的可解析对象之一。 执行此操作时，项目、任务或问题的状态更改会触发原始问题的状态更改。
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# 手动将问题的解决绑定到其他问题、任务或项目

您可以手动将问题的解决方案与项目、任务或问题的解决方案关联起来，而无需转换问题。 问题将成为您选择的项目、任务或问题的可解析对象之一。 执行此操作时，项目、任务或问题的状态更改会触发原始问题的状态更改。

>[!TIP]
>
>当您将问题的解决方法绑定到另一个对象的解决方法时，您将无法再手动编辑原始问题的状态。

有关解析和可解析对象的详细信息，请参阅[解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题、任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理您链接到另一个问题、任务或项目的问题的权限</p> <p>查看您添加到现有问题的问题、任务或项目的或更高权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

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
