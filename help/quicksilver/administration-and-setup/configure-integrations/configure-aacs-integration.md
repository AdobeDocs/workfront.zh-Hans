---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager Assets集成
description: 您可以通过以下Adobe Experience Manager Assets集成来连接您的工作。
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 96f4d2b65aa630e86fdd4ee28b460069c5fd4987
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 0%

---

# 配置 [!UICONTROL Experience Manager Assetsas a Cloud Service] 集成

您可以在 [!DNL Experience Manager Assets]&#x200B;:

* 将资产和元数据从 [!DNL Adobe Workfront] to [!DNL Experience Manager Assets]&#x200B;
* 将资产从 [!DNL Experience Manager Assets] 到中的项目和任务 [!DNL Workfront&#x200B;]
* 便于版本控制用例
* 创建链接到的文件夹 [!DNL Experience Manager Assets]
* 跟踪资产和文件夹的元数据
* 在之间同步项目元数据 [!DNL Workfront] 和 [!DNL Experience Manager Assets]

您还可以将多个Experience Manager Assets存储库连接到一个Workfront环境，或将多个Workfront环境跨组织ID连接到一个Experience Manager Assets存储库。 对于要设置的每个集成，请按照本文中的配置说明进行操作。

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
   <td>[!UICONTROL计划]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] 许可证</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>产品</strong>
   </td>
   <td>您必须 [!DNL Experience Manager Assets as a Cloud Service]，并且您必须作为用户添加到产品中。
   </td>
  </tr>
  <tr>
   <td>访问级别配置*
   </td>
   <td>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <strong>授予用户完全管理访问权限</strong>.
   </td>
  </tr>
</table>


*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。


## 先决条件

开始之前，

* 您必须 [!DNL Workfront] 和 [!DNL Adobe Experience Manager Assets] 与 [!DNL Adobe Admin Consol]e.有关详细信息，请参阅 [基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## 设置集成信息

1. 单击 **[!UICONTROL 主菜单]** 图标，然后单击 **[!UICONTROL 设置]** .
1. 选择 **[!UICONTROL 文档]** 在左侧面板中，选择 **[!UICONTROL [!DNL Experience Manager]集成]**.
   >[!NOTE]
   >
   >此配置区域仅在 [!DNL Workfront] 环境包含在 [!DNL Adobe Admin Console].

1. 选择 **[!UICONTROL 添加 [!DNL Experience Manager] 集成]**.
1. 在 **[!UICONTROL 名称]** 字段中，输入您希望用户在Workfront和Experience Manager Assets中与此集成进行交互时看到的名称。
1. 在 **[!UICONTROL 导航URL]** 字段中，系统会自动填充导航URL。 此只读URL用于链接到贵组织的 [!DNL Experience Manager] 实例 [!UICONTROL 主菜单] 以便快速访问。
1. 从 **[!UICONTROL [!DNL Experience Manager]资产存储库]** 下拉菜单。 系统会自动填充 [!DNL Experience Manager] 与用户配置文件被分配到的组织ID关联的存储库。
   ![选择experience manager存储库](assets/setup-information.png)

1. 单击 **[!UICONTROL 保存]** 或继续 [设置元数据（可选）](#set-up-metadata-optional) 章节。

   >[!NOTE]
   >
   >由于集成的复杂性，在保存初始配置后，您无法更改存储库。

## 设置元数据（可选）

您可以映射 [!DNL Workfront] 对象数据到中的资产媒体字段 [!DNL Experience Manager] 资产。

>[!IMPORTANT]
>
>您只能在一个方向上映射元数据：从 [!DNL Workfront] to [!DNL Experience Manager]. 链接到的文档的元数据 [!DNL Workfront] 从 [!DNL Experience Manager] 无法转移到 [!DNL Workfront].

### 配置元数据字段

在开始映射元数据字段之前，必须在Workfront和Experience Manager Assets中配置元数据字段。

要配置元数据字段，请执行以下操作：

1. 在中配置元数据架构 [!DNL Experience Manager Assets] 如 [配置资产元数据在Adobe之间的映射 [!DNL Workfront] 和 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. 在Workfront中配置自定义表单字段。 [!DNL Workfront] 具有许多您可以使用的内置自定义字段。 但是，您也可以创建自己的自定义字段，如 [创建或编辑自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **展开以查看有关受支持的Workfront和Experience Manager Assets字段的更多信息**

**Experience Manager Assets标记**

您可以将任何Workfront支持的字段映射到Experience Manager Assets中的标记。 要实现此目的，您必须确保Experience Manager Assets中的标记值与Workfront匹配。

* 标记和Workfront字段值在拼写和格式上必须完全匹配。
* 映射到experience Manager Assets标记的Workfront字段值必须全部为小写，即使Experience Manager Assets中的标记似乎具有大写字母也是如此。
* Workfront字段值不得包含空格。
* Workfront中的字段值还必须包含Experience Manager Assets标记的文件夹结构。
* 要将多个单行文本字段映射到标记，请在元数据映射的Workfront侧输入以逗号分隔的标记值列表， `xcm:keywords` 在Experience Manager Assets那边。 每个字段值都映射到一个单独的标记。 您可以使用计算字段将多个Workfront字段合并为一个以逗号分隔的文本字段。
* 您可以通过输入该字段中可用值的逗号分隔列表，来映射下拉、单选按钮或复选框字段中的值。


>[!INFO]
>
>**示例**:要匹配此处文件夹结构中显示的标记，Workfront中的字段值将为 `landscapes:trees/spruce`. 在Workfront字段值中记下小写字母。
>
>如果希望标记在标记树中位于最左侧的项目，则必须后跟一个冒号。 在此示例中，要映射到风景标记，Workfront中的字段值将为 `landscapes:`.
>
>![AEM中的文件夹结构](assets/aem-folder-structure-with-red-boxes.png)


在Experience Manager Assets中创建标记后，这些标记将显示在元数据部分的标记下拉菜单下。 要将字段链接到标记，请选择 `xcm:keywords` 在元数据映射区域的Experience Manager Assets字段下拉列表中。

有关Experience Manager Assets中标记的更多信息（包括如何创建和管理标记），请参阅 [管理标记](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Experience Manager Assets自定义元数据架构字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets中的自定义元数据架构字段。

在Experience Manager Assets中创建的自定义元数据字段在元数据设置区域的其自己部分中进行组织。

![自定义元数据部分](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets。 以下字段值在大小写和Workfront和Experience Manager Assets之间的拼写中必须匹配：

* 下拉字段
* 多选字段

>[!TIP]
>
> 要检查字段值是否完全匹配，请转到
>
> * Workfront中的设置>自定义Forms或对象中的字段
> * Experience Manager Assets中的Assets >元数据架构


+++

### 映射资产元数据

从推送资产时映射元数据 [!DNL Workfront] 第一次。 首次将资产发送到时，具有内置或自定义字段的文档会自动映射到指定的字段 [!DNL Experience Manager Assets].

要映射资产的元数据，请执行以下操作：

1. 选择 **[!UICONTROL 资产]** 元数据表上方。
1. 在 **[!UICONTROL [!DNL Workfront]字段]** 列中，选择内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以映射 [!DNL Workfront] 字段输入到多个 [!UICONTROL Experience Manager Assets] 字段。 您无法映射多个 [!DNL Workfront] 字段 [!DNL Experience Manager Assets] 字段。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->


1. 在 [!DNL Experience Manager Assets] 字段中，通过预填充的类别进行搜索，或在搜索字段中输入至少两个字母以访问其他类别。
1. 根据需要重复步骤2和3。
   ![元数据字段](assets/asset-metadata.png)
1. 单击 [!UICONTROL 保存] 或继续 [文件夹](#folders) 章节。

### 映射文件夹的元数据

当用户在项目上创建链接的文件夹时，关联的项目、项目组合和项目群数据会映射到 [!DNL Experience Manager Assets].

>[!NOTE]
>
>此集成不支持 [!DNL Adobe Experience Manager].

要映射文件夹的元数据，请执行以下操作：

1. 选择 **[!UICONTROL 文件夹]** 元数据表上方。
1. 在 **[!UICONTROL [!DNL Workfront]字段]** 列中，选择内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以将单个Workfront字段映射到多个Experience Manager Assets字段。 您无法映射多个 [!DNL Workfront] 字段 [!DNL Experience Manager Assets] 字段。

1. 在 **[!DNL Experience Manager Assets]** 字段中，通过预填充的类别进行搜索，或在搜索字段中输入至少两个字母以访问其他类别。
1. 根据需要重复步骤2和3。
   ![文件夹元数据](assets/folder-metadata.png)
1. 单击 **[!UICONTROL 保存]** 或继续 [项目元数据同步](#project-metadata-sync) 章节。


### 对象元数据同步

安 [!DNL Experience Manager] 映射到的字段 [!DNL Workfront] 当字段在 [!DNL Workfront].

>[!IMPORTANT]
>
>用户必须具有中的写入权限 [!DNL Experience Manager] 对于对象中的资产，以便在更新元数据时进行同步。

1. 启用 **[!UICONTROL 同步对象元数据]** 字段。
1. 单击保存或继续 [设置链接的文件夹（可选）](#set-up-linked-folders-optional) 章节。

## 设置链接的文件夹（可选）

您可以允许用户创建链接到的文件夹 [!DNL Experience Manager] 在 [!DNL Workfront] 项目。 链接文件夹后，添加到该文件夹的任何资产都会自动显示在 [!DNL Workfront] 和 [!DNL Experience Manager]. 将资产添加到 [!DNL Workfront] 首次将资产的元数据推送到 [!DNL Experience Manager Assets].

在以下步骤中，您需要指明创建链接文件夹的位置。 每个集成只能对所有链接文件夹有一个位置。

要设置链接的文件夹，请执行以下操作：

1. 切换 **[!UICONTROL 启用链接的文件夹]** 开。
1. 选择一个文件夹路径，以指示您希望将所有关联的文件夹关联到此集成的位置。

   >[!NOTE]
   >
   >用户需要在 [!DNL Adobe Experience Manager Assets] 到为创建链接文件夹而指定的文件夹。

1. 单击&#x200B;**[!UICONTROL 保存]**。
