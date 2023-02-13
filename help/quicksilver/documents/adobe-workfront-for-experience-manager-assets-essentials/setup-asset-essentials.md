---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 配置Experience Manager Assets Essentials集成
description: 在Experience Manager Assets Essentials — 编辑我中将您的作品与内容连接起来。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 059cfa79c57f071b3c7efd690b583099f46c99fb
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# 配置Experience Manager Assets Essentials集成

将您的作品与Experience Manager Assets Essentials中的内容&#x200B;连接：

* 将资产和元数据从Adobe Workfront推送到Experience Manager Assets Essentials &#x200B;
* 将资产从Experience Manager Assets Essentials链接到Workfront中的项目和任&#x200B;务
* 促进推送到Experience Manager Assets Essentials的资产的版本控制工作流


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
   <td>计划
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager许可证</strong>
   </td>
   <td>标准
   </td>
  </tr>
  <tr>
   <td><strong>产品</strong>
   </td>
   <td>您必须拥有Experience Manager Assets Essentials，并且必须以Admin Console用户身份添加到产品中。
   </td>
  </tr>
  <tr>
   <td><strong>访问级别配置</strong>
   </td>
   <td>您必须是Workfront管理员。 有关Workfront管理员的信息，请参阅 <strong>授予用户完全管理访问权限</strong>.
   </td>
  </tr>
</table>


*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。


## 设置集成

1. 单击 **主菜单** 图标，然后单击 **设置**.
1. 选择  **文档** ![文档图标](assets/document-icon.png) 在左侧面板中，选择 **Experience Manager集成**.
1. 选择 **添加Experience Manager集成**.
1. 指定以下内容：

   <table>
   <tr>
      <td><strong>名称</strong>
      </td>
      <td>在“文档”区域的“添加新”按钮中输入您希望用户看到的名称。
      </td>
   </tr>
   <tr>
      <td><strong>导航URL</strong>
      </td>
      <td>系统会自动填充导航URL。 此URL用于从主菜单链接到贵组织的Assets Essentials实例，以便快速访问。
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets存储库</strong>
      </td>
      <td>
      系统会自动填充与您的组织ID关联的Experience Manager存储库。
      </td>
   </tr>
   </table>

1. 单击 **保存** 或继续 [设置元数据（可选）](#set-up-metadata-optional) 章节。


## 设置元数据（可选）

将 Workfront 对象数据映射到 Experience Manager Assets 中的资源媒体字段。元数据会在第一次从 Workfront 推送资源时进行映射。


### 先决条件

在开始之前，您必须

* 在Experience Manager Assets Essentials中配置元数据架构，如 [配置Adobe Workfront和Experience Manager Assets之间的资产元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* （可选）在Workfront中配置自定义表单字段。 Workfront有许多您可以使用的内置自定义字段。 但是，您也可以创建自己的自定义字段。 有关更多信息，请参阅 [创建或编辑自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### 资产

元数据映射首次从Workfront推送资产时。 首次将资产发送到Experience Manager Assets Essentials时，具有内置或自定义字段的文档会自动映射到指定的字段。

1. 在 **Workfront字段** 列中，选择内置或自定义Workfront字段。
   >[!NOTE]
   >
   >您可以将单个Workfront字段映射到多个Experience Manager Assets字段。 您无法将多个Workfront字段映射到单个Experience Manager Assets字段。
1. 在 **Experience Manager** 字段中，选择一个Experience Manager Assets字段。
1. 根据需要重复步骤1和2。
   ![启用元数据](assets/metadata-assets-essentials.png)
1. 单击 **保存** 或继续 [设置链接的文件夹（可选）](#set-up-linked-folders-optional) 章节。


## 设置链接的文件夹（可选）

{{setup-linked-folder}}
