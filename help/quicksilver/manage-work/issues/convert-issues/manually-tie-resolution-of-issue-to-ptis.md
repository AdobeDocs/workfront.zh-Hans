---
product-area: projects
navigation-topic: convert-issues
title: 手动将问题的解决与其他问题、任务或项目关联
description: 您可以手动将问题的解决与项目、任务或问题的解决绑定，而无需转换问题。 该问题成为您选择的项目、任务或问题的可解析对象之一。 执行此操作时，项目、任务或问题状态的更改将触发原始问题的状态更改。
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: ea430157da539507c11a559a4dce6b24aca9e5a6
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# 手动将问题的解决与其他问题、任务或项目关联

您可以手动将问题的解决与项目、任务或问题的解决绑定，而无需转换问题。 该问题成为您选择的项目、任务或问题的可解析对象之一。 执行此操作时，项目、任务或问题状态的更改将触发原始问题的状态更改。

>[!TIP]
>
>将问题的解决方式与另一个对象的解决方式关联起来后，便无法再手动编辑原始问题的状态。

有关解析和可解析对象的更多信息，请参阅 [解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## 访问要求

您必须具备以下条件：

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
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题、任务、项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理您链接到其他问题、任务或项目的问题的权限</p> <p>查看或更高权限，以查看您添加到现有问题的问题、任务或项目</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

在开始之前，您必须：

* 有一个问题，您希望将其解决与另一个问题、任务或项目的解决联系起来

* 有其他问题、任务或项目

## 将问题的解决与另一个问题、任务或项目的解决联系起来

1. 导航到要将其解决方案与另一个问题或任务或项目的解决方案相关联的问题。
1. 单击 **问题详细信息** > **概述** 的上界。

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. 转到 **概述** 区域 **问题详细信息** 中。
1. 单击 **解决者** 字段，并从以下类型的解析对象中进行选择：

   * **项目**
   * **任务**
   * **问题**

   根据您选择的对象，将显示以下字段：

   * **解决项目**
   * **解决任务**
   * **解決问题**


1. 开始在 **解决项目问题**, **任务**&#x200B;或 **问题** 字段，然后在列表中显示该字段时单击该字段。

   >[!NOTE]
   >
   >不能将问题的解决与任务或问题所在的项目绑定。 问题的任务或项目不会显示在“解决任务”或“解决任务”字段中。


1. 单击 **保存更改**.

   原始问题将成为您在步骤4和5中选择的项目、任务或问题的可解析对象。 这意味着，在解决对象（您链接到的项目、任务或问题）完成时，原始问题即告结束。

   >[!NOTE]
   >
   >一个项目、任务或问题可能具有多个问题作为可解析对象。
