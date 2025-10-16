---
product-area: projects
navigation-topic: convert-issues
title: 将问题与其解析对象取消链接
description: 通过将问题转换为项目或任务来创建项目或任务时，您可以选择保留原始问题。 您的Adobe Workfront管理员必须启用此首选项，您才能在问题转换期间使用此选项。 有关将问题转化为项目和任务的更多信息，请参阅在Adobe Workfront中转化问题的概述。
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# 将问题与其解析对象取消链接

<!--Audited: 08/2025-->

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
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看对任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>查看任务或项目的权限</p> </td> 
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
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and&nbsp;Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 从项目、任务或问题中取消问题链接

1. 转到链接到项目、任务或问题的问题。
1. 单击&#x200B;**问题详细信息**&#x200B;部分。
1. 转到&#x200B;**问题详细信息**&#x200B;部分的&#x200B;**概述**&#x200B;区域。
1. 在&#x200B;**解析者**&#x200B;字段中，删除可解析的对象类型。\
   问题可以由项目、任务或问题解决。

   这将从问题中删除解析对象。

1. 单击&#x200B;**保存** **更改**。\
   问题不再与项目、任务或问题关联，您现在可以单独解决该问题。
