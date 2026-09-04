---
product-area: Canvas Dashboards
navigation-topic: report-types
title: 复制画布功能板
description: 您可以复制画布功能板以创建其变体，例如特定于受众的副本，而无需从头开始重建。
author: Courtney
feature: Reports and Dashboards
source-git-commit: b66f6931ee2fe83688fb8910861af6e958d1f74f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 4%

---

# 复制画布功能板

{{highlighted-preview-article-level}}

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

您可以复制画布功能板以针对不同受众创建其变体，例如执行功能板的董事级副本，而无需从头开始重新构建。

## 访问要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>“任一” </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
<p>标准 </p> 
<p>规划</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td><p>编辑或创建对功能板的访问权限</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>查看对仪表板的访问权限</p>
  </td> 
  </tr>
</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

必须先创建功能板，然后才能复制该功能板。

有关详细信息，请参阅[创建画布功能板](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)。

## 复制功能板

>[!NOTE]
>
>共享首选项将不会复制到新仪表板。 如果小组件具有&#x200B;**以用户**&#x200B;身份运行，则只有在您是指定用户或系统管理员时，该配置才会保留在副本中。

要复制功能板，请执行以下操作：

{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 在&#x200B;**画布功能板**&#x200B;页面上，打开要复制的功能板。

1. 在右上角，选择&#x200B;**更多** ![更多图标](assets/more-icon.png)图标，然后选择&#x200B;**复制**。
   ![复制仪表板菜单选项](assets/duplicate-dashboard.png)

1. 在&#x200B;**复制仪表板**&#x200B;对话框中，为新仪表板输入&#x200B;**名称**，该名称默认为源仪表板的名称，后跟“（复制）”。

1. （可选）在&#x200B;**仪表板详细信息**&#x200B;选项卡上，更新新仪表板的&#x200B;**Description**&#x200B;或&#x200B;**Currency**。
   ![复制仪表板 — 仪表板详细信息选项卡](assets/duplicate-details.png)

1. （可选）单击&#x200B;**小组件**选项卡，然后取消选择不想包含在重复仪表板中的任何小组件。
   ![复制仪表板 — Widget选项卡](assets/copy-widgets.png)

1. （可选）单击&#x200B;**筛选器和提示**&#x200B;选项卡，然后关闭&#x200B;**复制仪表板筛选器**&#x200B;或&#x200B;**复制仪表板提示**，以将其从重复仪表板中排除。
   ![复制仪表板 — “筛选器和提示”选项卡](assets/copy-filters.png)

1. 单击&#x200B;**复制仪表板**。

此时会显示一条确认消息，其中包含指向新功能板的链接。
