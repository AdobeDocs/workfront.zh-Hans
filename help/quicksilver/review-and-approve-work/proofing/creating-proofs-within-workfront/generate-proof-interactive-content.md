---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 在ZIP文件中为交互式内容创建验证
description: 您可以为存储在ZIP文件中的非网站交互式内容生成验证。 此类网络内容的示例包括带有流视频或音频的广告、HTML动画、交互式横幅。
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# 在ZIP文件中为交互式内容创建验证

您可以为存储在ZIP文件中的非网站交互式内容生成验证。 此类网络内容的示例包括带有流视频或音频的广告、HTML动画、交互式横幅。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>标准</p>
   <p>工作或计划</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在ZIP文件中为交互式内容创建验证

一旦您在ZIP文件中将交互式内容添加到验证中，Adobe Workfront就会创建压缩文档的验证。 上传加载时间因文件大小而异。 创建较大的文件需要较长时间。 您可以离开页面，Workfront将继续创建您的文件。 最大文件上传大小为4GB。 

1. 通过创建ZIP捆绑文件来准备内容。

   ZIP文件必须满足以下要求：

   * 捆绑包文件中应包含所有资源，如CSS、JavaScript、视频、声音和图像。
   * 确保主文件（如index.html、index.htm）位于根文件夹中，并且它是唯一存储在该文件夹中的.html/.htm文件。

     如果主文件未放在根文件夹中，Workfront会搜索该文件夹以查找主文件。

   * 最大包大小为500 MB。
   * 对于在iOS中创建的ZIP文件，此工具会自动标识放置内容的正确文件夹。

1. 转到要上传ZIP文件的项目、任务或问题。
1. 单击左侧面板中的&#x200B;**文档**。
1. 单击“新增”****，然后在出现的菜单中单击“校对”****。
1. 在&#x200B;**添加文件**&#x200B;部分中，拖放或浏览所需的ZIP文件。
1. 单击&#x200B;**创建校对**&#x200B;以创建无审阅过程的简单校对。\
   或\
   配置高级校对以继续：

   * [使用基本工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
