---
product-area: documents
navigation-topic: approvals
title: 为内容查看者创建和管理品牌
description: 为内容查看者创建和管理品牌
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: f89b6edead9dce1b0b4baa5ac792cf5e56fd46c0
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 3%

---

# 为内容查看者创建和管理品牌

{{highlighted-preview-article-level}}

内容审核者在审核过程中使用品牌指南评估内容。 您可以通过上传包含品牌指南的PDF文件或手动输入品牌元素，在Workfront中创建品牌。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是系统管理员。</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Admin Console权限*</td> 
   <td> <p>您必须是GenStudio品牌经理。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 要求

* 您的Workfront实例必须启用统一批准。

* 您的组织必须具有GenStudio Foundation。
   * Workfront中的内容审阅者提供了GenStudio Foundation中用于资源审阅和批准工作流的功能。 您无需直接访问GenStudio Foundation即可完成工作。 您通过Content Reviewer访问GenStudio Foundation功能是受Workfront合同条款约束的。
* Adobe必须有一个已签署的Adobe Gen AI协议文件。
有关签署协议的更多信息，请参阅[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。


## 先决条件

1. 在创建品牌之前，您必须先在Admin Console和Workfront访问级别中授予对品牌权限的访问权限。 有关说明，请参阅[授予对品牌权限的访问权限](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)。


## 使用PDF创建品牌

{{step-1-to-setup}}

1. 在左侧面板中，转到&#x200B;**审核和批准** > **品牌**。
1. 单击屏幕右上角的&#x200B;**添加品牌**。
1. 为品牌命名。
1. 单击&#x200B;**上传PDF**以上传品牌文件。
   ![上载品牌PDF](assets/upload-PDF.png)
1. 单击&#x200B;**继续**。
1. 上载一个或多个包含品牌指南的PDF文件，然后单击&#x200B;**添加品牌**。
1. 上传文件后，请查看提取的品牌元素，确保它们符合您的品牌准则。

   >[!IMPORTANT]
   >
   >准则是使用您的文件和创作AI技术生成的，可能不准确。 查看提取的准则以了解缺少或不正确的详细信息，并在发布此品牌之前编辑它们。

1. 完成后，单击&#x200B;**发布**&#x200B;以使该品牌可供内容查看者使用。

## 手动创建品牌

{{step-1-to-setup}}

1. 在左侧面板中，转到&#x200B;**审核和批准** > **品牌**。
1. 单击屏幕右上角的&#x200B;**添加品牌**。
1. 为品牌命名。
1. 单击&#x200B;**手动添加**&#x200B;以创建包含单个元素的品牌。
1. 根据需要填写品牌详细信息。 您可以添加以下元素：

   <table>
    <tr>
        <td>使用时间</td>
        <td>让营销人员知道何时使用此品牌。</td>
    </tr>
    <tr>
        <td>语音准则</td>
        <td>提供有关品牌声音的语调和风格的指导。</td>
    </tr>
    <tr>
        <td>图像准则</td>
        <td>指定与品牌标识一致的图像类型。</td>
    </tr>
    <tr>
        <td>渠道准则</td>
        <td>概述品牌交流的适当渠道。</td>
    </tr>
    <tr>
        <td>徽标</td>
        <td>包括与品牌关联的官方徽标。</td>
    </tr>
    <tr>
        <td>颜色</td>
        <td>指定品牌的调色板。</td>
    </tr>
    </table>

   ![手动添加品牌元素](assets/brand-elements.png)


1. 完成后，单击&#x200B;**发布**&#x200B;以使该品牌可供内容查看者使用。


## 编写品牌指南的最佳实践

*  编写描述可衡量标准的品牌指南。 内容审核者按字面意思对内容进行评估，因此客观规则会生成比主观规则更一致的分数。

* 在您的指南中查找“避免”、“保留”或“确保”等单词。 这些通常表示您可以收紧的规则。 将vague指令替换为单词、格式或限制的特定列表。 例如，将“避免常见的滑雪陈词滥调”替换为“不要使用‘gnar’、‘pow’或‘shred’”。

* 如果不能消除主观性，请缩小其范围。 将宽泛的形容词替换为特定的约束。 例如，“直接和行动导向”变为“直接和行动导向；省略空话和套期保值语言”。