---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 从Illustrator上传校样
description: 您可以将艺术展示板上传为文档，以便快速审阅和批准，或只需将其存储在Adobe Workfront中。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 0%

---

# 从[!DNL Illustrator]上传校样

您可以将艺术展示板作为验证直接上传到[!DNL Adobe Workfront]以进行彻底审阅和批准。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> 任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>标准</p> <p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>除了[!DNL Adobe Creative Cloud]许可证，您还必须具有[!DNL Workfront]许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>[!UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对[!UICONTROL 文档]的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

* 您必须先安装[!DNL Adobe Workfront for design and video]，然后才能从[!DNL Illustrator]上载校样。

  有关说明，请参阅[安装 [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md)。

## 上传基本校对

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![返回工作列表](assets/go-back-to-work-list-350x314.png)

1. 转到要上载校样的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。
1. 单击插件底部附近的&#x200B;**[!UICONTROL 新建文件]**。
1. 启用&#x200B;**[!UICONTROL 创建验证]**&#x200B;切换开关。
1. （可选）在&#x200B;**[!UICONTROL 校对名称]**&#x200B;文本框中键入校对的名称。
1. 在&#x200B;**[!UICONTROL 校对审批]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 基本]**。
1. （可选）添加批准者。
1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。

   ![添加评论](assets/add-comment.png)

1. 从下拉菜单中选择&#x200B;**[!UICONTROL 资源类型]**。

1. （可选）选择&#x200B;**[!UICONTROL 添加外部文件]**&#x200B;以从您的计算机添加文件。
1. 单击&#x200B;**[!UICONTROL 上传]**，然后根据以上选择的资源类型配置任何所需的导出选项。

   插件中的![文件](assets/plugin-files-350x307.png)\
   该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。


## 上传自动验证

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![返回工作列表](assets/go-back-to-work-list-350x314.png)

1. 转到要上载校样的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击插件底部附近的&#x200B;**[!UICONTROL 新建文件]**。
1. 启用&#x200B;**[!UICONTROL 创建验证]**&#x200B;切换开关。
1. （可选）在&#x200B;**[!UICONTROL 校对名称]**&#x200B;文本框中键入校对的名称。
1. 在&#x200B;**[!UICONTROL 校对审批]**&#x200B;部分中，选择&#x200B;**[!UICONTROL 自动]**。
1. （可选）在&#x200B;**[!UICONTROL 工作流模板]**&#x200B;框中，键入验证工作流模板的名称。

{{adjust-proof-settings}}

>[!NOTE]
>
> 如果工作流模板中有任何空白必填字段，则自动验证设置会自动打开，并且您需要填充这些字段才能上传验证。


1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。

   ![添加评论到自动审批](assets/add-comment-automated-approval.png)

1. 从下拉菜单中选择&#x200B;**[!UICONTROL 资源类型]**。
1. （可选）选择&#x200B;**[!UICONTROL 添加外部文件]**&#x200B;以从您的计算机添加文件。
1. 单击&#x200B;**[!UICONTROL 上传]**，然后根据以上选择的资源类型配置任何所需的导出选项。
该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。

## 上传新验证版本

您可以上传新版本的验证。 该插件会记住在以前的版本上设置的验证工作流，但您可以根据需要更改此设置。

1. 单击右上角的&#x200B;**[!UICONTROL 菜单]**&#x200B;图标，然后选择&#x200B;**[!UICONTROL 工作列表]**。 您还可以使用菜单导航到父对象。

   ![返回工作列表](assets/go-back-to-work-list-350x314.png)

1. 转到需要上载文档的工作项。
1. 单击导航栏中的&#x200B;**[!UICONTROL 文档]**&#x200B;图标![文档图标](assets/documents.png)。

1. 单击插件底部附近的&#x200B;**[!UICONTROL 新版本]**。
1. 启用&#x200B;**[!UICONTROL 创建验证]**&#x200B;切换开关。

1. 在&#x200B;*[!UICONTROL *校对审批]&#x200B;**分区中，选择&#x200B;**&#x200B;[!UICONTROL 基本]&#x200B;**&#x200B;或&#x200B;**&#x200B;[!UICONTROL 自动]**。

1. 根据您在步骤7中选择的审批类型添加&#x200B;**[!UICONTROL 审阅者]**&#x200B;或&#x200B;**[!UICONTROL 工作流模板]**。

1. （可选）在&#x200B;**[!UICONTROL 更新]**&#x200B;区域键入评论。
1. 从下拉菜单中选择&#x200B;**[!UICONTROL 资源类型]**。
1. 单击&#x200B;**[!UICONTROL 上传]**，然后根据以上选择的资源类型配置任何所需的导出选项。
该文档显示在插件和桌面应用程序的[!UICONTROL 文档]区域中。
