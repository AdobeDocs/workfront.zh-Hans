---
product-area: projects
navigation-topic: manage-issues
title: 查看问题
description: 您可以查看与项目、任务或开发周期关联的问题。
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: 393f858ba3711b367cf06ad846ea60be0d6d9034
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 0%

---

# 查看问题

<!--Audited: 10/2025-->

您可以查看与项目、任务或开发周期关联的问题。

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
   <td> <p>请求或更高版本</p> <p>查看或更高许可证以查看项目问题部分中的问题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对问题的访问权限</p> <p>查看或更高权限的项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看问题的权限</p> <p> 有关向问题授予权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a></p> <p>有关请求其他权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 基于状态查看问题

要查看有关项目、任务或开发周期的问题，请执行以下操作：

1. 打开包含问题的项目、任务或迭代，然后单击左侧面板中的&#x200B;**问题**。

1. 要显示所有、打开或已关闭的问题，请从&#x200B;**筛选器**&#x200B;下拉菜单中单击下面列出的任何筛选器。

>[!TIP]
>
>筛选器列表会因系统或组管理员选择在列表中显示的内容而异。

* **打开：**&#x200B;显示打开的问题。

  其中包括与解析对象关联的那些以及那些处于“已关闭 — 未决批准”状态的对象。

  有关解析对象的信息，请参阅[解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)。

* **已完成：**&#x200B;显示具有实际完成日期的所有问题。
* **所有**&#x200B;显示所有问题。

## 了解关于问题的信息

您可以在访问问题时查看有关问题的信息。

要访问问题并查看相关信息，请执行以下操作：

1. 打开包含问题的项目、任务或迭代，然后单击左侧面板中的&#x200B;**问题**。
1. 从&#x200B;**筛选器**&#x200B;下拉菜单中，选择筛选器以显示您尝试查看的问题。

   从以下项中选择：

   * Open
   * 已完成
   * 全部

1. 单击问题的名称。

   当您拥有问题的管理权限时，您可以编辑问题中的任何可编辑字段，并向问题添加批准、小时或文档。

1. 从左侧面板中，单击以下任意选项以查看有关该问题的更多信息：

* **更新**：您可以执行以下操作：

   * 对问题进行评论，或回复现有评论。
   * 记录时间。
   * 更改问题的状态。

     有关在Workfront中更新工作的详细信息，请参阅[更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)。

* **文档**：将文档附加到问题。 有关将文档添加到Workfront的更多信息，请参阅[将文档从您的文件系统添加到Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)。

* **问题详细信息**：展开此链接以显示&#x200B;**概述**&#x200B;和&#x200B;**自定义Forms**&#x200B;区域。

  如果您拥有问题的管理权限和自定义表单的编辑权限，则可以在此处编辑某些信息。

  在&#x200B;**概述**&#x200B;区域查看或编辑以下字段：

   * **名称**
   * **路径**：将问题记录到项目时所采用的路径。

     如果问题作为请求队列中的请求提交了，则此处列出了项目的名称、主题组和队列主题。 无法编辑此字段。

     有关提交请求的更多信息，请参阅[创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

   * **描述**
   * **URL**：与问题相关的任何网址。
   * **优先级**：允许您排列问题优先顺序的可视标志。
   * **严重性**：一个视觉标志，指示问题中描述的问题有多严重。
   * **主要联系人**：默认的主要联系人是创建问题的用户。 可以编辑此字段。
   * **计划小时数**：显示某人完成问题所花费的时间。 默认值为8小时。 可以编辑此字段。
   * **实际小时数**：显示完成问题所花费的时间。 这是某人登录问题的实际时间。
   * **计划开始日期**：问题计划开始的日期。 默认为创建问题的日期和时间。
   * **实际开始日期**：问题状态更改为“进行中”的日期和时间。
   * **计划完成日期**：计划完成问题的日期。
   * **实际完成日期**：问题实际完成的日期。 当问题状态变为“已关闭”或“已解决”时，或可手动编辑时，将自动填写此字段。
   * **实际成本**：基于问题记录的实际小时数的成本。 此字段不可编辑。 问题的实际成本是根据以下公式计算的，其中“用户成本费率”是与记录问题时间的用户关联的成本费率：

     问题实际成本=记录的小时数*用户成本率

   * **输入者**：此用户创建了问题。 此字段不可编辑。
   * **上次更新者**：这是上次更新问题中任何字段的用户。 此字段不可编辑。

     在&#x200B;**自定义Forms**&#x200B;区域，查看者可选择要与问题关联的一个或多个自定义表单。

* **小时**：显示问题的小时条目列表。
* **审批：**&#x200B;显示与问题关联的审批路径。

  有关将审批与问题关联的更多信息，请参阅[为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object)中的[将审批流程与工作项关联](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)部分。

## 查看哪些项目和任务存在问题

您可以在项目、任务报告或列表的视图中添加图标以显示它们是否附加了问题。

对于项目和任务，向报表或列表视图添加图标的方式很相似。

要添加显示项目在项目报告中是否有问题的图标，请执行以下操作：

{{step1-click-main-menu}}

1. 单击&#x200B;**报告** > **新报告** > **项目报告**。
1. 在&#x200B;**显示在此列**&#x200B;字段中，开始键入&#x200B;**状态图标**，然后当图标出现在列表中时将其选定。

1. 单击&#x200B;**保存+关闭** 。

   问题图标显示在&#x200B;**状态图标**&#x200B;列中有问题的项目中。

   ![项目列表，带有问题图标](assets/project-list-with-issue-icon-350x132.png)
