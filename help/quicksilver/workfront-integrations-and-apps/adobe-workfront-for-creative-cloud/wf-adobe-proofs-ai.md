---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 从Illustrator上传校样
description: 您可以将艺术展示板上传为文档，以便快速审阅和批准，或只需将其存储在Adobe Workfront中。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: e98f27d4-7c07-44cc-8df5-e04472ec946e
source-git-commit: 66186bb8af14e7ce86b3fb5e8bb1b07fe32dca7a
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 0%

---

# 上传校样自 [!DNL Illustrator]

您可以将艺术展示板作为校样直接上传到 [!DNL Adobe Workfront] 以进行彻底的审查和批准。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>当前计划： [！UICONTROL Pro]或更高版本</p> <p>或</p> <p>旧版计划： [！UICONTROL Premium]</p> <p>有关验证不同规划的访问权限的更多信息，请参阅。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>当前计划： [！UICONTROL Work]或[！UICONTROL Proof]</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须拥有 [!DNL Adobe Creative Cloud] 除了许可证之外， [!DNL Workfront] 许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>[！UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对[！UICONTROL文档]的访问权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或验证权限配置文件，请联系您的 [!DNL Workfront] 或 [!DNL Workfront Proof] 管理员。

## 先决条件

* 您必须安装 [!DNL Adobe Workfront for design and video] 上传校样之前 [!DNL Illustrator].

  有关说明，请参阅 [安装 [!DNL Adobe Workfront for design and video]](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-install-cc.md).

## 上传基本校对

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/go-back-to-work-list-350x314.png)

1. 转到要上载校样的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 在导航栏中。
1. 单击 **[!UICONTROL 新建文件]** 接近插件的底部。
1. 启用 **[!UICONTROL 创建验证]** 切换。
1. （可选）在中键入验证的名称 **[!UICONTROL 校对名称]** 文本框。
1. 在 **[!UICONTROL 校对审批]** 部分，选择 **[!UICONTROL 基本]**.
1. （可选）添加批准者。
1. （可选）在 **[!UICONTROL 更新]** 区域。

   ![](assets/add-comment.png)

1. 选择 **[!UICONTROL 资源类型]** 从下拉菜单中。

1. （可选）选择 **[!UICONTROL 添加外部文件]** 以从计算机添加文件。
1. 单击 **[!UICONTROL 上传]**，然后根据以上选择的资源类型配置任何所需的导出选项。

   ![](assets/plugin-files-350x307.png)\
   文档显示在 [!UICONTROL 文档] 插件和桌面应用程序中的区域。


## 上传自动验证

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/go-back-to-work-list-350x314.png)

1. 转到要上载校样的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 在导航栏中。

1. 单击 **[!UICONTROL 新建文件]** 接近插件的底部。
1. 启用 **[!UICONTROL 创建验证]** 切换。
1. （可选）在中键入验证的名称 **[!UICONTROL 校对名称]** 文本框。
1. 在 **[!UICONTROL 校对审批]** 部分，选择 **[!UICONTROL 自动]**.
1. （可选）在 **[!UICONTROL 工作流模板]** 框中，键入验证工作流模板的名称。

{{adjust-proof-settings}}

>[!NOTE]
>
> 如果工作流模板中有任何空白必填字段，则自动验证设置会自动打开，并且您需要填充这些字段才能上传验证。


1. （可选）在 **[!UICONTROL 更新]** 区域。

   ![](assets/add-comment-automated-approval.png)

1. 选择 **[!UICONTROL 资源类型]** 从下拉菜单中。
1. （可选）选择 **[!UICONTROL 添加外部文件]** 以从计算机添加文件。
1. 单击 **[!UICONTROL 上传]**，然后根据以上选择的资源类型配置任何所需的导出选项。
文档显示在 [!UICONTROL 文档] 插件和桌面应用程序中的区域。

## 上传新验证版本

您可以上传新版本的验证。 该插件会记住在以前的版本上设置的验证工作流，但您可以根据需要更改此设置。

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/go-back-to-work-list-350x314.png)

1. 转到需要上载文档的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png)在导航栏中。

1. 单击 **[!UICONTROL 新版本]** 接近插件的底部。
1. 启用 **[!UICONTROL 创建验证]** 切换。

1. 在 *[!UICONTROL *验证审批]**部分，选择 **[!UICONTROL 基本]** 或 **[!UICONTROL 自动]**.

1. 添加 **[!UICONTROL 审阅者]** 或 **[!UICONTROL 工作流模板]** 基于您在步骤7中选择的批准类型。

1. （可选）在 **[!UICONTROL 更新]** 区域。
1. 选择 **[!UICONTROL 资源类型]** 从下拉菜单中。
1. 单击 **[!UICONTROL 上传]**，然后根据以上选择的资源类型配置任何所需的导出选项。
文档显示在 [!UICONTROL 文档] 插件和桌面应用程序中的区域。
