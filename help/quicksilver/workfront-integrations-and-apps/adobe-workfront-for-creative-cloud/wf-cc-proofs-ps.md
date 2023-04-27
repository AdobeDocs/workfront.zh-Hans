---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: 从Adobe Photoshop上传校样
description: 您可以将您的艺术展示板作为校样直接上传到Adobe Workfront，以便进行彻底的审核和批准。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: cbb12ee7-949e-44a1-9340-3ef93c003b21
source-git-commit: 698affafa8771e9e91b725908d4782a2af12c0b8
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# 从上传校样 [!DNL Photoshop]

您可以将艺术展示板作为校样直接上传到 [!DNL Adobe Workfront] 进行彻底的审查和批准。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>当前计划：[!UICONTROL Pro]或更高版本</p> <p>或</p> <p>旧版计划：[!UICONTROL Premium]</p> <p>有关使用不同计划校样访问权限的更多信息，请参阅。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>当前计划：[!UICONTROL Work]或[!UICONTROL Proof]</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您必须具有 [!DNL Adobe Creative Cloud] 除 [!DNL Workfront] 许可证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>[!UICONTROL Manager]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>编辑对[!UICONTROL Documents]的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 先决条件

* 您必须安装 [!DNL Adobe Workfront for Photoshop] 插件，然后才能从 [!DNL Adobe Photoshop].

   有关说明，请参阅 [安装 [!DNL Adobe Workfront for Photoshop]](../../workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md).

## 上传基本校样

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/go-back-to-work-list-350x314.png)

1. 转到要上传校样的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 中。
1. 单击 **[!UICONTROL 新建文件]** 在插件底部附近。
1. 启用 **[!UICONTROL 创建校样]** 切换。
1. （可选）在中键入校样的名称 **[!UICONTROL 校样名称]** 框中。
1. 在 **[!UICONTROL 校样批准]** 选择 **[!UICONTROL 基本]**.
1. （可选）添加批准者。
1. （可选）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/add-comment.png)

1. 选择 **[!UICONTROL 资产类型]** 下拉菜单中。

1. （可选）选择 **[!UICONTROL 添加外部文件]** 从计算机添加文件。
1. 单击 **[!UICONTROL 上传]**，然后根据上面选择的资产类型配置任何所需的导出选项。

   ![](assets/plugin-files-350x307.png)\
   文档将显示在 [!UICONTROL 文档] 区域。


## 上传自动校样

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/go-back-to-work-list-350x314.png)

1. 转到要上传校样的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png) 中。

1. 单击 **[!UICONTROL 新建文件]** 在插件底部附近。
1. 启用 **[!UICONTROL 创建校样]** 切换。
1. （可选）在中键入校样的名称 **[!UICONTROL 校样名称]** 框中。
1. 在 **[!UICONTROL 校样批准]** 选择 **[!UICONTROL 自动]**.
1. （可选）在 **[!UICONTROL 工作流模板]** 框中，键入校样工作流模板的名称。

{{adjust-proof-settings}}

>[!NOTE]
>
> 如果工作流模板中存在任何空白必填字段，则会自动打开自动校样设置，您需要填充这些字段才能上传校样。


1. （可选）在 **[!UICONTROL 更新]** 的上界。

   ![](assets/add-comment-automated-approval.png)

1. 选择 **[!UICONTROL 资产类型]** 下拉菜单中。
1. （可选）选择 **[!UICONTROL 添加外部文件]** 从计算机添加文件。
1. 单击 **[!UICONTROL 上传]**，然后根据上面选择的资产类型配置任何所需的导出选项。
文档将显示在 [!UICONTROL 文档] 区域。

## 上传新校样版本

您可以上传校样的新版本。 该插件会记住在以前版本中设置的校对工作流，但您可以根据需要更改此工作流。

1. 单击 **[!UICONTROL 菜单]** 图标，然后选择 **[!UICONTROL 工作列表]**. 您还可以使用菜单导航到父对象。

   ![](assets/go-back-to-work-list-350x314.png)

1. 转到将文档上传到所需的工作项。
1. 单击 **[!UICONTROL 文档]** 图标 ![](assets/documents.png)中。

1. 单击 **[!UICONTROL 新版本]** 在插件底部附近。
1. 启用 **[!UICONTROL 创建校样]** 切换。

1. 在 *[!UICONTROL *校样批准]**部分，选择 **[!UICONTROL 基本]** 或 **[!UICONTROL 自动]**.

1. 添加 **[!UICONTROL 审阅人]** 或 **[!UICONTROL 工作流模板]** 根据您在步骤7中选择的批准类型。

1. （可选）在 **[!UICONTROL 更新]** 的上界。
1. 选择 **[!UICONTROL 资产类型]** 下拉菜单中。
1. 单击 **[!UICONTROL 上传]**，然后根据上面选择的资产类型配置任何所需的导出选项。
文档将显示在 [!UICONTROL 文档] 区域。
