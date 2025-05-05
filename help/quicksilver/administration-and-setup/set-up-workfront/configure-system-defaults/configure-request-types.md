---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: 配置请求类型
description: 在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 您也可以提交请求，在指定为请求队列的项目中，这些请求将记录为问题。 在Adobe Workfront中，问题和请求被视为可互换的。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 配置请求类型

在处理项目时，您可能会发现出现意外事件。 您可以将这些意外事件记录为特定项目或任务的问题。 您也可以提交请求，在指定为请求队列的项目中，这些请求将记录为问题。 在Adobe Workfront中，问题和请求被视为可互换的。

有关在[!DNL Workfront]中创建问题的信息，请参阅[创建问题](../../../manage-work/issues/manage-issues/create-issues.md)。 有关在[!DNL Workfront]中创建请求的信息，请参阅[创建并提交 [!DNL Adobe Workfront] 请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。 有关将请求类型与项目关联的信息，请参阅[为项目定义请求类型](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [!UICONTROL Standard]</p>
   或
   <p>当前： [!UICONTROL 计划]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

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

作为[!DNL Workfront]管理员，您可以在系统中配置请求类型的名称。 新名称显示在[!DNL Workfront]中显示&#x200B;**[!UICONTROL 问题类型]**&#x200B;或&#x200B;**[!UICONTROL 请求类型]**&#x200B;字段的任何区域：

* 在接收问题或请求的项目的&#x200B;**[!UICONTROL 队列详细信息]**&#x200B;区域中。
* 如果您为请求队列选择了多个请求类型，则在创建新问题或提交新请求时，请在&#x200B;**[!UICONTROL 问题类型]**&#x200B;字段的&#x200B;**[!UICONTROL 新建问题]表单**&#x200B;中进行。

  有关在[!DNL Workfront]中创建问题的详细信息，请参阅[创建问题](../../../manage-work/issues/manage-issues/create-issues.md)

  有关在[!DNL Workfront]中创建请求的更多信息，请参阅[创建并提交 [!DNL Adobe Workfront] 请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

* 在&#x200B;**[!UICONTROL 队列主题详细信息]**&#x200B;表单上配置队列主题时。\
   有关创建队列主题的详细信息，请参阅[创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)。

要自定义请求类型的名称，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 项目首选项]** > **[!UICONTROL 状态]**。

1. 单击&#x200B;**[!UICONTROL 问题]**&#x200B;选项卡。
1. 在&#x200B;**[!UICONTROL 问题]**&#x200B;选项卡的顶部，将鼠标悬停在请求类型的名称上，然后单击显示的&#x200B;**[!UICONTROL 编辑]**&#x200B;图标。

   ![编辑请求类型名称](assets/edit-request-type-name-nwe.png)

1. 在出现的框中，键入新名称，然后按&#x200B;**[!UICONTROL Enter]**。

## 配置不同请求类型中的问题状态

您可以将每种请求类型与不同的问题状态相关联。 您还可以根据问题的类型更改问题状态显示的顺序。

有关更改问题状态的默认顺序和配置问题状态的更多信息，请参阅[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中的[创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)部分。
