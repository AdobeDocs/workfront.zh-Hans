---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager Assets集成
description: 您可以将工作与以下Adobe Experience Manager Assets集成联系起来。
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 3849bd8ce80f40ae7d05b81e0dd8e846851dffc0
workflow-type: tm+mt
source-wordcount: '1504'
ht-degree: 0%

---

# 配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成

您可以将工作与您的内容关联到 [!DNL Experience Manager Assets]以&#x200B;下：

* 推送资源和元数据的来源 [!DNL Adobe Workfront] 到 [!DNL Experience Manager Assets]&#x200B;
* 链接资产来源 [!DNL Experience Manager Assets] 至您的项目和任务 [!DNL Workfront&#x200B;]
* 促进版本控制用例
* 创建链接到的文件夹 [!DNL Experience Manager Assets]
* 跟踪资源和文件夹的元数据
* 在之间同步项目元数据 [!DNL Workfront] 和 [!DNL Experience Manager Assets]

您还可以将多个Experience Manager Assets存储库连接到一个Workfront环境，或将多个Workfront环境连接到跨组织ID的一个Experience Manager Assets存储库。 对于要设置的每个集成，请按照本文中的配置说明进行操作。

## 访问要求

您必须具备以下条件：

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 计划*</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] 许可证*</strong>
   </td>
   <td>[！UICONTROL计划]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] 许可证</strong>
   </td>
   <td>[！UICONTROL标准]
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
   <td>您必须是 [!DNL Workfront] 管理员。 有关以下项的信息 [!DNL Workfront] 管理员，请参见 <strong>授予用户完全管理访问权限</strong>.
   </td>
  </tr>
</table>


*要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。


## 先决条件

开始之前，

* 您必须拥有 [!DNL Workfront] 和 [!DNL Adobe Experience Manager Assets] 与中的组织ID关联 [!DNL Adobe Admin Consol]e.欲了解更多信息，请参阅， [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 设置集成信息

1. 单击 **[!UICONTROL 主菜单]** Adobe Workfront图标，然后单击 **[!UICONTROL 设置]** .
1. 选择 **[!UICONTROL 文档]** 在左侧面板中，然后选择 **[!UICONTROL [!DNL Experience Manager]集成]**.
   >[!NOTE]
   >
   >此配置区域仅在以下情况下显示： [!DNL Workfront] 环境包含在 [!DNL Adobe Admin Console].

1. 选择 **[!UICONTROL 添加 [!DNL Experience Manager] 集成]**.
1. 在 **[!UICONTROL 名称]** 字段中，输入您希望用户在Workfront和Experience Manager Assets中与此集成交互时看到的名称。
1. 在 **[!UICONTROL 导航URL]** 字段中，系统会自动填充导航URL。 此只读URL用于链接到您组织的 [!DNL Experience Manager] 实例来自 [!UICONTROL 主菜单] 以进行快速访问。
1. 从中选择存储库 **[!UICONTROL [!DNL Experience Manager]资产存储库]** 下拉菜单。 系统会自动填充任意 [!DNL Experience Manager] 与您的用户配置文件所分配到的组织ID相关联的存储库。
   ![选择experience manager存储库](assets/setup-information.png)

1. 单击 **[!UICONTROL 保存]** 或转到 [设置元数据（可选）](#set-up-metadata-optional) 章节。

   >[!NOTE]
   >
   >由于集成的复杂性，在保存初始配置后，您将无法更改存储库。

## 设置元数据（可选）

您可以映射 [!DNL Workfront] 对象数据到中的资产媒体字段 [!DNL Experience Manager] 资产。

>[!IMPORTANT]
>
>只能在一个方向上映射元数据：从 [!DNL Workfront] 到 [!DNL Experience Manager]. 链接到的文档的元数据 [!DNL Workfront] 起始日期 [!DNL Experience Manager] 无法转移到 [!DNL Workfront].

### 配置元数据字段

在开始映射元数据字段之前，必须在Workfront和Experience Manager Assets中配置元数据字段。

要配置元数据字段，请执行以下操作：

1. 在中配置元数据架构 [!DNL Experience Manager Assets] 如中所述 [配置Adobe之间的资源元数据映射 [!DNL Workfront] 和 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. 在Workfront中配置自定义表单字段。 [!DNL Workfront] 有许多内置的自定义字段可供您使用。 但是，您也可以创建自己的自定义字段，如中所述 [创建或编辑自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **展开以查看有关支持的Workfront和Experience Manager Assets字段的更多信息**

**Experience Manager Assets标记**

您可以将任何Workfront支持的字段映射到Experience Manager Assets中的标记。 为此，您必须确保Experience Manager Assets中的标记值与Workfront匹配。

* Tags和Workfront字段值在拼写和格式上必须完全匹配。
* 映射到Experience Manager Assets标记的Workfront字段值必须全部小写，即使Experience Manager Assets中的标记似乎包含大写字母。
* Workfront字段值不得包含空格。
* Workfront中的字段值还必须包含Experience Manager Assets标记的文件夹结构。
* 要将多个单行文本字段映射到标记，请在元数据映射的Workfront端输入标记值的逗号分隔列表，并且 `xcm:keywords` 在Experience Manager Assets那边。 每个字段值都映射到单独的标记。 您可以使用计算字段将多个Workfront字段组合到一个以逗号分隔的文本字段中。
* 您可以通过输入该字段中可用值的逗号分隔列表，来映射下拉字段、单选按钮或复选框字段中的值。


>[!INFO]
>
>**示例**：要匹配此处文件夹结构中所显示的标记，Workfront中的字段值将为 `landscapes:trees/spruce`. 请注意Workfront字段值中的小写字母。
>
>如果希望标记是标记树中最左边的项目，则必须后跟一个冒号。 在此示例中，要映射到景观标记，Workfront中的字段值将为 `landscapes:`.
>
>![AEM中的文件夹结构](assets/aem-folder-structure-with-red-boxes.png)


在Experience Manager Assets中创建标记后，这些标记将显示在元数据部分的标记下拉列表下方。 要将字段链接到标记，请选择 `xcm:keywords` 在元数据映射区域的Experience Manager Assets字段下拉列表中。

有关Experience Manager Assets中的标记（包括如何创建和管理标记）的更多信息，请参阅 [管理标记](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Experience Manager Assets自定义元数据架构字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets中的自定义元数据架构字段。

在Experience Manager Assets中创建的自定义元数据字段在元数据设置区域的各自部分中进行了组织。

![自定义元数据部分](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets。 Workfront和Experience Manager Assets之间的以下字段值大小写和拼写必须匹配：

* 下拉字段
* 多选字段

>[!TIP]
>
> 要检查字段值是否完全匹配，请转到
>
> * Workfront中的“设置”>“自定义Forms”或对象中的字段
> * Experience Manager Assets中的Assets >元数据架构


+++

### 映射资源的元数据

从推送资源时进行元数据映射 [!DNL Workfront] 这是第一次。 具有内置或自定义字段的文档在首次将资产发送到时会自动映射到指定的字段 [!DNL Experience Manager Assets].

要映射资源的元数据，请执行以下操作：

1. 选择 **[!UICONTROL 资产]** 在元数据表的上方。
1. 在 **[!UICONTROL [!DNL Workfront]字段]** 列中，选择内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以映射一个 [!DNL Workfront] 字段到多个 [!UICONTROL Experience Manager Assets] 字段。 无法映射多个 [!DNL Workfront] 字段到单个 [!DNL Experience Manager Assets] 字段。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->


1. 在 [!DNL Experience Manager Assets] 字段，在预填充的类别中搜索，或在搜索字段中输入至少两个字母以访问其他类别。
1. 根据需要重复步骤2和3。
   ![元数据字段](assets/asset-metadata.png)
1. 单击 [!UICONTROL 保存] 或转到 [文件夹](#folders) 章节。

### 映射文件夹的元数据

当用户在项目中创建链接文件夹时，关联的项目、项目组合和项目群数据将映射到中的文件夹元数据字段 [!DNL Experience Manager Assets].

>[!NOTE]
>
>此集成不支持来自的自定义元数据 [!DNL Adobe Experience Manager].

要映射文件夹的元数据，请执行以下操作：

1. 选择 **[!UICONTROL 文件夹]** 在元数据表的上方。
1. 在 **[!UICONTROL [!DNL Workfront]字段]** 列中，选择内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以将一个Workfront字段映射到多个Experience Manager Assets字段。 无法映射多个 [!DNL Workfront] 字段到单个 [!DNL Experience Manager Assets] 字段。

1. 在 **[!DNL Experience Manager Assets]** 字段，在预填充的类别中搜索，或在搜索字段中输入至少两个字母以访问其他类别。
1. 根据需要重复步骤2和3。
   ![文件夹元数据](assets/folder-metadata.png)
1. 单击 **[!UICONTROL 保存]** 或转到 [项目元数据同步](#project-metadata-sync) 章节。


### 对象元数据同步

An [!DNL Experience Manager] 映射到的字段 [!DNL Workfront] 项目组合、项目群、项目、任务、问题和文档字段更改后会自动更新 [!DNL Workfront].

>[!IMPORTANT]
>
>用户必须具有写入权限 [!DNL Experience Manager] 用于位于对象中的资产，以便元数据在更新时同步。

1. 启用 **[!UICONTROL 同步对象元数据]** 字段。
1. 单击 **保存** 或转到 [设置工作流（可选）](#set-up-workflows-optional) 章节。

<!--Courtney start here-->

## 设置工作流（可选）

工作流是一组将Workfront连接到Adobe Experience Manager as a Cloud Service的操作。 作为Workfront管理员，您可以在Workfront中配置工作流，然后将其分配给项目模板。 使用为其分配了工作流的项目模板创建项目时，将触发在工作流中定义的操作。

您可以在项目模板和项目级别覆盖在集成中设置的默认工作流值。

### 设置用于创建Adobe Experience Manager链接文件夹的工作流

1. 切换 **[!UICONTROL 创建链接文件夹]** 打开。
1. 选择文件夹路径，以指示要将所有链接文件夹与此集成关联的位置。
   ![链接的文件夹导航](assets/select-folder-aem-integration.png)
1. 启用 **附加Portfolio和项目群名称** 选项，用于在链接文件夹名称的末尾自动包含Portfolio和项目群名称。
1. 单击 **保存** 或转到 [设置链接文件夹（可选）](#set-up-linked-folders-optional) 章节。

<!--Courtney end here-->

## 设置链接文件夹（可选）

您可以允许用户创建链接到的文件夹 [!DNL Experience Manager] 当在 [!DNL Workfront] 项目。 链接文件夹后，添加到该文件夹的任何资产都会自动显示在两者中 [!DNL Workfront] 和 [!DNL Experience Manager]. 将资产添加到中的链接文件夹时 [!DNL Workfront] 资产元数据首次被推送到 [!DNL Experience Manager Assets].

在下面的步骤中，您将指示希望创建链接文件夹的位置。 对于所有链接的文件夹，每个集成只能有一个位置。

要设置链接的文件夹，请执行以下操作：

1. 切换 **[!UICONTROL 启用链接的文件夹]** 打开。
1. 选择文件夹路径，以指示要将所有链接文件夹与此集成关联的位置。

   >[!NOTE]
   >
   >用户需要写入权限 [!DNL Adobe Experience Manager Assets] 到指定用于创建链接文件夹的文件夹。

1. 单击&#x200B;**[!UICONTROL 保存]**。
