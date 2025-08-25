---
product-area: projects
navigation-topic: create-projects
title: 创建与Frame.io连接的项目
description: 项目是Adobe Workfront中的一个大型工作单位。 您可以从头开始创建项目，使用模板，或将问题或任务转换为项目。
author: Courtney
feature: Work Management
hide: true
hidefromtoc: true
exl-id: 230d8e62-a3c9-4e38-9b26-5ba1c4f56391
source-git-commit: f381b37e6d4537e6f83e55ed4a2f4ff7f868dd54
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 1%

---

# 创建与Frame.io连接的项目

通过Workfront和Frame.io集成，您可以在Workfront中创建在Frame.io中镜像的项目，从而提供无缝的审阅和批准体验。

当Workfront项目与Frame.io连接时，您可以

* **将Frame.io用户分配给任务**：启用Frame.io的用户在分配给Workfront任务时会收到电子邮件通知，告知有工作要完成。
* **与Frame.io用户共享项目**：与启用了Frame.io的用户共享项目时，用户可以访问Workfront和Frame.io中的项目。
* **与Frame.io共享创意资料**：项目协调员可以使用单向同步项目文件夹，直接从Workfront将说明和资料发送给Frame.io中的创意用户。 [!BADGE 即将推出]{type=Informative}
* **跟踪任务进度**：创意人员可以发送完成的资源并将任务标记为完成 — 所有这些操作无需离开Frame.io。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在创建项目时，您会自动收到该项目的管理权限。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* 在Workfront设置区域中设置默认的Frame.io帐户
* 在Workfront用户配置文件中启用Frame.io用户

有关上述先决条件的更多信息，请参阅[配置 [!DNL Workfront] 和 [!DNL Frame.io] 集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md)。


## 创建新项目模板

在构建新模板时，您可以为所有任务和未来项目设置输入信息。 然后，此信息将传输到您从模板创建的任何项目。

Frame.io中的项目由连接到Workfront组的团队组织。 我们建议使用项目模板来创建连接的项目，因为您之前可以设置项目组。

如果选择从头开始创建项目，Workfront会自动添加默认项目组，并在Frame.io中的该默认团队下创建镜像Frame.io项目。

>[!NOTE]
>
>在创建项目后更新组不会更改Frame.io团队。


### 创建模板并指定项目组

{{step1-to-templates}}

1. 单击&#x200B;**新建模板**。
1. 键入模板的名称，然后按&#x200B;**Enter**&#x200B;保存该名称。
1. 在左侧面板中，单击&#x200B;**模板详细信息**。
1. 在&#x200B;**模板关联**&#x200B;部分中，确保指定组。 如果不添加组，则会添加默认项目组，并在Frame.io中的相应默认团队下创建Frame.io中的项目。

继续下一部分。

![模板组](assets/template-group.png)

### 添加任务并分配启用了Frame.io的用户

1. 在左侧面板中，单击&#x200B;**模板任务**。
1. 单击&#x200B;**开始添加模板任务**&#x200B;以快速将任务添加到模板。 您可以稍后配置其他设置。

   或

   单击&#x200B;**新建模板任务**&#x200B;以一次添加一个任务并配置其他设置。
   ![将任务添加到模板](assets/add-tasks-to-template.png)
1. 添加任务名称。
1. 在&#x200B;**工作**&#x200B;区域，分配用户或团队。 如果单独或在团队中分配启用了Frame.io的用户，则会授予他们访问Frame.io项目的协作者权限，并通过电子邮件通知他们有关Frame.io项目中的任务的信息。 从该电子邮件中，他们可以加入Frame.io项目并开始工作。
1. 根据需要重复步骤1和2。

继续下一部分。

### 配置其他模板详细信息

Workfront具有强大的项目管理功能。 我们建议使用[编辑项目模板](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)文章来配置模板的以下区域：

* 概述
* 财务
* 自定义表单
* 项目设置
* 任务设置
* 问题设置
* 访问

### 从模板创建项目

创建模板后，即可将其用于创建项目。

{{step1-to-projects}}

1. 单击&#x200B;**从模板新建项目**。
1. 使用搜索框，开始键入所需模板的名称。
1. 选择模板名称，然后单击&#x200B;**使用模板**。
   ![查找您的模板](assets/find-your-template.png)
1. 根据需要调整任何项目设置，然后单击&#x200B;**创建项目**。
1. 在左侧面板中，单击&#x200B;**文档**。
1. 使用单向同步文件夹可自动与Frame.io共享创意素材。 [!BADGE 即将推出]{type=Informative}

   >[!NOTE]
   >
   >此功能目前正在开发中。 要与Frame.io中的用户共享信息，请将文件上传到“文档”选项卡。 当项目的状态设置为“当前”时，这些文件会自动推送到Frame.io。

1. 在项目标头中，将项目从&#x200B;**计划**&#x200B;更改为&#x200B;**当前**。

创建项目并创意人员上传已完成的资源后，您可以在Workfront中为该资源分配一个审阅和批准工作流。 有关详细信息，请参阅[创建文档审阅或审批请求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。<!-- name may need to change -->

## 从头开始创建新项目

您可以根据需要从头开始创建新项目。

>[!IMPORTANT]
>
>* Frame.io中的项目由连接到Workfront组的团队组织。 我们建议使用项目模板来创建连接的项目，因为您之前可以设置项目组。
>
>
>* 如果选择从头开始创建项目，Workfront会自动添加默认项目组，并在Frame.io中的该默认团队下创建镜像Frame.io项目。
>
>在创建项目后更新组不会更改Frame.io团队。

### 创建项目

{{step1-to-projects}}

1. 单击&#x200B;**新建项目**。
1. 键入项目的名称，然后按&#x200B;**Enter**&#x200B;保存该名称。

继续下一部分。

### 添加任务并分配启用了Frame.io的用户

1. 在左侧面板中，单击&#x200B;**任务**。
1. 单击&#x200B;**开始添加任务**&#x200B;以快速将任务添加到您的项目。 您可以稍后配置其他设置。

   或

   单击&#x200B;**新建任务**&#x200B;以一次添加一个任务并配置其他设置。
   ![新任务](assets/add-project-tasks.png)
1. 添加任务名称。
1. 在&#x200B;**工作**&#x200B;区域，分配用户或团队。 如果单独或在团队中分配启用了Frame.io的用户，则会授予他们访问Frame.io项目的协作者权限，并通过电子邮件通知他们有关Frame.io项目中的任务的信息。 从该电子邮件中，他们可以加入Frame.io项目并开始工作。
1. 根据需要重复步骤1和2。

继续下一部分。

### 上传创意资料

1. 在左侧面板中，单击&#x200B;**文档**。
1. 使用单向同步文件夹可自动与Frame.io共享创意素材。 [!BADGE 即将推出]{type=Informative}

   >[!NOTE]
   >
   >此功能目前正在开发中。 要与Frame.io中的用户共享信息，请将文件上传到“文档”选项卡。 当项目的状态设置为“当前”时，这些文件会自动推送到Frame.io

继续下一部分。

### 配置其他项目详细信息

Workfront具有强大的项目管理功能。 我们建议使用[编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)文章来配置项目的以下方面：

* 概述
* 财务
* 自定义表单
* 项目设置
* 任务设置
* 问题设置
* 访问

### 将项目设置为当前项目

1. 在项目标题中，将项目从“计划”更改为“当前”。
创建项目并创意人员上传已完成的资源后，您可以在Workfront中为该资源分配一个审阅和批准工作流。

创建项目并创意人员上传已完成的资源后，您可以在Workfront中为该资源分配一个审阅和批准工作流。

有关详细信息，请参阅[创建文档审阅或审批请求](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)。<!-- name may need to change -->
