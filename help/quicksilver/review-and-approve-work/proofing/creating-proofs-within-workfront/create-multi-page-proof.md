---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 创建多页校样
description: 您可以将多个文件合并到单个多页校样中。 审阅人可以使用校对查看器中的导航工具来浏览多页面校样中的页面。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# 创建多页校样

您可以将多个文件合并到单个多页校样中。 审阅人可以使用校对查看器中的导航工具来浏览多页面校样中的页面。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 创建多页校样

启用此选项后，静态文件和网站可通过单个校样使用。 禁用此选项后，所有文档和网站都将作为单个校样生成，并且您在给定时间最多可上传100个文件。

要创建多页校样，请执行以下操作：

1. 转到要校样的项目、任务或问题，然后单击 **文档** 中。
1. 单击 **新增** > **校样** .
1. 拖放文件或浏览并从文件资源管理器中选择它们。 您一次最多可以上传50个文件。 有关文件限制的信息，请参阅 [注意事项](#considerations) 章节。

   >[!NOTE]
   >
   >交互式文件（包括视频和交互式网站）不能合并为单个校样。

1. 在 **单次校样**，启用选项， **将所有兼容的文件合并到单个校样中**.
1. 在 **校样名称** 字段，为组合校样指定新名称。
1. （可选）在已上传的文件列表中，通过拖动文件来重新排序。 文件的顺序是组合校样的页面顺序。
1. （可选）要从New校样页面中删除单个文件，请将鼠标悬停在该文件上，然后单击 **垃圾** 图标。

   或

   要同时删除所有上传的文件，请单击 **全部删除** 列表右上角。

1. 上传所有文件后，您必须决定要配置基本校样还是自动校样：

   * 通过基本校样，您可以添加任意所需数量的审阅人来进行校样，但这些审阅人并不是分阶段组织的。 您添加的所有审阅人都可以在创建校样后立即访问该校样。 要配置基本校样，请参阅 [使用基本工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * 使用自动校样，校样会从舞台移动到舞台，Adobe Workfront会在每位用户需要进行审阅时通知他们。 要配置自动校样，请参阅 [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 注意事项 {#considerations}

将文件合并到单个校样中时，请考虑以下事项：

* 您最多可以上传500个单独的文件。
* 您最多可以合并不同类型(例如，PDF、JPG、DOC、PPT、EXC)的静态文件，共2,000页。
* 您可以合并静态Web捕获。
* 您可以组合GIF文件；但是，动画GIF会作为静态文件进行处理。
* 不能将AV文件和交互式Web捕获相结合。
* 校样的缩略图图像取自校样的第一页(请参阅 [在Workfront校样中管理校样详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md))。
* 您可以在校样详细信息页面上检查为创建校样而组合的文件名称。 有关更多信息，请参阅 [在Workfront校样中管理校样详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* 如果校样上启用了下载原始文件的选项，则可以下载已合并的所有文件，以将校样创建为.zip文件。 有关更多信息，请参阅  [下载存储在Workfront校样中的文件](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
