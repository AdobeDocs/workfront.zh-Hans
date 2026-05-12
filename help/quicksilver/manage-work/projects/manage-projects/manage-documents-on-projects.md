---
product-area: projects
navigation-topic: manage-projects
title: 项目和相关对象的文档管理概述
description: 根据您的Workfront管理员是否选择将文档存储在旧版Workfront存储或Adobe企业级存储中，具体取决于您的存储首选项默认值。 本文介绍了如何管理项目、项目组合、程序、模板、任务和问题的文档。
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: ccf8af65b9f8ac96a4f9fa2e4dc32a721477375a
workflow-type: tm+mt
source-wordcount: '1830'
ht-degree: 0%

---

# 项目和相关对象的文档管理概述

您的Adobe Workfront管理员可以为贵组织的存储首选项定义默认值，以指示文档应存储在Workfront中的什么位置。

Workfront管理员可以选择以下选项之一：

* Workfront存储
* Adobe企业存储

此首选项允许您自动将附加到Workfront对象的文档存储在某个可用的存储位置。

>[!IMPORTANT]
>
>您的Workfront实例可能无法同时访问Workfront和Adobe存储。 某些Workfront实例仅有权访问Workfront，而其他实例默认仅有权访问Adobe企业存储。 仅访问一种存储类型的客户不需要任何配置。

Workfront管理员可以执行以下操作之一：

* 从两个存储选项中选择一个作为您组织的默认存储选项
* 允许您选择在创建以下对象之一时要使用的存储：

   * 项目
   * 项目组合
   * 模板

有关为Workfront设置存储首选项的信息，请参阅[为您的组织启用Adobe企业存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)。

本文介绍了如何管理项目、项目组合、程序、任务、问题、模板和模板任务的文档。

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## 文档存储概述

客户可以访问以下文档存储功能之一：

* 仅限Workfront存储。 “系统首选项”中的“存储首选项”区域不存在。
* 仅限Adobe企业级存储。 “系统首选项”中的“存储首选项”区域不存在。
* Workfront Storage和Adobe Enterprise Storage。 Workfront管理员可以选择以下选项：

   * 选择默认存储环境，以便将来处理文档。
   * 允许用户选择在创建以下对象时选择的存储：

      * 项目
      * 项目组合
      * 模板

  >[!NOTE]
  >
  >* 任务和问题从项目继承存储类型。
  >* 模板任务从模板继承存储类型
  >* 项目从产品组合中继承存储类型。


存储在Workfront存储中的对象上的文档的管理方式与存储在Adobe企业存储中的文档的管理方式不同。

有关详细信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

以下部分介绍了在同一环境中同时存在Workfront和Workfront企业级存储选项时，文档存储如何用于Adobe对象。

### 项目的文档管理

处理项目时，请考虑以下事项：

* 创建Adobe企业存储项目时，Workfront会在项目的“文档”部分中创建一个用于保存文档的文件夹。 文件夹名称与项目同名。 无法删除或手动重命名文件夹。 如果更改项目名称以匹配项目的新名称，则将重命名文件夹。
* 在创建Adobe企业存储项目或将项目移动到旧版Workfront存储项目组合或项目群时，如果该项目组合或项目群在添加项目之前没有附加文档，则该项目组合或项目群会自动转换为Adobe企业存储对象。
* 您无法为Workfront企业存储产品组合或项目群创建Adobe存储项目。
* 从MS Project导入项目时，Workfront会创建一个Workfront存储项目，即使Workfront管理员将Adobe企业存储设置为系统的默认存储空间也是如此。
* 当您使用Workfront Planning自动化功能创建项目时，Workfront会使用您系统的默认项目存储首选项。 您必须购买Planning包才能访问Workfront Planning。

### 项目组合的文档管理

使用项目组合时，请考虑以下事项：

* 创建Adobe企业存储产品组合时，Workfront会在产品组合的“文档”部分创建一个文件夹来保存文档。 文件夹名称与项目组合同名。 无法删除或手动重命名文件夹。 如果更改项目组合名称以匹配项目组合的新名称，则将重命名文件夹。

* 当您将Adobe存储项目添加到Workfront存储产品组合，并且该产品组合没有附加文档时，该产品组合将转换为Adobe存储产品组合。
* 当您将一个Adobe存储项目添加到Workfront存储产品组合，并且该产品组合具有附加文档时，该产品组合文档存储仍保留在Workfront存储上。 但是，已从产品组合中删除![旧产品组合存储图标](assets/legacy-storage-project-icon.png)的旧版Workfront存储图标。
* 您无法将Workfront-storage项目添加到Adobe-storage产品组合。

* 当您使用Workfront Planning自动化创建项目组合时，Workfront会使用您系统的项目组合默认存储偏好设置。 您必须购买Planning包才能访问Workfront Planning。

### 方案的文档管理

使用程序时，请考虑以下事项：

* 创建Adobe企业存储程序时，Workfront会在程序的“文档”部分创建一个文件夹，用于保存文档。 文件夹名称与项目的名称相同。 无法删除或手动重命名文件夹。 如果更改项目名称，将重命名文件夹，以匹配项目的新名称。

* 将Adobe存储项目添加到Workfront存储项目时，如果该项目没有附加任何文档，则该项目会转换为Adobe存储项目。
* 当您将一个Adobe存储项目添加到Workfront存储项目群时，而该项目群具有附加的文档，则该项目群文档存储仍保留在Workfront存储中。 但是，程序![旧版项目组合存储图标](assets/legacy-storage-project-icon.png)的旧版Workfront存储图标已从程序中删除。
* 您无法将Workfront-storage项目添加到Adobe-storage程序。

* 当您使用Workfront Planning自动化创建程序时，Workfront会使用您系统的默认程序存储首选项。 您必须购买Planning包才能访问Workfront Planning。

### 任务的文档管理

处理任务时，请考虑以下事项：

* 任务从项目继承存储类型。
* 在将文档上传到Adobe存储项目上的任务时，Workfront会自动在任务的“文档”部分创建文件夹。 文件夹名称与任务相同。
* 您可以从Adobe企业存储任务中重命名和删除文档文件夹，这也会删除文件夹中的文档。 将新文档添加到任务后，会自动重新创建文件夹。 已删除的文档不会放回文件夹中。
* 对于Adobe企业存储项目，任务中的文档文件夹显示为自动为项目创建的文档文件夹中的子文件夹。
* 您无法将任务从Workfront存储项目复制或移动到Adobe存储项目。 反之亦然。
* 将任务转化为项目时，存在以下情况： <!--this info also duplicated in Convert tasks to projects-->
   * Workfront存储任务创建Workfront存储项目。
   * Adobe企业存储任务将创建一个Adobe存储项目。
   * 使用Workfront-storage模板转换Adobe-storage任务会创建一个Adobe-storage项目。
   * 使用Adobe-storage模板转换Workfront-storage任务会创建一个Workfront-storage项目。
* 无法在“摘要”面板中将文档添加到Adobe存储任务。

### 问题的文档管理

处理问题时请考虑以下事项：

* 从项目继承存储类型时出现问题。
* 当您将文档上传到Adobe存储项目中的问题时，Workfront会自动在问题的“文档”部分创建文件夹。 文件夹名称与问题相同。
* 您可以重命名文档文件夹，并将其从Adobe企业存储问题中删除，这也会删除文件夹中的文档。 在将新文档添加到问题中后，会自动重新创建文件夹。 已删除的文档不会放回文件夹中。
* 对于Adobe企业存储项目，问题中的文档文件夹显示为自动为项目创建的documents文件夹中的子文件夹。
* 您无法将问题从Workfront存储项目复制或移动到Adobe存储项目。 反之亦然。
* 当您提交带有附加到Workfront存储项目的文档的请求时，该请求的“文档”区域将使用项目的存储类型显示文档，即使系统存储默认首选项为Adobe企业也是如此。
* 将问题转化为项目时，存在以下情况：<!--this info also duplicated in Convert an issue to a project-->
   * 出现Workfront存储问题，会创建一个Workfront存储项目。
   * Adobe企业存储问题会创建一个Adobe存储项目。
   * 使用Workfront-storage模板转换Adobe-storage问题会创建一个Adobe-storage项目。
   * 使用Adobe-storage模板转换Workfront-storage问题会创建一个Workfront-storage项目。
* 无法在“摘要”面板中将文档添加到Adobe存储问题。

### 项目模板的文档管理

使用模板时，请考虑以下事项：

* 创建Adobe企业存储模板时，Workfront会在模板的“文档”部分中创建一个用于保存文档的文件夹。 文件夹名称与程序同名。 无法删除或手动重命名文件夹。 如果更改了模板的名称，将重命名文件夹，以匹配模板的新名称。
* 可以使用Workfront-storage模板创建Workfront-storage项目；可以使用Adobe-storage模板创建Adobe-storage项目。
* 您可以将Workfront-storage模板附加到Adobe-storage项目，这不会更改该项目的存储位置。
* 您可以将Adobe-storage模板附加到Workfront-storage项目，这不会更改该项目的存储位置。 模板的Adobe-storage文件夹中的文档直接添加到项目中，而不是文件夹，而模板任务文件夹中的文档添加到附加到任务的“文档”部分中的项目任务的文件夹中。

### 模板任务的文档管理

处理模板任务时，请考虑以下事项：

* 模板任务从模板继承存储类型。
* 当您在Adobe存储模板上向模板任务上传文档时，Workfront会自动在模板任务的“文档”部分创建文件夹。 文件夹名称与模板任务相同。
* 您可以从Adobe企业存储模板任务中重命名和删除文档文件夹，这也会删除文件夹中的文档。 将新文档添加到模板任务后，会自动重新创建文件夹。 已删除的文档不会放回文件夹中。
* 对于Adobe企业存储模板，模板任务上的文档文件夹显示为自动为模板创建的文档文件夹上的子文件夹。
* 您不能将模板任务从Workfront存储模板复制或移动到Adobe存储模板。 反之亦然。
* 当您向与Adobe存储相关联的“请求队列”中提交的问题附加文档时，将为每个提交的问题创建一个文件夹以存储文档。 该文件夹还将作为子文件夹添加到请求队列中自动创建的项目文件夹中。
