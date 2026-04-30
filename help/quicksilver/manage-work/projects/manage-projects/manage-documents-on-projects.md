---
product-area: projects
navigation-topic: manage-projects
title: 项目和相关对象的文档管理概述
description: 根据您的Workfront管理员是否选择将文档存储在旧版Workfront存储或Adobe企业级存储中，具体取决于您的存储首选项默认值。 本文介绍了如何管理项目、项目组合、程序、模板、任务和问题的文档。
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 5c4ffeabf710374b14a2335b47342be4c393a7c8
workflow-type: tm+mt
source-wordcount: '1422'
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
>并非所有客户都可以同时访问Workfront和Adobe存储。 某些客户只能访问Workfront，而其他客户在默认情况下只能访问Adobe企业存储。 如果客户没有权限访问Workfront存储，则无需进行配置。

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


存储在Workfront存储中的对象上的文档的管理方式与Adobe企业级存储中的文档的管理方式不同。

有关详细信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

以下部分介绍了当Workfront和Workfront企业级存储选项都就绪后，文档存储如何用于Adobe对象。

### 项目的文档管理

处理项目时，请考虑以下事项：

* 创建Adobe企业存储项目时，Workfront会在项目的“文档”部分中创建一个用于保存文档的文件夹。 文件夹名称与项目同名。 无法删除或手动重命名文件夹。 如果更改项目名称以匹配项目的新名称，则将重命名文件夹。
* 在创建Adobe企业存储项目或将项目移动到旧版Workfront存储产品组合或项目群时，该项目组合或项目群会自动转换为Adobe企业存储对象。
* 您无法为Workfront企业存储产品组合或项目群创建Adobe存储项目。

### 项目组合的文档管理

使用项目组合时，请考虑以下事项：

* 创建Adobe企业存储产品组合时，Workfront会在产品组合的“文档”部分创建一个文件夹来保存文档。 文件夹名称与项目组合同名。 无法删除或手动重命名文件夹。 如果更改项目组合名称以匹配项目组合的新名称，则将重命名文件夹。
* 在创建Adobe企业级存储项目或将项目移动到旧版Workfront存储产品组合时，该项目组合会自动转换为Adobe企业级存储对象。
* 如果转换后的产品组合以前附加过文档，则这些文档将继续存储在Workfront存储中。 新文档还存储在Workfront存储中。
* 如果转换后的产品组合没有在Workfront存储中附加文档，则新文档将存储在Adobe企业存储中。

### 方案的文档管理

使用程序时，请考虑以下事项：

* 创建Adobe企业存储程序时，Workfront会在程序的“文档”部分创建一个文件夹，用于保存文档。 文件夹名称与程序同名。 无法删除或手动重命名文件夹。 如果更改项目名称，将重命名文件夹，以匹配项目的新名称。
* 在创建Adobe企业级存储项目或将项目移动到旧版Workfront存储产品组合时，该项目组合会自动转换为Adobe企业级存储对象。
* 如果转换后的程序以前附加过文档，则这些文档将继续存储在Workfront存储中。 新文档还存储在Workfront存储中。
* 如果转换后的程序未在Workfront存储中附加任何文档，则新文档将存储在Adobe企业存储中。

### 任务的文档管理

处理任务时，请考虑以下事项：

* 任务从项目继承存储类型。
* 在将文档上传到Adobe存储项目上的任务时，Workfront会自动在任务的“文档”部分创建文件夹。 文件夹名称与任务相同。
* 您可以从Adobe企业存储任务中重命名和删除文档文件夹，这也会删除文件夹中的文档。 将新文档添加到任务后，会自动重新创建文件夹。 已删除的文档不会放回文件夹中。
* 对于Adobe企业存储项目，任务中的文档文件夹显示为自动为项目创建的文档文件夹中的子文件夹。
* 您无法将任务从Workfront存储项目复制或移动到Adobe存储项目。 反之亦然。

### 问题的文档管理

处理问题时请考虑以下事项：

* 从项目继承存储类型时出现问题。
* 当您将文档上传到Adobe存储项目中的问题时，Workfront会自动在问题的“文档”部分创建文件夹。 文件夹名称与问题相同。
* 您可以重命名文档文件夹，并将其从Adobe企业存储问题中删除，这也会删除文件夹中的文档。 在将新文档添加到问题中后，会自动重新创建文件夹。 已删除的文档不会放回文件夹中。
* 对于Adobe企业存储项目，问题中的文档文件夹显示为自动为项目创建的documents文件夹中的子文件夹。
* 您无法将问题从Workfront存储项目复制或移动到Adobe存储项目。 反之亦然。

### 项目模板的文档管理

使用模板时，请考虑以下事项：

* 创建Adobe企业存储模板时，Workfront会在模板的“文档”部分中创建一个用于保存文档的文件夹。 文件夹名称与程序同名。 无法删除或手动重命名文件夹。 如果更改了模板的名称，将重命名文件夹，以匹配模板的新名称。
* 可以使用Workfront-storage模板创建Workfront-storage项目；可以使用Adobe-storage模板创建Adobe-storage项目。
* 您可以将Workfront-storage模板附加到Adobe-storage项目，这不会更改该项目的存储位置。
* 您可以将Adobe-storage模板附加到Workfront-storage项目，这不会更改该项目的存储位置。

### 模板任务的文档管理

处理模板任务时，请考虑以下事项：

* 模板任务从模板继承存储类型。
* 当您在Adobe存储模板上向模板任务上传文档时，Workfront会自动在模板任务的“文档”部分创建文件夹。 文件夹名称与模板任务相同。
* 您可以从Adobe企业存储模板任务中重命名和删除文档文件夹，这也会删除文件夹中的文档。 将新文档添加到模板任务后，会自动重新创建文件夹。 已删除的文档不会放回文件夹中。
* 对于Adobe企业存储模板，模板任务上的文档文件夹显示为自动为模板创建的文档文件夹上的子文件夹。
* 您不能将模板任务从Workfront存储模板复制或移动到Adobe存储模板。 反之亦然。
* 当您向与Adobe存储相关联的“请求队列”中提交的问题附加文档时，将为每个提交的问题创建一个文件夹以存储文档。 该文件夹还将作为子文件夹添加到请求队列中自动创建的项目文件夹中。
