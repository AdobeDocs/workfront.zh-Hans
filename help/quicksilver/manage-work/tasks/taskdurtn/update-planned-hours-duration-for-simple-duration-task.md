---
product-area: projects
navigation-topic: task-duration
title: 使用简单持续时间类型更新任务的计划小时数和持续时间
description: 默认情况下，Adobe Workfront会根据计划小时数量计算具有简单持续时间类型的任务的持续时间。 但是，您也可以在Workfront的某些区域中手动编辑计划小时数和简单持续时间任务的持续时间。
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# 使用简单持续时间类型更新任务的计划小时数和持续时间

默认情况下，Adobe Workfront会根据计划小时数量计算具有简单持续时间类型的任务的持续时间。 但是，您也可以在Workfront的某些区域中手动编辑计划小时数和简单持续时间任务的持续时间。

您可以编辑任务的计划小时数和持续时间，该任务具有内嵌的简单持续时间类型，也可以在“分配”区域的任务层编辑。

有关编辑内联信息的更多信息，请参阅 [在Adobe Workfront中内联编辑列表中的项目](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

本文介绍了如何在任务层的“分配”区域中使用简单持续时间类型来更新任务的计划小时数和持续时间。

## 访问要求

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
   <td> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑任务访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 使用简单持续时间类型更新任务的计划小时数和持续时间

>[!IMPORTANT]
>
>在您手动更新简单持续时间任务上的持续时间后，Workfront会停止根据计划小时数计算持续时间。

要在“高级分配”框中编辑具有简单持续时间类型的任务的计划小时数和持续时间，请执行以下操作：

1. 在任务列表中，单击要更改其持续时间类型的任务名称。
1. 执行下列操作之一：

   * 单击 **更多** 图标 ![](assets/qs-more-icon-on-an-object.png) 在任务名称旁边，单击 **编辑**，则 **分配**.
   * 单击 **已分配给** 或任务标题的“分配”(Assignments)区域中的分配名称，然后单击 **高级**.

1. 输入 **计划小时数** 例如，10小时。 在分配给任务的所有资源之间平均分配计划小时数的总数。
1. （可选）人工调整分配给任务的每个资源的计划小时数。 任务更新的计划小时数总数，以反映单独分配给您的资源的新小时数。
1. 输入任务的值 **持续时间**，例如2天。

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 单击&#x200B;**保存**。
