---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 配置请求类型
description: 在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 您还可以提交请求，这些请求会被记录为指定为请求队列的项目中的问题。 问题和请求在Adobe Workfront中被视为可互换。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# 配置请求类型

在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 您还可以提交请求，这些请求会被记录为指定为请求队列的项目中的问题。 问题和请求在Adobe Workfront中被视为可互换。

有关在 [!DNL Workfront]，请参阅 [创建问题](../../../manage-work/issues/manage-issues/create-issues.md). 有关在中创建请求的信息 [!DNL Workfront]，请参阅 [创建和提交 [!DNL Adobe Workfront] 请求](../../../manage-work/requests/create-requests/create-submit-requests.md). 有关将请求类型与项目关联的信息，请参阅 [为项目定义请求类型](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## 自定义请求类型的名称

As a [!DNL Workfront] 管理员，您可以在系统中配置请求类型的名称。 新名称将显示在 [!DNL Workfront] 其中 **[!UICONTROL 问题类型]** 或 **[!UICONTROL 请求类型]** 字段显示：

* 在 **[!UICONTROL 队列详细信息]** 接收问题或请求的项目区域。
* 如果为请求队列选择了多个请求类型，则在 **[!UICONTROL 新问题] 表单** 在 **[!UICONTROL 问题类型]** 字段中，选择“新建问题”或“提交新请求”。

   有关在 [!DNL Workfront]，请参阅  [创建问题](../../../manage-work/issues/manage-issues/create-issues.md)

   有关在 [!DNL Workfront]，请参阅  [创建和提交 [!DNL Adobe Workfront] 请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

* 在 **[!UICONTROL 队列主题详细信息]** 表单。\
   有关创建队列主题的更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

要自定义请求类型的名称，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 项目首选项]** > **[!UICONTROL 状态]**.

1. 单击 **[!UICONTROL 问题]** 选项卡。
1. 在 **[!UICONTROL 问题]** 选项卡，将鼠标悬停在请求类型的名称上，然后单击 **[!UICONTROL 编辑]** 图标。

   ![](assets/edit-request-type-name-nwe.png)

1. 在显示的框中，键入新名称，然后按 **[!UICONTROL 输入]**.

## 在不同请求类型中配置问题状态

您可以将每个请求类型与不同的问题状态相关联。 您还可以根据问题的类型更改状态在问题上的显示顺序。

有关更改问题状态的默认顺序和配置问题状态的详细信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) 部分 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
