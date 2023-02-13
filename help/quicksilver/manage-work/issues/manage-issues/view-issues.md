---
product-area: projects
navigation-topic: manage-issues
title: 查看问题
description: 您可以查看与项目、任务或小版本关联的问题。
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# 查看问题

您可以查看与项目、任务或小版本关联的问题。

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
   <td> <p>请求或更高版本</p> <p>查看或获取更高许可，以查看项目“问题”部分中的问题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看问题的访问权限</p> <p>查看或更高权限访问项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看问题的权限</p> <p> 有关授予问题权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 查看基于状态的问题

要查看项目、任务或小版本的问题，请执行以下操作：

1. 打开包含问题的项目、任务或小版本，然后单击 **问题** 中。

1. 要显示所有、打开或关闭的问题，请单击 **过滤器** 下拉菜单。

>[!TIP]
>
>过滤器列表会因系统或组管理员选择在其中显示的内容而异。

* **打开：** 显示打开的问题。

   这包括与“解析对象”关联的对象以及处于“已关闭 — 待批准”状态的对象。

   有关“解析对象”(Resolving Objects)的信息，请参阅 [解析和可解析对象概述](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **已完成：** 显示具有实际完成日期的所有问题。
* **全部** 显示所有问题。

## 了解有关问题的信息

您可以在访问问题时查看有关问题的信息。

要访问问题并查看其相关信息，请执行以下操作：

1. 打开包含问题的项目、任务或小版本，然后单击 **问题** 中。
1. 从 **过滤器** 下拉菜单中，选择过滤器以显示您尝试查看的问题。

   从以下选项中进行选择：

   * 打开
   * 已完成
   * 全部

1. 单击问题的名称。

   在您对问题拥有管理权限后，可以编辑问题中的任何可编辑字段，并向问题添加批准、小时或文档。

1. 在左侧面板中，单击以下任意选项以查看有关该问题的更多信息：

* **更新**:您可以执行以下操作：

   * 对问题发表评论或对现有评论的回复。
   * 记录时间。
   * 更改问题的状态。

      有关更新Workfront中工作的更多信息，请参阅 [更新工作](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **文档**:将文档附加到问题。 有关将文档添加到Workfront的更多信息，请参阅 [从文件系统将文档添加到Adobe Workfront](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **问题详细信息**:展开此链接可显示 **概述** 和 **自定义Forms** 区域。

   如果您拥有对问题的管理权限并拥有对自定义表单的编辑权限，则可以在此处编辑一些信息。

   在 **概述** 区域：

   * **名称**
   * **路径**:将问题记录到项目的路径。

      如果问题是作为请求队列中的请求提交的，则此处将列出项目名称、主题组和队列主题。 无法编辑此字段。

      有关提交请求的更多信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **描述**
   * **URL**:任何与问题相关的网址。
   * **优先级**:一个可视标记，用于确定问题的优先级。
   * **严重性**:一个可视标记，指示问题中描述的问题的严重程度。
   * **主要联系人**:默认的主要联系人是创建问题的用户。 可以编辑此字段。
   * **计划小时数**:显示完成问题所花费的时间。 默认为8小时。 可以编辑此字段。
   * **实际小时数**:显示完成问题所花费的时间。 这是某人为问题记录的实际时间。
   * **计划开始日期**:计划开始问题的日期。 默认为创建问题的日期和时间。
   * **实际开始日期**:问题状态更改为“进行中”的日期和时间。
   * **计划完成日期**:计划完成问题的日期。
   * **实际完成日期**:实际完成问题的日期。 当问题状态更改为“已关闭”或“已解决”时，将自动填写此字段，或者可以手动编辑此字段。
   * **实际成本**:基于问题上记录的实际小时数的成本。 此字段不可编辑。 问题的实际成本是根据以下公式计算的，其中用户成本率是与记录问题时间的用户相关联的成本率：

      发放实际成本=记录的小时数*用户成本率

   * **输入者**:这是创建问题的用户。 此字段不可编辑。
   * **上次更新者**:这是上次更新问题任何字段的用户。 此字段不可编辑。

      在 **自定义Forms** 区域，视图中可以选择一个或多个要与问题关联的自定义表单。

* **小时**:显示问题上的小时条目列表。
* **批准：** 显示与问题关联的批准路径。

   有关将审批与问题关联的详细信息，请参阅 [将审批流程与工作项关联](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) 部分 [为工作项创建审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## 查看哪些项目和任务存在问题

您可以在项目或任务报表或列表的视图中添加图标，以显示它们是否存在附加的问题。 向报表或列表视图添加图标与向项目和任务添加图标类似。

要添加图标以显示项目在项目报表中是否遇到问题，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角。
1. 单击 **报表** > **新建报表** > **项目报表**.
1. 在 **在此列中显示** 字段，开始键入 **状态图标**，然后在列表中显示时将其选中。

1. 单击 **保存并关闭** .

   问题图标会显示在 **状态图标** 列。

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
