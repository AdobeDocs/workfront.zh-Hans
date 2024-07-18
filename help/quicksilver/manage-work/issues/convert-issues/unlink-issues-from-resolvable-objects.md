---
product-area: projects
navigation-topic: convert-issues
title: 将问题与其解析对象取消链接
description: 通过将问题转换为项目或任务来创建项目或任务时，您可以选择保留原始问题。 您的Adobe Workfront管理员必须启用此首选项，您才能在问题转换期间使用此选项。 有关将问题转化为项目和任务的更多信息，请参阅在Adobe Workfront中转化问题的概述。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# 将问题与其解析对象取消链接

通过将问题转换为项目或任务来创建项目或任务时，您可以选择保留原始问题。 您的Adobe Workfront管理员必须启用此首选项，您才能在问题转换期间使用此选项。\
有关将问题转化为项目和任务的更多信息，请参阅[在Adobe Workfront中转化问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

当您决定保留已转换为项目或任务的问题时，问题的解决与项目或任务绑定。 问题将成为项目或任务的可解析对象。 项目或任务是问题的解析对象。

您也可以手动将问题链接到另一个问题。 在这种情况下，第二个问题将成为第一个问题的解析对象。\
有关解析对象的详细信息，请参阅[解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

>[!TIP]
>
>问题状态无法更改，因为它会自动随解析对象的状态更改。

您可以从问题中删除项目、任务或问题，从而取消问题解决方案与项目、任务或问题解决方案的链接。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

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
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看对任务和项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>查看任务或项目的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 从项目、任务或问题中取消问题链接

1. 转到链接到项目、任务或问题的问题。
1. 单击&#x200B;**问题详细信息**&#x200B;部分。
1. 转到&#x200B;**问题详细信息**&#x200B;部分的&#x200B;**概述**&#x200B;区域。
1. 在&#x200B;**解析者**&#x200B;字段中，删除可解析的对象类型。\
   问题可以由项目、任务或问题解决。

   这将从问题中删除解析对象。

1. 单击&#x200B;**保存** **更改**。\
   问题不再与项目、任务或问题关联，您现在可以单独解决该问题。
