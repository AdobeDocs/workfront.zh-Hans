---
product-area: projects
navigation-topic: convert-issues
title: 取消与其解决对象的问题的关联
description: 通过将问题转换为项目或任务来创建项目或任务时，您可以选择保留原始问题。 您的Adobe Workfront管理员必须启用此首选项才能在问题转换期间使用此选项。 有关将问题转换为项目和任务的更多信息，请参阅在Adobe Workfront中转换问题概述。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 取消与其解决对象的问题的关联

通过将问题转换为项目或任务来创建项目或任务时，您可以选择保留原始问题。 您的Adobe Workfront管理员必须启用此首选项才能在问题转换期间使用此选项。\
有关将问题转换为项目和任务的更多信息，请参阅 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

当您决定保留已转换为项目或任务的问题时，问题的解决将与项目或任务绑定。 该问题成为项目或任务的可解析对象。 项目或任务是问题的“解决对象”。

您还可以手动将问题链接到另一个问题。 第二个问题成为第一个问题的解决对象，在本例中为。\
有关“解析对象”(Resolving Objects)的详细信息，请参阅 [解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>无法更改问题状态，因为它会随“解决对象”的状态自动更改。

您可以通过从问题中删除项目、任务或问题，将问题的解决与项目、任务或问题的解决取消关联。

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
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>查看任务或项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将问题与项目、任务或问题取消链接

1. 转到链接到项目、任务或问题的问题。
1. 单击 **问题详细信息** 中。
1. 转到 **概述** 区域 **问题详细信息** 中。
1. 在 **解决者** 字段中，删除可解析的对象类型。\
   问题可以通过项目、任务或问题来解决。

   这会从问题中删除解析对象。

1. 单击 **保存** **更改**.\
   该问题不再与项目、任务或问题链接，您现在可以单独解决该问题。
