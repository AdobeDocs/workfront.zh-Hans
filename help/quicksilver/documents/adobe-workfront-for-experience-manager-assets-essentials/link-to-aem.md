---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 将内容和文件夹链接到由Experience Manager Assets提供支持的Content Advisor
description: 您可以使用内容审查程序将Experience Manager Assets中的内容或文件夹链接到任何支持文档的Adobe Workfront对象。 Content Advisor将智能、上下文感知的发现直接引入Workfront，帮助您快速找到相关、经批准的内容。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 2%

---

# 将内容和文件夹与Experience Manager Assets的内容审查程序链接

Content Advisor将智能的上下文感知发现直接引入Workfront，帮助您根据上下文快速找到相关的经批准内容。 借助智能建议、Dynamic Media演绎版和详细资产元数据等功能，您可以在不离开Workfront的情况下高效地评估和重用内容，从而加快内容创建，同时保持品牌一致性。

您可以使用内容审查程序将内容和文件夹从Experience Manager Assets链接到Workfront。 链接后，您可以在Workfront中查看和管理内容，对Experience Manager Assets中的内容所做的任何更改都将反映在Workfront中。

>[!IMPORTANT]
>
>如果贵组织拒绝签署GenAI Rider协议，您仍可以使用Content Advisor在Experience Manager Assets中选择资源和文件夹，但您将无法访问由AI支持的功能，例如AI 搜索、智能建议或分析活动简报。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p> “任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可证</td> 
   <td> 
   <p>参与者或更高版本</p> 
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他产品</td> 
   <td>您必须安装了Experience Manager as a Cloud Service或Assets Essentials，并且您必须作为用户添加到Admin Console的产品中。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager权限</td> 
    <td>您必须具有此文件夹的写入权限。</td> 
   </tr>
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看访问权限或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

开始之前：

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)。

* 要使用Smart建议或Campaign Briefs功能，您必须签署GenAI Rider。 有关详细信息，请参阅[使用内容审查程序访问Adobe应用程序中的AEM内容](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)。



## 将Experience Manager Assets中的内容与内容审查程序链接到一起

现在，您可以使用内容审查程序直接在Workfront中链接Experience Manager Assets中的内容。 内容审查程序不适用于Assets Essentials。

要链接内容，请执行以下操作：

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 选择&#x200B;**新增**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets。

1. 使用内容审查程序，您可以：


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>使用AI 搜索搜索资源。</strong>使用AI支持的搜索，该搜索理解查询背后的含义和意图，支持多种语言、拼写错误和同义词。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">更智能的资源发现AI 搜索</a>。</td>
      </tr>
      <tr>
         <td><strong>根据上下文和意图查看智能建议。</strong>使用宿主Adobe应用程序中的上下文感知推荐，查找与您的内容需求相符的资源。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">基于上下文和意图的智能建议</a>。</td>
      </tr>
      <tr>
         <td><strong>上传营销活动简报以发现相关资源。</strong>上传PDF、DOCX或TXT营销活动简介文档，以便内容顾问分析该文档并推荐相关资源。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">发现相关资产的Campaign简介</a>。</td>
      </tr>
      <tr>
         <td><strong>查看和选择Dynamic Media资源演绎版。</strong>浏览渠道优化演绎版（包括图像预设、智能裁剪和格式类型），并应用Dynamic Media修饰符实时预览调整。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的Dynamic Media资源演绎版</a>。</td>
      </tr>
      <tr>
         <td><strong>将Dynamic Media修饰符应用于演绎版。</strong>添加修饰符以实时转换资源演绎版，并在为主机应用程序选择演绎版之前预览结果。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的Dynamic Media资源演绎版</a>。</td>
      </tr>
      <tr>
         <td><strong>发现和浏览内容片段。</strong>搜索内容片段，查看实时缩略图预览，检查状态（草稿、已修改或已发布），并检查详细的属性、引用和变量。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">发现内容片段</a>。</td>
      </tr>
      <tr>
         <td><strong>访问资源元数据。</strong>查看与Assets视图一致的资源属性，如标题、描述、格式、大小和其他元数据选项卡（产品、营销活动、标记）。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">访问与Assets视图一致的资源元数据</a>。</td>
      </tr>
      <tr>
         <td><strong>使用预定义筛选器筛选资源。</strong>使用文件类型、文件格式、资源状态、文件大小、图像宽度、图像高度、修改日期和创建日期等过滤器优化资源结果。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">与Assets视图一致的访问筛选器</a>。</td>
      </tr>
      <tr>
         <td><strong>保存并重用搜索。</strong>通过指定搜索词和筛选器选项创建保存的搜索，然后在Experience Manager Assets和其他Adobe应用程序中重复使用它们。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">访问和重复使用最近和保存的搜索</a>。</td>
      </tr>
      <tr>
         <td><strong>在收藏集间和收藏集中搜索资源。</strong>在所有收藏集中搜索资源或收藏集，或限制仅搜索特定收藏集。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">在收藏集间和收藏集中搜索资产</a>。</td>
      </tr>
   </tbody>
   </table>


### 将Experience Manager Assets中的新版本与内容审查程序链接到一起

您可以从Experience Manager Assets或Assets Essentials拉取新内容，并将其作为新版本添加到现有资源。 如果文档已链接，并且在Experience Manager Assets或Assets Essentials中添加了新版本，则新版本会自动显示在Workfront中。

要链接新版本，请执行以下操作：

1. 转到Workfront中要添加文档的&#x200B;**文档**&#x200B;区域。
1. 选择要替换为新版本的资产。 您无法在链接的文件夹中创建资产的新版本。
1. 选择&#x200B;**新增** > **版本**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets。

1. 选择要链接的内容：

   * 选择“Assets”选项卡以浏览Experience Manager Assets或Assets Essentials中的资源、文件夹或收藏集。

     ![内容顾问](assets/content-advisor-full.png)

   * 内容片段不支持版本。 如果您选择内容片段，新版本将替换现有的内容片段，而不是创建新版本。

1. 单击&#x200B;**选择**。

## 将Experience Manager Assets中的文件夹与内容审查程序链接到一起

查看文件夹中各个资产的权限取决于Experience Manager Assets权限。

链接文件夹：

1. 转到Workfront中要放置文件夹的&#x200B;**文档**&#x200B;区域。
1. 选择&#x200B;**新增**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Experience Manager Assets。

1. 单击&#x200B;**Assets** > **文件和文件夹**。

1. 单击&#x200B;**筛选器**&#x200B;图标，然后在&#x200B;**资源类型**&#x200B;部分中选择&#x200B;**文件夹**。

1. 选择要链接的文件夹。

1. 单击&#x200B;**选择**。

## 注意事项

* 内容审查程序功能不适用于使用Adobe企业级存储的对象。 如果贵组织使用Adobe企业存储，您仍然可以链接Experience Manager Assets或Assets Essentials中的资源和文件夹，但您将无权访问Content Advisor功能，例如AI 搜索、智能建议或Dynamic Media呈现版本。 有关详细信息，请参阅[将Adobe Experience Manager与Frame.io集成一起使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

* 内容审查程序功能不适用于Assets Essentials。 要从Assets Essentials链接资源和文件夹，请参阅[从Experience Manager Assets Essentials链接资源和文件夹](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md)。

* 在将资源从Workfront发送到Experience Manager Assets时，首先映射元数据字段。 如果您的Workfront管理员启用了对象元数据同步，则在任一应用程序中更改了某些字段后，这些字段将保持最新状态。
