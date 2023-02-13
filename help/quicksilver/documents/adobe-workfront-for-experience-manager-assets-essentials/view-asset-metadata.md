---
content-type: reference
product-area: documents;workfront-integrations
navigation-topic: documents-navigation-topic
title: 查看Experience Manager Assets或Assets Essentials的映射元数据
description: 您可以在“文档详细信息和摘要”面板中查看已映射元数据的实时视图。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: cfad5855-033c-4a15-b5a2-7ff32ed65fe9
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# 查看Experience Manager Assets或Assets Essentials的映射元数据

您可以在“文档详细信息和摘要”面板中查看已映射元数据的实时视图。 当您将资产从Workfront发送到Experience Manager Assets或Assets Essentials时，首先会映射元数据字段。 如果Workfront管理员已启用对象元数据同步，则在任一应用程序中更改字段时，这些字段将保持为最新。

## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>Adobe Workfront计划*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront许可证*</strong>
   </td>
   <td>请求或更高版本
   </td>
  </tr>
  <tr>
   <td><strong>产品</strong>
   </td>
   <td>您必须具有Experience Manager Assetsas a Cloud Service或Assets Essentials，并且必须以Admin Console用户身份添加到产品中。
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置*</strong>
   </td>
   <td>编辑对文档的访问
<p>
<strong>注意： </strong>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <strong>创建或修改自定义访问级别</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>对象权限</strong>
   </td>
   <td>查看访问权限或更高权限
<p>
有关请求其他访问权限的信息，请参阅 <strong>请求对对象的访问 </strong>.
   </td>
  </tr>
</table>


*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。


## 先决条件

开始之前，

* 您的Workfront管理员必须配置Experience Manager集成。 有关更多信息，请参阅 [配置Experience Manager Assetsas a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) 或 [配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## 文档详细信息

要在文档详细信息中打开元数据面板，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后选择 **文档**.
1. 将鼠标悬停在所需的文档上，然后选择 **文档详细信息**.
1. 查找并展开 **元数据** 中。
   >[!NOTE]
   >
   >无法编辑此部分中的字段。 它们仅视图。

![“文档详细信息”面板](assets/metadata-panel-doc-details.png)


## 文档摘要

要在“摘要”面板中打开“元数据”面板，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后选择 **文档**.
1. 查找所需的文档。
1. 单击 **“摘要”图标** ![摘要图标](assets/summary-panel-icon.png)，然后展开 **元数据** 中。
   >[!NOTE]
   >
   >无法编辑此部分中的字段。 它们仅视图。

![文档摘要](assets/metadata-panel-summary.png)
