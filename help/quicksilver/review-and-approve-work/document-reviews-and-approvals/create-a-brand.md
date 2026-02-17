---
product-area: documents
navigation-topic: approvals
title: 为AI审阅者设置品牌
description: 为AI审阅者设置品牌
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b2788f3f-43d2-46f3-8502-bb833f8a0970
source-git-commit: 07b401c70dfd209d13c34cf62844f334f3260af1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 5%

---

# 为AI审阅者设置品牌

>[!IMPORTANT]
>
>此功能当前处于测试阶段。

AI审阅者使用品牌准则在审阅过程中评估内容。 您可以通过上传包含品牌指南的PDF文件或手动输入品牌元素，在Workfront中创建品牌。

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
   <td> <p>您必须安装GenStudio Brand Manager。</p>
    <p>注意：要选择GenStudio Brand Manager，您必须按照<a href="https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/intro/configure-brand-permissions">分配品牌权限</a>中概述的步骤操作。</p>
   </td> 
  </tr> 
 </tbody> 
</table>





有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 先决条件

* 贵组织必须已迁移到Adobe IMS (Identity Management System)。
* 您的Workfront实例必须启用统一批准。
* 您的组织必须具有GenStudio Foundation。
* Adobe必须有一个已签署的Adobe Gen AI协议文件。
有关签署协议的更多信息，请参阅[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。


## 使用PDF创建品牌

{{step-1-to-setup}}

1. 在左侧面板中，转到&#x200B;**审核和批准** > **品牌**。
1. 单击屏幕右上角的&#x200B;**添加品牌**。
1. 为品牌命名。
1. 单击上传PDF以上传品牌文件。
   ![上载品牌PDF](assets/upload-PDF.png)
1. 单击&#x200B;**继续**。
1. 上载一个或多个包含品牌指南的PDF文件，然后单击&#x200B;**添加品牌**。
1. 上传文件后，请查看提取的品牌元素，确保它们符合您的品牌准则。

   >[!IMPORTANT]
   >
   >准则是使用您的文件和创作AI技术生成的，可能不准确。 查看提取的准则以了解缺少或不正确的详细信息，并在发布此品牌之前编辑它们。

1. 完成后，单击&#x200B;**发布**&#x200B;以使该品牌可用于AI审阅者。

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
        <td>标志</td>
        <td>包括与品牌关联的官方徽标。</td>
    </tr>
    <tr>
        <td>颜色</td>
        <td>指定品牌的调色板。</td>
    </tr>
    </table>

   ![手动添加品牌元素](assets/brand-elements.png)


1. 完成后，单击&#x200B;**发布**&#x200B;以使该品牌可用于AI审阅者。
