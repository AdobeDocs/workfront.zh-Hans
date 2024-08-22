---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 配置Experience Manager Assets Essentials集成
description: 将您的工作与Experience Manager Assets Essentials中的内容连接起来。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 1%

---

# 配置 Experience Manager Assets Essentials 集成

将您的工作与Experience Manager Assets Essentials中的内容连接起来&#x200B;：

* 将资源和元数据从Adobe Workfront推送到Experience Manager Assets &#x200B; Essentials
* 将Experience Manager Assets Essentials中的资源关联到Workfront中的项目和任务&#x200B;。
* 促进推送到Experience Manager Assets Essentials的资源的版本控制工作流

>[!NOTE]
>
>您还可以跨组织ID将多个Experience Manager Assets存储库连接到一个Workfront环境，或将多个Workfront环境连接到一个Experience Manager Assets存储库。 对于要设置的每个集成，请按照本文中的配置说明进行操作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table>
  <tr>
   <td>[!DNL Adobe Workfront] 计划
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] 许可证
   </td>
   <td><p>当前： [！UICONTROL计划]</p>
   <p>新文档： [！UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] 许可证
   </td>
   <td>[！UICONTROL标准版]
   </td>
  </tr>
  <tr>
   <td>产品
   </td>
   <td>您必须具有Experience Manager Assets Essentials，并且您必须在Admin Console中作为用户添加到产品中。
   </td>
  </tr>
  <tr>
   <td>访问级别配置
   </td>
   <td>您必须是[!DNL Workfront]管理员。
   </td>
  </tr>
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 设置集成

{{step-1-to-setup}}

1. 在左侧面板中选择&#x200B;**文档** ![文档图标](assets/document-icon.png)，然后选择&#x200B;**Experience Manager集成**。
1. 选择&#x200B;**添加Experience Manager集成**。
1. 指定以下内容：

   <table>
   <tr>
      <td><strong>名称</strong>
      </td>
      <td>在“文档”区域的“新增”按钮中，输入您希望用户看到的名称。
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
      系统会自动填充与您的Experience ManagerID关联的组织存储库。
      </td>
   </tr>
   </table>

1. 单击&#x200B;**保存**&#x200B;或转到本文中的[设置元数据（可选）](#set-up-metadata-optional)部分。


## 设置元数据（可选）

将Workfront对象数据映射到Experience Manager Assets中的资源媒体字段。 元数据在首次从Workfront推送资源时映射。


### 先决条件

在开始之前，您必须

* 在Experience Manager Assets Essentials中配置元数据架构，如[配置Adobe Workfront和Experience Manager Assets之间的资源元数据映射](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en)中所述。
* （可选）在Workfront中配置自定义表单字段。 Workfront提供了许多内置自定义字段。 但是，您也可以创建自己的自定义字段。 有关详细信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 支持的Workfront和Experience Manager Assets字段

### AEM关键词

您可以将任何Workfront支持的字段映射到Experience Manager Assets Essentials中的关键字。

要将字段链接到关键字，请在元数据映射区域的Experience Manager Assets字段下拉列表中选择`xcm:keywords`。

要将多个单行文本字段映射到关键字，请在元数据映射的Workfront端和Experience Manager Assets端分别输入一个以逗号分隔的关键字值列表，`xcm:keywords`。 每个字段值都映射到单独的关键字。 您可以使用计算字段将多个Workfront字段组合到一个以逗号分隔的文本字段中。

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### 资源

元数据在首次从Workfront推送资源时映射。 在首次将资源发送到Experience Manager Assets Essentials时，具有内置或自定义字段的文档会自动映射到指定字段。

1. 在&#x200B;**Workfront字段**&#x200B;列中，选择一个内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以将单个Workfront字段映射到多个Experience Manager Assets字段。 您无法将多个Workfront字段映射到一个Experience Manager Assets字段。

1. 在&#x200B;**Experience Manager**&#x200B;字段中，选择一个Experience Manager Assets字段。

   要将Workfront字段映射到Experience Manager Assets标记，请选择`xcm:keywords`。

1. 根据需要重复步骤1和2。
   ![启用元数据](assets/metadata-assets-essentials.png)
1. 单击&#x200B;**保存**&#x200B;或转到本文中的[设置链接文件夹（可选）](#set-up-linked-folders-optional)部分。


## 设置链接的文件夹（可选）

{{setup-linked-folder}}
