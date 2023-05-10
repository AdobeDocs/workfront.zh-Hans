---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 配置Experience Manager Assets Essentials集成
description: 在Experience Manager Assets Essentials — 编辑我中将您的作品与内容连接起来。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 9965ec9f436724e438fbbc5977f22761cc673878
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 4%

---

# 配置Experience Manager Assets Essentials集成

将您的作品与Experience Manager Assets Essentials中的内容&#x200B;连接：

* 将资产和元数据从Adobe Workfront推送到Experience Manager Assets Essentials &#x200B;
* 将资产从Experience Manager Assets Essentials链接到Workfront中的项目和任&#x200B;务
* 促进推送到Experience Manager Assets Essentials的资产的版本控制工作流

您还可以将多个Experience Manager Assets存储库连接到一个Workfront环境，或将多个Workfront环境跨组织ID连接到一个Experience Manager Assets存储库。 对于要设置的每个集成，请按照本文中的配置说明进行操作。

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

+++ **支持的Workfront和Experience Manager Assets字段**

**AEM关键词**

您可以在Workfront Essentials中将任何Experience Manager Assets支持的字段映射到关键词。

要将字段链接到关键词，请选择 `dc:subject` 在元数据映射区域的Experience Manager Assets字段下拉列表中。

要将多个单行文本字段映射到关键字，请在元数据映射的Workfront侧输入以逗号分隔的关键字值列表， `dc:subject` 在Experience Manager Assets那边。 每个字段值都映射到一个单独的关键字。 您可以使用计算字段将多个Workfront字段合并为一个以逗号分隔的文本字段。

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### 资产

元数据映射首次从Workfront推送资产时。 首次将资产发送到Experience Manager Assets Essentials时，具有内置或自定义字段的文档会自动映射到指定的字段。

1. 在 **Workfront字段** 列中，选择内置或自定义Workfront字段。
   >[!NOTE]
   >
   >您可以将单个Workfront字段映射到多个Experience Manager Assets字段。 您无法将多个Workfront字段映射到单个Experience Manager Assets字段。
1. 在 **Experience Manager** 字段中，选择一个Experience Manager Assets字段。

   要将Workfront字段映射到Experience Manager Assets标记，请选择 `dc:subject`.
1. 根据需要重复步骤1和2。
   ![启用元数据](assets/metadata-assets-essentials.png)
1. 单击 **保存** 或继续 [设置链接的文件夹（可选）](#set-up-linked-folders-optional) 章节。


## 设置链接的文件夹（可选）

{{setup-linked-folder}}
