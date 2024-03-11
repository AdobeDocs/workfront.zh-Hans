---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: 配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成
description: 您可以将工作与您的内容关联到 [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 54ece5a3082264af80d6a720452f8afe5e99c868
workflow-type: tm+mt
source-wordcount: '1763'
ht-degree: 0%

---

# 配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成

<!-- Audited: 1/2024 -->

<span class="preview">此页面上高亮显示的信息是指尚未普遍可用的功能。 它仅在预览Sandbox环境中可用。</span>

>[!IMPORTANT]
>
>此功能仅适用于已载入到 [!DNL Adobe Admin Console].

您可以将工作与您的内容关联到 [!DNL Experience Manager Assets]下&#x200B;列：

* 从推送资源和元数据 [!DNL Adobe Workfront] 到 [!DNL Experience Manager Assets]&#x200B;AEM
* 链接资产来源 [!DNL Experience Manager Assets] 中的项目和任务 [!DNL Workfront&#x200B;]
* 促进版本控制用例
* 创建链接到的文件夹 [!DNL Experience Manager Assets]
* 跟踪资源和文件夹的元数据
* 同步项目元数据 [!DNL Workfront] 和 [!DNL Experience Manager Assets]

>[!NOTE]
>
>您还可以连接多个 [!DNL Experience Manager Assets] 将存储库合并到一个 [!UICONTROL Workfront] 环境或多个 [!DNL Workfront] 环境到一个 [!DNL Experience Manager Assets] 跨组织ID的存储库 对于要设置的每个集成，请按照本文中的配置说明进行操作。

## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 计划</strong>
   </td>
   <td>任何
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 许可证</strong>
   </td>
   <td>当前： [！UICONTROL计划] <br>
   新文档： [！UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] 许可证</strong>
   </td>
   <td>[！UICONTROL标准版]
   </td>
  </tr>
  <tr>
   <td><strong>产品</strong>
   </td>
   <td>您必须拥有 [!DNL Experience Manager Assets as a Cloud Service]，并且您必须作为用户添加到产品中。
   </td>
  </tr>
  <tr>
   <td>访问级别配置*
   </td>
   <td>您必须是 [!DNL Workfront] 管理员。
   </td>
  </tr>
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## 先决条件

开始之前，

* 您必须拥有 [!DNL Workfront] 和 [!DNL Adobe Experience Manager Assets] 与中的组织ID关联 [!DNL Adobe Admin Console]. 有关详细信息，请参阅， [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 设置集成信息

{{step-1-to-setup}}

1. 选择 **[!UICONTROL 文档]** 在左侧面板中，然后选择 **[!UICONTROL [!DNL Experience Manager]集成]**.

   >[!NOTE]
   >
   >此配置区域仅在以下情况下显示： [!DNL Workfront] 环境包含在 [!DNL Adobe Admin Console].

1. 选择 **[!UICONTROL 添加 [!DNL Experience Manager] 集成]**.
1. 在 **[!UICONTROL 名称]** 字段中，输入您希望用户在Workfront和Experience Manager Assets中与此集成交互时看到的名称。
1. 在 **[!UICONTROL 导航URL]** 字段中，系统会自动填充导航URL。 此只读URL用于链接到您组织的 [!DNL Experience Manager] 实例来自 [!UICONTROL 主菜单] 以进行快速访问。
1. 从中选择存储库 **[!UICONTROL [!DNL Experience Manager]资产存储库]** 下拉菜单。 系统会自动填充 [!DNL Experience Manager] 与您的用户配置文件所分配到的组织ID关联的存储库。
   ![选择experience manager存储库](assets/setup-information.png)

1. 单击 **[!UICONTROL 保存]** 或转到 [设置元数据（可选）](#set-up-metadata-optional) 部分。

   >[!NOTE]
   >
   >由于集成的复杂性，您在保存初始配置后无法更改存储库。

## 设置元数据（可选）

您可以映射 [!DNL Workfront] 对象数据到中的资产媒体字段 [!DNL Experience Manager] 资产。

>[!IMPORTANT]
>
>只能在一个方向上映射元数据：从 [!DNL Workfront] 到 [!DNL Experience Manager]. 链接到的文档的元数据 [!DNL Workfront] 从 [!DNL Experience Manager] 无法转移到 [!DNL Workfront].

### 配置元数据字段

在开始映射元数据字段之前，必须在Workfront和Experience Manager Assets中配置元数据字段。

要配置元数据字段，请执行以下操作：

1. 在中配置元数据架构 [!DNL Experience Manager Assets] 如中所述 [配置Adobe之间的资源元数据映射 [!DNL Workfront] 和 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. 在Workfront中配置自定义表单字段。 [!DNL Workfront] 有许多内置的自定义字段可供您使用。 但是，您也可以创建自己的自定义字段，如中所述 [创建或编辑自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **展开以查看有关支持的Workfront和Experience Manager Assets字段的更多信息**

**Experience Manager Assets标记**

您可以将任何Workfront支持的字段映射到Experience Manager Assets中的标记。 为此，您必须确保Experience Manager Assets中的标记值与Workfront匹配。

* 标记和Workfront字段值在拼写和格式上必须完全匹配。
* 映射到Workfront assets标记的Experience Manager字段值必须全部小写，即使Experience Manager Assets中的标记似乎包含大写字母。
* Workfront字段值不得包含空格。
* Workfront中的字段值还必须包含Experience Manager Assets标记的文件夹结构。
* 要将多个单行文本字段映射到标记，请在元数据映射的Workfront端输入一个以逗号分隔的标记值列表，并且 `xcm:keywords` 在Experience Manager Assets那边。 每个字段值都映射到单独的标记。 您可以使用计算字段将多个Workfront字段组合到一个以逗号分隔的文本字段中。
* 您可以通过输入该字段中可用值的逗号分隔列表，来映射下拉字段、单选按钮或复选框字段中的值。


>[!INFO]
>
>**示例**：要匹配此处文件夹结构中显示的标记，Workfront中的字段值将为 `landscapes:trees/spruce`. 请注意Workfront字段值中的小写字母。
>
>如果希望标记是标记树中最左边的项目，则必须后跟一个冒号。 在本例中，要映射到景观标记，Workfront中的字段值将为 `landscapes:`.
>
>![AEM中的文件夹结构](assets/aem-folder-structure-with-red-boxes.png)


在Experience Manager Assets中创建标记后，这些标记将显示在元数据部分的标记下拉列表下。 要将字段链接到标记，请选择 `xcm:keywords` 在元数据映射区域的Experience Manager Assets字段下拉列表中。

有关Experience Manager Assets中的标记（包括如何创建和管理标记）的更多信息，请参阅 [管理标记](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Experience Manager Assets自定义元数据架构字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets中的自定义元数据架构字段。

在Experience Manager Assets中创建的自定义元数据字段在元数据设置区域的相应部分中进行了组织。

![自定义元数据部分](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets。 Workfront和Experience Manager Assets之间的以下字段值的大小写和拼写必须匹配：

* 下拉字段
* 多选字段

>[!TIP]
>
> 要检查字段值是否完全匹配，请转到
>
> * Workfront中的设置>自定义Forms或对象中的字段
> * Experience Manager Assets中的Assets >元数据架构

+++

### 映射资源的元数据

从推送资产时进行元数据映射 [!DNL Workfront] 这是第一次。 具有内置或自定义字段的文档在首次将资产发送到时会自动映射到指定字段 [!DNL Experience Manager Assets].

要映射资源的元数据，请执行以下操作：

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. 在 **[!UICONTROL [!DNL Workfront]字段]** 列中，选择一个内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以映射单个 [!DNL Workfront] 字段到多个 [!UICONTROL Experience Manager Assets] 字段。 无法映射多个 [!DNL Workfront] 字段到单个 [!DNL Experience Manager Assets] 字段。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. 在 [!DNL Experience Manager Assets] 字段，在预填充的类别中进行搜索，或在搜索字段中输入至少两个字母以访问其他类别。
1. 根据需要重复步骤2和3。
   ![元数据字段](assets/metadata-no-asset-toggle.png)
1. 单击 [!UICONTROL 保存] 或转到 [设置工作流](#set-up-workflows-optional) 部分。

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## 设置工作流（可选）

工作流是一组将Workfront连接到Adobe Experience Manager as a Cloud Service的操作。 作为Workfront管理员，您可以在Workfront中配置工作流，然后将其分配给项目模板。 使用为其分配工作流的项目模板创建项目时，会触发工作流中定义的操作。

可以为整个Adobe Experience Manager启用和配置工作流。 然后，可以将这些工作流应用于项目模板，并在模板或项目级别进行调整或自定义。

Adobe Experience Manager集成中提供了以下工作流：

* [创建Adobe Experience Manager链接文件夹](#create-adobe-experience-manager-linked-folders)
* [发布发送到Adobe Experience Manager Assets的资源](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### 创建Adobe Experience Manager链接文件夹

1. 切换 **[!UICONTROL 创建链接文件夹]** 打开。
1. 选择文件夹路径以指示要将所有链接文件夹与此集成关联的位置。
   ![链接的文件夹导航](assets/select-folder-aem-integration.png)
1. 启用 **[!UICONTROL 附加Portfolio和程序名称]** 选项，用于在链接文件夹名称的末尾自动包含Portfolio和项目名称。
1. 单击 **[!UICONTROL 保存]** 或转到 [发布发送到Adobe Experience Manager Assets的资源](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) 部分。

在预览Sandbox环境中

<div class="preview">

1. 切换 **[!UICONTROL 创建链接文件夹]** 打开。
1. 输入正在创建的链接文件夹的名称。
1. （视情况而定）启用 **默认文件夹树** 选项，适用于希望此链接文件夹成为使用使用此集成的模板创建的项目的默认文件夹。 您可以选择一个或多个默认文件夹。
1. 选择文件夹路径以指示要将所有链接文件夹与此集成关联的位置。
1. （视情况而定）要将文件夹树（嵌套文件夹）添加到此集成，请执行以下操作：

   1. 单击 **添加文件夹** 图标 ![添加文件夹](assets/add-folder-aem.png).
   1. 在 **名称类型** 字段中，选择命名文件夹的方式：

      * **名称**：键入文件夹的名称。
      * **对象数据**：选择文件夹名称的源，如项目名称。

      >[!NOTE]
      >
      >* 文件夹名称必须少于100个字符。
      >* 将从文件夹名称中删除以下字符：
      >
      >   `/`， `:`， `[`， `]`， `|`， `*`

   1. 要将嵌套文件夹添加到文件夹树，请单击要在其中创建嵌套文件夹的文件夹旁边的三个点菜单，然后选择 **添加文件夹**. 按照上一步骤中的说明填写字段。
   1. 要将文件夹链接到Workfront，请选择该文件夹，然后单击 **制作链接的文件夹**   图标 ![链接文件夹](assets/link-folder.png).
   1. （可选）要编辑文件夹，请选择该文件夹并单击 **编辑文件夹** 图标 ![“编辑”图标](assets/edit-icon.png).
   1. （可选）要删除文件夹，请选择该文件夹并单击 **删除文件夹** 图标 ![删除文件夹](assets/delete-folder.png).
1. （视情况而定）要添加其他文件夹树，请单击 **+添加文件夹树** 并按照步骤5中的步骤执行操作。

1. 单击 **[!UICONTROL 保存]**，或转到 [发布发送到Adobe Experience Manager Assets的资源](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) 部分。

>[!NOTE]
>
>* 此集成创建的文件夹数不会超过100个，这与创建的文件夹树数量无关。 例如，与4个文件夹树集成最多可创建100个文件夹，而不是400个文件夹。
>* 文件夹树中的第一个文件夹会自动标记为已链接到Workfront。 如果不希望链接此文件夹，可以取消其链接。
>* 如果未提供文件夹树，则根文件夹将变为链接的文件夹。


</div>

### 发布发送到Adobe Experience Manager Assets的资源

1. 打开 **[!UICONTROL 自动发布资源]**.
1. 选中要发布发送到Adobe Experience Manager资源的资源的位置旁边的框。 您可以启用任一选项或同时启用两个选项。
1. （视情况而定）如果已启用Brand Portal选项，请选择要发布资源的Brand Portal 。
1. 单击 **[!UICONTROL 保存]** 或转到 [设置链接的文件夹（可选）](#set-up-linked-folders-optional) 部分。

## 设置链接的文件夹（可选）

您可以允许用户创建链接到的文件夹 [!DNL Experience Manager] 在 [!DNL Workfront] 项目。 链接文件夹时，添加到该文件夹的任何资产都会自动显示在两者中 [!DNL Workfront] 和 [!DNL Experience Manager]. 将资产添加到中链接的文件夹时 [!DNL Workfront] 资产元数据首次被推送到 [!DNL Experience Manager Assets].

在以下步骤中，您将指明创建链接文件夹的位置。 每个集成只能有一个位置用于所有链接的文件夹。

要设置链接的文件夹，请执行以下操作：

1. 切换 **[!UICONTROL 启用链接的文件夹]** 打开。
1. 选择文件夹路径以指示要将所有链接文件夹与此集成关联的位置。

   >[!NOTE]
   >
   >用户需要写入权限 [!DNL Adobe Experience Manager Assets] 到指定用于创建链接文件夹的文件夹。

1. 单击&#x200B;**[!UICONTROL 保存]**。
