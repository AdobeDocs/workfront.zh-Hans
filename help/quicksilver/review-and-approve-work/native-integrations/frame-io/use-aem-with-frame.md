---
product-area: documents
navigation-topic: approvals
title: 将Adobe Experience Manager与Frame.io集成一起使用
description: 将Adobe Experience Manager与Frame.io集成一起使用
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cb2a17991a5562c6e734eaa0ada781d706dc5a77
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---


# 将Adobe Experience Manager与Frame.io集成一起使用

您可以使用&#x200B;[!DNL Experience Manager Assets]&#x200B;管理和存储已过审阅和批准周期的数字资产。 此集成允许您利用Adobe Experience Manager、Frame.io和Workfront的功能来简化内容管理和协作流程。

## 配置Experience Manager Assets集成

您可以在&#x200B;[!DNL Experience Manager Assets]中将您的工作与您的内容连接起来：

* 将资源和元数据从[!DNL Adobe Workfront]推送到[!DNL Experience Manager Assets]&#x200B;
* 促进版本控制用例
* 跟踪资源的元数据
* 在[!DNL Workfront]和[!DNL Experience Manager Assets]之间同步项目元数据

>[!NOTE]
>
>您还可以跨组织ID将多个[!DNL Experience Manager Assets]存储库连接到一个[!UICONTROL Workfront]环境，或将多个[!DNL Workfront]环境连接到一个[!DNL Experience Manager Assets]存储库。 对于要设置的每个集成，请按照本文中的配置说明进行操作。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table>
  <tr>
   <td>Adobe Workfront包
   </td>
   <td> <p>Prime或Ultimate</p>
    <p>工作流 Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront许可证
   </td>
   <td>
  <p>要配置集成，请执行以下操作：</p>
   <p>标准</p>
   <p>规划</p>

<p>要将文档发送到Experience Manager Assets，请执行以下操作：</p>
   <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Adobe Experience Manager许可证
   </td>
   <td>标准
   </td>
  </tr>
  <tr>
   <td>其他产品
   </td>
   <td>您必须具有[!DNL Experience Manager Assets as a Cloud Service]，并且您必须作为用户添加到产品中。
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

## 先决条件

开始之前，

* 您必须在[!DNL Workfront]中将[!DNL Adobe Experience Manager Assets]和[!DNL Adobe Admin Console]与组织ID关联。 有关详细信息，请参阅[基于平台的管理差异([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。
* 您的Workfront实例必须使用Adobe企业存储。


## 设置集成信息

{{step-1-to-setup}}

1. 在左侧面板中选择&#x200B;**[!UICONTROL 文档]**，然后选择&#x200B;**[!UICONTROL [!DNL Experience Manager]集成]**。
1. 选择&#x200B;**[!UICONTROL 添加[!DNL Experience Manager]集成]**。
1. 在&#x200B;**[!UICONTROL 名称]**&#x200B;字段中，输入您希望用户在Workfront和Experience Manager Assets中与此集成交互时看到的名称。
1. 在&#x200B;**[!UICONTROL 导航URL]**&#x200B;字段中，系统会自动填充导航URL。 此只读URL用于从[!DNL Experience Manager]主菜单[!UICONTROL 链接到组织的]实例，以进行快速访问。
1. 从&#x200B;**[!UICONTROL [!DNL Experience Manager]Assets存储库]**&#x200B;下拉菜单中选择一个存储库。 系统会自动填充与您的用户配置文件所分配到的组织ID关联的任何[!DNL Experience Manager]存储库。
   ![选择Experience Manager存储库](assets/setup-information.png)

1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;或转到本文中的[设置元数据（可选）](#set-up-metadata-optional)部分。

   >[!IMPORTANT]
   >
   >由于集成的复杂性，您在保存初始配置后无法更改存储库。


## 设置元数据（可选）

您可以将[!DNL Workfront]对象数据映射到[!DNL Experience Manager] Assets中的资源媒体字段。

>[!NOTE]
>
>只能在一个方向上映射元数据：从[!DNL Workfront]到[!DNL Experience Manager]。 从[!DNL Workfront]链接到[!DNL Experience Manager]的文档的元数据无法传输到[!DNL Workfront]。

### 配置元数据字段

在开始映射元数据字段之前，必须在Workfront和Experience Manager Assets中配置元数据字段。

要配置元数据字段，请执行以下操作：

1. 在[!DNL Experience Manager Assets]中配置元数据架构，如[配置Adobe [!DNL Workfront] 和 [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping)之间的资源元数据映射中所述。


1. 在Workfront中配置自定义表单字段。 [!DNL Workfront]有许多您可以使用的内置自定义字段。 但是，您也可以创建自己的自定义字段，如[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)中所述。

+++ **展开以查看有关支持的Workfront和Experience Manager Assets字段的更多信息** 

**Experience Manager Assets标记**

您可以将任何Workfront支持的字段映射到Experience Manager Assets中的标记。 为此，您必须确保Experience Manager Assets中的标记值与Workfront匹配。

* 标记和Workfront字段值在拼写和格式上必须完全匹配。
* 映射到Workfront assets标记的Experience Manager字段值必须全部小写，即使Experience Manager Assets中的标记似乎包含大写字母。
* Workfront字段值不得包含空格。
* Workfront中的字段值还必须包含Experience Manager Assets标记的文件夹结构。
* 要将多个单行文本字段映射到标记，请在元数据映射的Workfront端和Experience Manager Assets端分别输入一个以逗号分隔的标记值列表，`xcm:keywords`。 每个字段值都映射到单独的标记。 您可以使用计算字段将多个Workfront字段组合到一个以逗号分隔的文本字段中。
* 您可以通过输入该字段中可用值的逗号分隔列表，来映射下拉字段、单选按钮或复选框字段中的值。


>[!INFO]
>
>**示例**：要匹配此处文件夹结构中显示的标记，Workfront中的字段值应为`landscapes:trees/spruce`。 请注意Workfront字段值中的小写字母。
>
>如果希望标记是标记树中最左边的项目，则必须后跟一个冒号。 在此示例中，要映射到景观标记，Workfront中的字段值将为`landscapes:`。
>
>AEM中的![文件夹结构](assets/aem-folder-structure-with-red-boxes.png)


在Experience Manager Assets中创建标记后，这些标记将显示在元数据部分的标记下拉列表下。 要将字段链接到标记，请在元数据映射区域的Experience Manager Assets字段下拉列表中选择`xcm:keywords`。

有关Experience Manager Assets中的标记（包括如何创建和管理标记）的更多信息，请参阅[管理标记](https://experienceleague.adobe.com/zh-hans/docs/experience-manager-64/administering/contentmanagement/tags)。

**Experience Manager Assets自定义元数据架构字段**

您可以将内置和自定义Workfront字段映射到Experience Manager Assets中的自定义元数据架构字段。

在Experience Manager Assets中创建的自定义元数据字段在元数据设置区域的相应部分中进行了组织。

![自定义元数据节](assets/custom-metadata.png)

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

首次从[!DNL Workfront]推送资产时元数据映射。 具有内置或自定义字段的文档在首次将资源发送到[!DNL Experience Manager Assets]时自动映射到指定的字段。

要映射资源的元数据，请执行以下操作：

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. 在&#x200B;**[!UICONTROL [!DNL Workfront]字段]**&#x200B;列中，选择一个内置或自定义Workfront字段。

   >[!NOTE]
   >
   >您可以将单个[!DNL Workfront]字段映射到多个[!UICONTROL Experience Manager Assets]字段。 您无法将多个[!DNL Workfront]字段映射到单个[!DNL Experience Manager Assets]字段。
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. 在[!DNL Experience Manager Assets]字段中，搜索预填充的类别，或在搜索字段中输入至少两个字母以访问其他类别。
1. 根据需要重复步骤2和3。
   ![元数据字段](assets/metadata-no-asset-toggle.png)
1. 单击&#x200B;[!UICONTROL **保存**]&#x200B;或移动到本文中的[对象元数据同步](#object-metadata-sync)部分。



### 对象元数据同步

映射到[!DNL Experience Manager]项目组合、计划、项目、任务、问题和文档字段的[!DNL Workfront]字段在[!DNL Workfront]中更改该字段时会自动更新。

启用此选项后，任何已推送到Adobe Experience Manager的资源都会在Workfront的“文档详细信息”页面上显示文档Adobe Experience Manager元数据的实时视图。

1. 启用&#x200B;**[!UICONTROL 同步对象元数据]**&#x200B;字段，然后单击&#x200B;**保存**。

>[!IMPORTANT]
>
>用户必须在[!DNL Experience Manager]中拥有对象中资产的写入权限，元数据才能在更新时同步。


## 将文档发送到Experience Manager Assets或Assets Essentials

您可以将文档从Workfront发送到Experience Manager Assets或Assets Essentials。 从Workfront上传并发送到Assets Essentials的文档仍会计入您的总体文档存储中。

通过此集成发送到Experience Manager的Assets具有&#x200B;**5 GB**&#x200B;的大小限制。

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

在将资源从Workfront发送到Experience Manager Assets或Assets Essentials时，首先映射元数据字段。 配置为映射父对象的任何元数据也会发送。 有关配置元数据映射的详细信息，请参阅[配置Experience Manager Assets as a Cloud Service集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)或[配置Experience Manager Assets Essentials集成](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)。

>[!INFO]
>
>**示例**&#x200B;首次发送附加到项目的资源时，元数据将映射到Experience Manager Assets或Assets Essentials以及父对象（例如项目组合和项目群）中的任何映射元数据。



### 从Workfront发送文档

当用户将文档从Workfront发送到Experience Manager Assets或Assets Essentials时，映射的元数据将沿文档传输。 发送文档后，在Workfront中对文档元数据所做的更改不会反映在Assets或Assets Essentials中。 如果Workfront中的映射字段发生更改，您必须将包含更新后元数据的文档的新版本发送到Assets或Assets Essentials。

要发送文档，请执行以下操作：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后选择要发送的文档。
1. 单击&#x200B;**发送至**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Assets或Assets Essentials。

   ![发送至](assets/send-to-aem.png)

1. 选择要将资源放置到的位置，然后单击&#x200B;**选择文件夹**。
1. 找到所需目标后，单击&#x200B;**保存**。

### 发送新版本

您可以向先前上载到Workfront的文档中添加新版本。 有关详细信息，请参阅[上载文档的新版本](/help/quicksilver/documents/managing-documents/upload-new-document-version.md)。 上传最新版本后，可将其发送到Assets Essentials。 如果Workfront中的映射字段已更改，则新版本会在发送时更新Assets Essentials中的元数据。

>[!IMPORTANT]
>
>在将新版本上传到Workfront之前，我们建议重命名文件。 如果上传的文件名与以前版本完全相同，则只能从Workfront下载最新版本。 无论文件名如何，均可从Experience Manager Assets或Assets Essentials下载所有版本。<!--Is this still a thing with ESM?-->

发送最新版本：

1. 转到Workfront中的&#x200B;**文档**&#x200B;区域，然后找到该文档。
1. 选择&#x200B;**发送至**，然后选择管理员设置的Experience Manager集成。

   >[!NOTE]
   >
   >Workfront管理员可以选择此集成的任何名称，因此可能没有特别提及Assets或Assets Essentials。

   ![发送至](assets/send-to-aem.png)

1. 单击 **Save**。新版本将保存在与先前版本相同的位置。
