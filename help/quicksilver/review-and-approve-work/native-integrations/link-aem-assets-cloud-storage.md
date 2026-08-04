---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: 将Experience Manager Assets中的内容和文件夹与Adobe云存储链接到一起
description: 如果您的组织使用Adobe云存储，则可以将Experience Manager Assets中的内容和文件夹链接到支持文档的任何Adobe Workfront对象。
author: Courtney
source-git-commit: 66635b2edc78833ec2d08cef382b39b89238b565
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 2%

---

# 将Experience Manager Assets中的内容和文件夹与Adobe云存储链接到一起

如果您的组织使用Adobe云存储，您可以将内容和文件夹从Experience Manager Assets链接到Workfront。 链接后，您可以在Workfront中查看和管理内容，对Experience Manager Assets中的内容所做的任何更改都将反映在Workfront中。

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
   <td>您必须具有Experience Manager as a Cloud Service，并且您必须在Admin Console中作为用户添加到产品中。</td> 
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

* 您的Workfront管理员必须配置Experience Manager集成。 有关详细信息，请参阅[将Adobe Experience Manager与Frame.io集成一起使用](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md)。

* 要使用Smart建议或Campaign Briefs功能，您必须签署GenAI Rider。 有关详细信息，请参阅[使用内容审查程序访问Adobe应用程序中的AEM内容](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search)。

## 从Experience Manager Assets链接内容

要链接内容，请执行以下操作：

1. 转到要在其中链接内容的Workfront对象。
1. 单击左侧面板中的&#x200B;**文档**&#x200B;部分。
1. 单击页面右侧的&#x200B;**新建**，然后单击&#x200B;**AEM文件**以链接单个资源。
   ![将AEM文件添加到文档区域](assets/aem-files.png)

1. 使用内容审查程序，您可以：

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>使用AI 搜索搜索资源。</strong> 使用AI支持的搜索，该搜索理解查询背后的含义和意图，支持多种语言、拼写错误和同义词。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">更智能的资源发现AI 搜索</a>。</td>
      </tr>
      <tr>
         <td><strong>根据上下文和意图查看智能建议。</strong> 使用宿主Adobe应用程序提供的上下文感知推荐，探索符合您的内容需求的资源。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">基于上下文和意图的智能建议</a>。</td>
      </tr>
      <tr>
         <td><strong>上传营销活动简报以发现相关资源。</strong> 上传PDF、DOCX或TXT营销活动简介文档，以便内容顾问可以分析该文档并推荐相关资源。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">发现相关资产的Campaign简介</a>。</td>
      </tr>
      <tr>
         <td><strong>查看和选择Dynamic Media资源演绎版。</strong> 浏览渠道优化演绎版（包括图像预设、智能裁剪和格式类型），并应用Dynamic Media修饰符实时预览调整。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的Dynamic Media资源演绎版</a>。</td>
      </tr>
      <tr>
         <td><strong>将Dynamic Media修饰符应用于演绎版。</strong> 添加修饰符以实时转换资源演绎版，并在为主机应用程序选择演绎版之前预览结果。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">可供使用的Dynamic Media资源演绎版</a>。</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>访问资源元数据。</strong> 查看与Assets视图一致的资源属性，例如标题、描述、格式、大小和其他元数据选项卡（产品、营销活动、标记）。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">访问与Assets视图一致的资源元数据</a>。</td>
      </tr>
      <tr>
         <td><strong>使用预定义筛选器筛选资源。</strong> 使用文件类型、文件格式、资源状态、文件大小、图像宽度、图像高度、修改日期和创建日期等过滤器优化资源结果。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">与Assets视图一致的访问筛选器</a>。</td>
      </tr>
      <tr>
         <td><strong>保存并重用搜索。</strong> 通过指定搜索词和过滤器选项创建保存的搜索，然后在Experience Manager Assets和其他Adobe应用程序中重复使用它们。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">访问和重复使用最近和保存的搜索</a>。</td>
      </tr>
      <tr>
         <td><strong>在收藏集间和收藏集中搜索资产。</strong> 在所有收藏集中搜索资产或收藏集，或将搜索限制在特定收藏集中。</td>
         <td>有关详细信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">在收藏集间和收藏集中搜索资产</a>。</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >内容指导中的推荐内容使用来自以下项的数据来确定Workfront中的推荐内容：
   >
   >* Workfront对象名称和描述字段
   >* 标记为必填的自定义表单字段
   >* 来自附加文档的数据

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## 注意事项

* 链接的AEM资源不支持审阅和批准工作流。
* 在将资源从Workfront发送到Experience Manager Assets时，首先映射元数据字段。 如果您的Workfront管理员启用了对象元数据同步，则在任一应用程序中更改了某些字段后，这些字段将保持最新状态。
