---
title: 配置文档集成
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 作为Adobe Workfront管理员，您可以配置文档集成以管理Workfront中的文档。
author: Courtney, Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 7f24186c8803237a6f5116293b3c6a5fd1ea90f6
workflow-type: tm+mt
source-wordcount: '1125'
ht-degree: 1%

---

# 配置文档集成

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作为[!DNL Adobe Workfront]管理员，您可以配置文档集成以管理[!UICONTROL Workfront]中的文档。 您还可以配置[!UICONTROL Workfront]，使文档仅存储在文档服务应用程序中，而不存储在[!UICONTROL Workfront]本身中。 有关详细信息，请参阅[从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[更新文档，并将文档从[!UICONTROL Workfront]链接到外部云提供商](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider)。

>[!NOTE]
>
>列入允许列表若要允许[!DNL Workfront Proof]与[!DNL Workfront]服务器之间的开放通信，您可能需要将某些IP地址添加到您的。 有关详细信息，请参阅[配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [！UICONTROL Standard]</p>
       <p>或</p>
       <p>当前： [！UICONTROL计划]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是[!DNL Workfront]管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 受支持的集成

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以配置以下集成来管理文档：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  从[!DNL Workfront Proof]链接校对允许您在[!DNL Workfront]内提供原本在[!DNL Workfront Proof]内创建的校对。 对于当前计划，需要[!UICONTROL Pro] [!DNL Workfront]计划或更高版本才能使用此功能。 对于新计划，此功能可用于所有计划。 有关各种可用计划的详细信息，请参阅[Workfront计划](https://business.adobe.com/products/workfront/pricing.html)。

* [!DNL Microsoft SharePoint]

  有关与[!DNL SharePoint]集成的信息，请参阅[配置 [!DNL SharePoint] 集成](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md)。

* 第三方云文档提供商：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google驱动器]
   * Quip

  >[!TIP]
  >
  >您可以验证和批准从外部云提供商链接的文档，就像验证和批准直接上传到[!DNL Workfront]的文档一样。

* 其他文档提供程序（通过自定义文档集成）。

  对于当前计划，需要[!UICONTROL Pro] [!DNL Workfront]计划或更高版本才能使用此功能。 对于新计划，此功能可用于所有计划。 有关各种可用计划的详细信息，请参阅[Workfront计划](https://business.adobe.com/products/workfront/pricing.html)。

此外，您还可以通过第三方DAM集成来增强[!DNL Workfront]文档体验。 管理员必须启用这些功能，用户才能将服务链接到其[!DNL Workfront]帐户。

## 配置集成以管理文档

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 云提供商]。**

1. （可选）要将文档存储在文档服务应用程序中，而不是存储在[!DNL Workfront]中，请选择&#x200B;**[!UICONTROL 阻止用户在[!DNL Workfront]]中存储文档。**

1. 选择要启用的集成。
1. 单击&#x200B;**[!UICONTROL 保存]**。

如果您正在设置与[!DNL Workfront DAM]的集成，则可以启用[!DNL Workfront]以将元数据与文档包含在内。 有关映射元数据的信息，请参阅[设置元数据映射](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md)。

## 配置自定义文档集成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自定义文档集成允许[!DNL Workfront]用户将文件链接到几乎任何系统的[!DNL Workfront]，前提是该系统能够与[!DNL Workfront]配合使用。

要使自定义集成可供用户使用，您首先需要构建集成。 有关如何生成与[!DNL Workfront]一起使用的集成的信息，请参阅[文档Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md)。

构建自定义文档集成后，您可以将其提供给网站上的用户。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 自定义集成]**。

1. 单击&#x200B;**[!UICONTROL 添加自定义集成]**。
1. 输入以下信息以配置集成：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名称]</td> 
      <td>自定义集成的名称。 这是用户在Workfront中使用集成时看到的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL基本API URL] </td> 
      <td>API调用的基本HTTP或安全HTTP URL。 例如， <code>https://&lt;documentprovider&gt;.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL身份验证类型]</td> 
      <td> <p>对自定义集成进行授权的API调用时要使用的身份验证方法。</p> 
       <ul> 
        <li>如果选择<strong>[！UICONTROL OAuth]</strong>，请继续执行步骤5。</li> 
        <li>如果选择<strong>[！UICONTROL ApiKey]</strong>，请继续执行步骤6。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果您为&#x200B;**[!UICONTROL 身份验证类型]**&#x200B;选择了&#x200B;**[!UICONTROL OAuth]**&#x200B;身份验证，请输入以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL身份验证URL]</td> 
      <td>用于用户身份验证的完整URL。 在OAuth配置过程中，[!DNL Workfront]将用户导航到此地址。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL令牌端点URL]</td> 
      <td>用于检索 OAuth 令牌的完整 API URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL客户端ID]</td> 
      <td>此集成的OAut客户端ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL客户端密钥]</td> 
      <td>此集成的OAut客户端密钥</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL请求参数]</td> 
      <td> <p>输入要附加到每个API调用的查询字符串的可选值。 例如，access_type=offline。</p> <p>要添加多个请求参数，请单击<strong>+添加请求参数</strong>。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >显示在[!UICONTROL 自定义集成]页底部的[!DNL Workfront]重定向URI列出了用于向外部文档提供程序注册此集成的URI。

1. （视情况而定）如果您为&#x200B;**[!UICONTROL 身份验证类型]**&#x200B;选择了&#x200B;**[!UICONTROL ApiKey]**&#x200B;身份验证，请输入由自定义文档提供程序颁发的API密钥。

   [!DNL Workfront]使用此API密钥向文档提供商进行授权的API调用。

1. 单击&#x200B;**[!UICONTROL 保存]**&#x200B;以创建集成。

## 使用文档集成

有关用户如何使用验证的信息，请参阅[创建验证](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md)。

有关用户如何在配置第三方文档集成后使用这些集成的信息，请参阅[链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)。

### 将[!DNL Workfront]配置为将元数据发送到[!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

将文档从[!DNL Workfront]发送到[!DNL Workfront DAM]时，您还可以发送与该文档关联的信息。 有关文档的信息作为元数据映射到[!DNL Workfront DAM]。

信息仅单向映射，从[!DNL Workfront]到[!DNL Workfront DAM]，并且仅在文档上载到[!DNL Workfront DAM]时传输。 将来对Workfront字段所做的任何更改都不会在上传文档后更新[!DNL Workfront DAM]中的元数据字段。\
您可以将同一[!DNL Workfront]字段映射到各种[!DNL Workfront DAM]字段，但不能对多个[!DNL Workfront]字段使用同一[!DNL Workfront DAM]字段。

如果您必须配置多个[!DNL Workfront]字段以导出到一个[!DNL Workfront DAM]字段，请先在[!DNL Workfront]中创建计算自定义字段以显示对象的所有单个自定义字段。 然后，将计算的[!DNL Workfront]字段映射到一个[!DNL Workfront DAM]字段。\
有关计算自定义字段的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

该映射会影响任何用户从[!DNL Workfront]上传到[!UICONTROL Workfront] DAM的所有文档。

作为[!DNL Workfront]管理员，您必须在Workfront中启用[!DNL Workfront DAM]，然后才能映射元数据映射过程的字段。

要将[!DNL Workfront]配置为将元数据发送到[!DNL Workfront DAM]，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**。

1. 在&#x200B;**[!UICONTROL 选择要映射的Source字段]**&#x200B;字段中，开始输入要映射到[!DNL Workfront DAM]的Workfront字段的名称，然后在列表中看到该字段时将其选定。
1. 在&#x200B;**[!UICONTROL 选择要映射的目标字段]**&#x200B;中，选择要使用选定[!DNL Workfront]字段中的信息填充的[!DNL Workfront DAM]字段。

   >[!NOTE]
   >
   > 有权发送给[!DNL Workfront DAM]的用户在将其元数据上传到[!DNL Workfront DAM]时，会使用映射到此处的[!DNL Workfront]字段更新其元数据。

1. 单击&#x200B;**[!UICONTROL 添加映射]**。

1. 继续添加更多[!UICONTROL Workfront]字段和相应的[!DNL Workfront DAM]字段。

### 删除映射字段

{{step-1-to-setup}}

1. 展开&#x200B;**[!UICONTROL 文档]**，然后单击&#x200B;**[!UICONTROL 元数据映射]**。

1. 在字段列表中，选择要从元数据映射中删除的任何字段。
1. 单击&#x200B;**[!UICONTROL 删除]**。

   这些字段将从元数据映射中删除，并且其中包含的信息不会随上载的文档一起传输到[!DNL Workfront DAM]。


## 限制

* Google Drive文档集成支持从Google Drive的“我的驱动器”区域添加文件夹和图像。 无法从共享驱动器添加文件夹或映像。 了解有关[Google共享驱动器](https://support.google.com/a/users/answer/7212025?hl=en)的更多信息。