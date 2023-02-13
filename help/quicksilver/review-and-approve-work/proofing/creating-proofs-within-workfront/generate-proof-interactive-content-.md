---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 在ZIP文件中为交互式内容创建校样
description: 您可以为存储在ZIP文件中的非网站交互式内容生成校样。 此类Web内容的示例包括带有流视频或音频的广告、HTML动画、交互式横幅。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# 在ZIP文件中为交互式内容创建校样

您可以为存储在ZIP文件中的非网站交互式内容生成校样。 此类Web内容的示例包括带有流视频或音频的广告、HTML动画、交互式横幅。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
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

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 在ZIP文件中为交互式内容创建校样

在将ZIP文件中的交互式内容添加到校样后，Adobe Workfront会创建压缩文档的校样。 根据文件大小，上传加载时间可能会有所不同。 创建较大的文件需要更长的时间。 您可以从页面中导航到其他位置，Workfront将继续创建您的文件。 最大文件上传大小为4 GB。 

1. 通过创建捆绑的ZIP文件来准备内容。

   ZIP文件必须满足以下要求：

   * 包文件中应包含所有资产，如CSS、JavaScript、视频、声音和图像。
   * 确保主文件（如index.html、index.htm）位于根文件夹中，并且它是存储在该根文件夹中的唯一.html/.htm文件。

      如果主文件未放在根文件夹中，则Workfront会搜索该文件夹以查找主文件。

   * 最大包大小为500 MB。
   * 对于在iOS中创建的ZIP文件，该工具会自动标识放置内容的正确文件夹。

1. 转到要上传ZIP文件的项目、任务或问题。
1. 单击 **文档** 中。
1. 单击 **新增**，然后单击&#x200B;**校样** 中。
1. 在 **添加文件** ，拖放或浏览所需的ZIP文件。
1. 单击 **创建校样** 创建简单的校样，而不进行审核过程。\
   或\
   继续配置高级校样：

   * [使用基本工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
