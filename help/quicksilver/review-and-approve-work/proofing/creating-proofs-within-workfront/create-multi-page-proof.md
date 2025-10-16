---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 创建多页验证
description: 您可以将多个文件合并到单个多页验证中。 查看者可以使用验证查看者中的导航工具来浏览多页验证中的页面。
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 创建多页验证

您可以将多个文件合并到单个多页验证中。 查看者可以使用验证查看者中的导航工具来浏览多页验证中的页面。

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
    <p>工作或计划</p> </td> 
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

## 创建多页验证

启用此选项后，静态文件和网站在单个验证中可用。 禁用此选项后，所有文档和网站都将生成为单独的校样，您最多可以在给定时间上传100个文件。

要创建多页验证，请执行以下操作：

1. 转到要验证的项目、任务或问题，然后单击&#x200B;**文档**&#x200B;部分。
1. 单击&#x200B;**新增** > **校对**。
1. 拖放文件或浏览并从文件资源管理器中选择它们。 您一次最多可以上传50个文件。 有关文件限制的信息，请参阅本文中的[注意事项](#considerations)部分。

   >[!NOTE]
   >
   >交互式文件（包括视频和交互式网站）无法合并为单个验证。

1. 在&#x200B;**单个校对**&#x200B;下，启用选项&#x200B;**将所有兼容的文件合并为单个校对**。
1. 在&#x200B;**校对名称**&#x200B;字段中，为组合校对指定新名称。
1. （可选）在您上载的文件列表中，通过拖动文件来重新排序文件。 文件的顺序是组合验证的页面顺序。
1. （可选）要从“新建验证”页面中删除单个文件，请将鼠标悬停在该文件上，然后单击右侧显示的&#x200B;**垃圾桶**&#x200B;图标。

   或

   要一次删除所有已上传的文件，请单击列表右上角的&#x200B;**全部删除**。

1. 上传所有文件后，您必须决定是配置基本验证还是自动验证：

   * 使用基本验证，您可以添加所需数量的审阅人，但他们不会归为多个阶段。 您添加的所有审阅人可以在您创建验证后立即访问该验证。 要配置基本验证，请参阅[使用基本工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)。
   * 借助自动验证，验证会从一个阶段移动到另一个阶段，Adobe Workfront会通知每个用户何时需要查看它。 要配置自动验证，请参阅[使用自动工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)。

## 注意事项 {#considerations}

将文件组合到单个验证中时，请考虑以下事项：

* 您最多可以上传500个单独的文件。
* 您可以合并各种类型的静态文件(例如，PDF、JPG、DOC、PPT、EXC)，最多可达2,000页。
* 您可以组合静态Web捕获。
* 您可以合并GIF文件；但是，动画GIF会作为静态文件处理。
* 无法将AV文件与交互式Web捕获结合使用。
* 校样的缩略图图像是从校样的首页获取的(请参阅[在Workfront Proof中管理校样详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md))。
* 您可以在验证详细信息页面上检查合并以创建验证的文件名称。 有关详细信息，请参阅[在Workfront Proof中管理校对详细信息](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)。
* 如果验证上启用了下载原始文件的选项，则您可以下载已合并的所有文件，以将验证创建为.zip文件。 有关更多信息，请参阅  [下载存储在Workfront Proof中的文件](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md)。
