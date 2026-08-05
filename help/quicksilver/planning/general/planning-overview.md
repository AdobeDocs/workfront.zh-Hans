---
title: Adobe Workfront Planning入门
description: Adobe Workfront Planning是Adobe Workfront的一项附加功能。 您可以创建完全可自定义的工作区，以定义满足企业中每个组织单位需求的工作流。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EXDQUUA9-OKoA8Yj3de1TnanFEgXfKPvP8ksBGChiSI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: c3a155b4-a54b-4a82-a3d2-c8f0f971673e
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
  - id: eb361af2-3e4f-4a79-b5f3-7a344ac5794c
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f8dfa5a4aec4541d885bcc45933488cd1fdefac4
workflow-type: tm+mt
source-wordcount: 1228
ht-degree: 0%

---

# Adobe Workfront Planning入门

<!--

this article is linked to the WF Planning landing page - do not change URL or move it; send the team a new URL after we add the redirects for this page

-->

<!--do not use the snippet for IMPORTANT as it links to this article-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>本文中的信息介绍了Adobe Workfront Planning。 Workfront Planning是独立的产品，或者是Adobe Workfront另外购买的功能。
>
>
>本文包含有关客户同时购买Workfront或Workflow包时Workfront Planning的一般信息。
>
>有关包含Workfront Planning文档的文章的完整列表，请参阅[Adobe Workfront Planning的一般信息和文章索引](/help/quicksilver/planning/planning-information.md)。
>
>有关Workfront Planning作为独立产品的信息，请参阅[Adobe Workfront Planning作为独立产品入门](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)。


## Workfront Planning可用性

<!--
the bullets repeat in the "Access needed for Planning STA" article
-->

当您的组织购买以下Workfront包之一时，即可访问Workfront Planning：

* Workfront Workflow和Workfront Planning一起购买。 组织中的每个用户都有一个Workflow和一个Planning许可证。 这可让所有用户完全访问这两个模块的所有Workfront功能。

* Workfront Workflow适用于贵组织中的每个人，Workfront Planning仅适用于贵组织中的某些用户。 这样，用户就拥有了所有Workflow功能的完全访问权限，而分配了Planning许可证的用户则拥有对Planning功能的更多有限访问权限。

* Workfront Planning作为适用于组织中用户的独立产品。 这样，用户既无法访问任何Workfront工作流功能，也无法访问Planning功能。

有关Planning作为独立产品所包含功能的信息，请参阅[Adobe Workfront Planning作为独立产品入门](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)。

## Adobe Workfront Planning简介

与工作流许可证一起购买时，Adobe Workfront Planning是Adobe Workfront的附加功能。 Workfront Planning的目的是全面了解企业的运营详细信息，并回答工作管理生命周期各阶段的关键业务问题。

Workfront Planning可以回答类似下面的问题：

* 我们在欧洲、中东和非洲地区针对第4季度运行了多少营销活动？
* 并行营销活动之间是否存在任何受众重叠？
* 认识项目目前进展如何？
  <!--* What do the assets look like for a particular campaign? Which of them must still be approved?-->

要回答这些问题，领导力需要一种解决方案，能够全面了解从规划到执行、从交付到结果衡量的每个工作阶段。 目前，各组织拥有一些工具，可以涵盖流程的某些部分，但许多组织没有与工作的所有阶段建立良好的联系，也无法可靠地提供结果。

以下是一些主要功能：

* 解决跨所有阶段和参与工作流程的所有利益相关者管理工作的问题。
* 全面自定义工作流，从决定组织使用哪些对象类型（或记录类型）到配置这些对象如何相互链接。
* 链接到来自其他系统的对象类型，为所有进程创建一致的框架。

## 为Workfront实例中的用户启用Workfront Planning

贵组织购买Workfront Planning包后，作为Workfront管理员，您必须确保满足以下要求才能访问Workfront Planning：

* 将包含Planning的布局模板分配给具有参与者或轻度访问级别的用户。

  默认情况下，标准用户和系统管理员已启用Planning。

  有关详细信息，请参阅[使用布局模板自定义主菜单](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)和[将用户分配给布局模板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)。

* 为用户分配Workfront和Planning许可证以及Workfront Planning权限，以便他们能够在Workfront Planning中查看或创建对象。

  有关授予他人访问权限以及允许他人使用Workfront Planning的更多信息，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。

## Workfront Planning术语

虽然Workfront Planning是Workfront的一部分，但它附带了专有的概念和术语。 在开始为组织设置Workfront计划之前，请确保您熟悉这些概念。

Workfront Planning的框架是完全可自定义的。 您可以创建所有记录类型、其属性以及与其关联的任何字段，以满足贵组织的确切需求。

有关详细信息，请参阅[Workfront规划术语概述](/help/quicksilver/planning/general/planning-terminology.md)。

<!--the content from this section was moved to the article linked above-->

## 找到Adobe Workfront Planning

要找到Adobe Planning，请确保贵组织已获得Workfront Planning的访问权限，且您的系统或组管理员已将Planning区域添加到主菜单。 有关信息，请参阅[Adobe计划访问概述](/help/quicksilver/planning/access/access-overview.md)。

要找到Workfront Planning，请执行以下操作：

1. 登录到Workfront。

{{step1-click-main-menu-shell-only}}

1. 单击&#x200B;**Planning** ![Planning图标](assets/planning-icon.png)。

   Workfront Planning主页将打开。

   ![计划登陆页面管理员](assets/planning-landing-page-admin.png)

   >[!TIP]
   >
   >    您的Workfront管理员可以将Planning区域添加到布局模板中的“选择登陆页面”选项，以便您一登录到Workfront即可打开Planning。 有关信息，请参阅[使用布局模板自定义登陆页面](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)。

1. （视情况而定，可选）如果您是Workfront管理员，请单击以下选项卡之一：
   * **我所在的工作区**：显示您创建的工作区或与您共享的工作区。
   * **其他工作区**：显示系统中的所有其他工作区。

   对于所有其他用户，他们创建或与他们共享的工作区都显示在&#x200B;**工作区**&#x200B;区域中。

1. （可选并推荐）继续执行以下某些操作以构建您的工作结构：

   1. 从头开始或使用模板创建工作区。 有关信息，请参阅[创建工作区](/help/quicksilver/planning/architecture/create-workspaces.md)。

   1. 向新工作区中添加部分。 有关信息，请参阅[编辑工作区](/help/quicksilver/planning/architecture/edit-workspaces.md)。
   1. 重命名新工作区中的现有节。
   1. 将记录类型添加到新工作区。 有关信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   1. 单击记录类型的名称以打开记录类型的页面。 默认情况下，记录类型页面会在“表”视图中打开。

      您还可以创建时间轴或日历视图。 有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

   1. 在表视图中，通过添加行来开始添加记录

      或

      通过添加列开始添加记录字段。

      有关信息，请参阅以下文章：

      * [创建记录](/help/quicksilver/planning/records/create-records.md)
      * [创建字段](/help/quicksilver/planning/fields/create-fields.md)。

## Workfront Planning的其他资源

* [Adobe Workfront Planning的一般信息和文章索引](/help/quicksilver/planning/planning-information.md)：包含有关Workfront Planning文档的所有文章的索引，按关注区域分组。
* [Adobe Workfront Planning作为独立产品入门](/help/quicksilver/planning/planning-sta/planning-sta-overview.md)：有关Workfront Planning的一般信息（作为独立产品购买时）。
* [Adobe Workfront Planning AI助手概述](/help/quicksilver/planning/general/planning-ai-assistant-overview.md)：使用Workfront AI Assistant for Planning，您可以使用命令搜索记录，或者创建、更新和删除记录，并让助手为您完成工作。

  <!--
    >[!NOTE]
    >
    >The Workfront AI Assistant has been temporarily removed and it will be available at a later date.
    -->

* [适用于Workfront Fusion的Adobe Workfront规划模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules)：使用Adobe Workfront规划模块，可以在Workfront规划中发生事件时触发方案。 您还可以创建、读取、更新和删除记录，或对Adobe Workfront Planning帐户执行自定义API调用。 您必须购买额外的许可证才能访问Workfront Fusion。

* [Adobe Workfront Planning API基础知识](/help/quicksilver/planning/general/planning-api-basics.md)： Adobe Workfront Planning API的目标是通过引入通过HTTP运行的REST-ful架构，简化与Planning的生成集成。

* [Adobe Workfront Planning与Adobe GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)：您可以在Workfront Planning的GenStudio工作区中管理GenStudio for Performance Marketing中的记录。 您必须购买GenStudio for Performance Marketing许可证。

* [画布功能板概述](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md)：您可以使用Workfront画布功能板在Workfront的报表中查看Workfront计划信息。 您必须购买Workfront Workflow许可证才能访问画布功能板。


<!--
## Currently available Workfront Planning features
(*****for GA just make a list of what features ARE included in Planning and eliminate the last 2 columns; also update the title of this section*****)

(*****at GA: update the link below to the new place for release notes *****)

For information about new features and when they are released, see [Adobe Workfront Planning release activity for 2024](/help/quicksilver/planning/general/release-activity.md). 

The following features are currently available in Workfront Planning:

* Create workspaces             
* Create record types             
* Create record custom fields             
(************ * Import record types and fields using an Excel or CSV file*****)
          
* Display records in a table view            
* Display records in a timeline view            
* Display records in a calendar view            
* Filter, sort, and group records in a table view
* Filter, group, and color code records in the timeline view
* Filter records in the calendar view 
* Search for records in the table and timeline views             
* Connect records that belong to the same workspace  
* Connect records that belong to different workspaces   
* Connect Workfront Planning records to Workfront projects, programs, portfolios, companies, groups             
* Connect Workfront Planning records to Adobe Experience Manager assets          
    You must have an Adobe Experience Manager Assets license and an integration between AEM Assets and Workfront.
    For information, see [Adobe Workfront for Experience Manager Assets and Assets Essentials: article index](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md). 
* View record information in the Details tab
* View record connections in the Connections tab
* Customize the layout of a record's page             
* Share workspaces             
* Share views             
* Share views publicly with any external resource, even people who are not Workfront users         
* Duplicate views             
* Submit requests to create records            
* Export record details to Word and PDF.
* Add comments to records             
* Receive in-app notifications             
* Receive email notifications             
* Add thumbnails and cover pages to records             
* View the history of changes on a record             
* Rich Text formatting for Paragraph fields             
* Access Planning records from Workfront objects             
* Connect and disconnect Planning records from Workfront objects 
* Create Planning records by submitting a request form            
* Workfront Planning public API             
* Adobe Workfront Planning modules for Adobe Workfront Fusion             
* Workfront Planning AI Assistant
* Reporting on Workfront Planning information
    You can report on Planning information using the Canvas Dashboard. For information, see [Canvas Dashboards overview](/help/quicksilver/reports-and-dashboards/canvas-dashboards/canvas-dashboards-overview.md). 

-->

<!--
<table style="table-layout:auto"> 

|       Feature                                      |     Available now  |     Coming soon   |     In research  |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
|     Create workspaces                              |   ✓                           |                                  |                  |
|     Create record types                |   ✓                           |                                  |                  |
|     Create record custom fields                    |   ✓                           |                                  |                  |
|     Import record types and fields using an Excel  or CSV file                              |                              |           ✓                       |                  |
|     Link records                                   |   ✓                           |                                  |                  |
|     View records in a table                        |   ✓                           |                                  |                  |
|     View records in a timeline                     |   ✓                           |                                  |                  |
|     View records in a calendar                     |   ✓                           |                                  |                  |
|     Filter records                                 |   ✓                           |                                  |                  |
|     Group records in the timeline view             |   ✓                           |                                  |                  |
|     Group records in the table view                | ✓                              |                                 |                  |
|     Sort records in the table view                                 |  ✓                             |                                 |                  |
|     Sort records in the timeline view                                 |                               |   ✓                              |                  |
|     Sort groupings in the table view                                 |                               |   ✓                              |                  |
|     Sort groupings in the timeline view                                 |                               |   ✓                              |                  |
|   Search for records in the table view    | ✓    |   |
|   Search for records in the timeline view    | ✓    |   |
|     Connect Workfront Planning records to Workfront projects, programs, portfolios, companies, groups  |   ✓                            |                                 |                  |
|     Connect Workfront Planning records to Adobe Experience Manager assets                                  |      ✓                         |                                  |                 |
|     Connect Planning records from different workspaces                                  |      ✓                         |                                  |                 |
|     Record page with detailed information                            |   ✓                           |                                  |                  |
|     Update the layout of the record's page              |    ✓                           |                                 |                  |
|  Share workspaces | ✓| |  |
|  Share views |✓ | |  |
|  Share views publicly with external resources |✓ | |  |
|  Duplicate views |✓ | |  |
|     Submit requests                                |                               |          ✓                        |                 |
|     Export record details to Word                                 |    ✓                           |                                  |                 |
|     Export record details to PDF                                 |                               |                                  |       ✓          |
|     Customize the color and icon of a record                                 |      ✓                         |                                  |                 |
|     Add comments to records                                 | ✓                              |                                  |                 |
|     Receive in-app notifications                                 | ✓                              |                                  |                 |
|     Receive email notifications                                 | ✓                              |                                  |                 |
|     Add thumbnails to records                                 | ✓                              |                                  |                 |
|     View history of changes on a record                                 | ✓                              |                                  |                 |
|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 |
|     Adobe Workfront Planning modules for Adobe Workfront Fusion                                 |      ✓                         |                                  |                 |
|     Copy and paste information from one field to another                                  |      ✓                         |                                  |                 |
|     Access Planning records from Workfront objects                                  |      ✓                         |                                  |                 |
|     Connect Planning records from Workfront objects                                  |      ✓                         |                                  |                 |
|     Workfront Planning public API                                 |      ✓                         |                                  |                 |
|     Workfront Planning AI Assistant*                                 |      ✓                         |                                  |                 |
|     Reporting on Workfront Planning information (Canvas Dashboard)                              |                               |       ✓                           |                 |
</table>

-->