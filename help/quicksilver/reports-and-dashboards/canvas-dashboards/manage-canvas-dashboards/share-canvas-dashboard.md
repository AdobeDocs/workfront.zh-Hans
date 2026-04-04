---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: 共享画布功能板
description: 您可以与其他Adobe Workfront用户共享画布功能板，以便他们能够查看或编辑该功能板。
author: Courtney
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 7716fb1c68bee2540556df98c227d8c5bae7b2d8
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# 共享画布功能板

{{highlighted-preview}}

>[!IMPORTANT]
>
>画布功能板目前仅适用于参与Beta测试阶段的用户。 在此阶段，部分功能可能无法完成或无法按预期工作。 请按照“画布功能板测试版”概述文章中[提供反馈](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)部分的说明提交任何有关您体验的反馈。<br>
>如果您对可能的错误或技术问题有反馈，请向Workfront支持提交票证。 有关详细信息，请参阅[联系客户支持](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)。<br>
>请注意，以下云提供商未提供此测试版：
>
>* 自带Amazon Web Services密钥
>* Azure
>* Google Cloud Platform

您可以与其他Adobe Workfront用户共享画布功能板，以便他们查看或编辑该功能板。

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
   <td><p>查看对报告、功能板和日历的访问权限</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td><p>查看仪表板共享仪表板的权限</p>
   <p>管理仪表板的权限以分配仪表板权限</p>
  </td> 
  </tr>
</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 关于共享功能板的注意事项

* 可以将功能板共享给用户、团队、组、工作角色或公司资源。

* 默认情况下，功能板的创建者具有功能板的管理权限。

* 系统管理员和具有管理权限的用户可以授予对功能板的“查看”或“管理”访问权限。

* 对功能板具有查看权限的用户可以授予对功能板的查看权限。

* 共享功能板时，共享该功能板的资源将继承对该功能板中显示的报告的权限。

* 当通过布局模板分发功能板时，该功能板（及其报表）的自动查看权限被授予分配给布局模板的所有资源。

* <span class="preview">当仪表板上的报告配置为以用户身份运行选项时，所有查看者都会根据选定用户的权限而不是他们自己的权限查看数据。 这意味着查看者可能会看到他们通常无权访问的数据。 如果仪表板上的某些报表使用以用户身份运行，而其他报表未使用以用户身份运行，则查看者可能会看到报表间的数据不一致。</span>


## 共享画布功能板


{{step1-to-dashboards}}

1. 在左侧面板中，单击&#x200B;**画布功能板**。

1. 在&#x200B;**画布功能板**&#x200B;页面上，选择要共享的功能板。

1. 在页面的右上角，单击&#x200B;**共享**&#x200B;按钮。 出现&#x200B;**仪表板共享**&#x200B;对话框。

   ![共享按钮](assets/share-button.png)

1. 在&#x200B;**将访问权限授予**&#x200B;字段中，开始键入要与共享画布功能板的特定用户、团队、角色、组或公司的名称，然后当它出现在下拉列表中时将其选定。

1. （可选）要编辑资源对仪表板的访问权限，请单击资源名称旁边的&#x200B;**查看**，然后在显示的下拉列表中选择&#x200B;**管理**。

   >[!NOTE]
   >
   > 当用户没有通过访问级别分配的功能板的编辑权限时，无法将管理权限分配给功能板。

1. 对要与其共享功能板的每个资源重复步骤5至6。

1. 单击&#x200B;**共享**&#x200B;按钮。 收件人会收到电子邮件通知，告知他们该仪表板已与他们共享，他们现在可以在&#x200B;**仪表板** > **画布仪表板** > **共享仪表板**&#x200B;中访问它。

   >[!NOTE]
   >
   > 可能会应用电子邮件通知的单个用户首选项和系统排除项。<br>
   > 仅当直接与用户共享时，才会发送通知。 共享到组、角色、公司和团队不会生成电子邮件通知。<br>
   > 从布局模板继承的权限不会生成有关仪表板访问权限的电子邮件通知。
