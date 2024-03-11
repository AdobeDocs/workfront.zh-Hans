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
source-git-commit: a243094dc6bbbe71a6efdb4fe99f7365daae514d
workflow-type: tm+mt
source-wordcount: '1106'
ht-degree: 1%

---

# 配置文档集成

<!-- Audited: 12/2023 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作为 [!DNL Adobe Workfront] 管理员，您可以配置文档集成以管理中的文档 [!UICONTROL Workfront]. 您还可以配置 [!UICONTROL Workfront] 因此文档仅存储在文档服务应用程序中，而不存储在 [!UICONTROL Workfront] 本身。 有关更多信息，请参阅 [更新并链接文档 [!UICONTROL Workfront] 到外部云提供商](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#update-and-link-a-document-from-workfront-to-an-external-cloud-provider) 在 [链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>要允许开放通信，请执行以下操作： [!DNL Workfront Proof] 和 [!DNL Workfront] 服务器中，您可能需要将某些IP地址添加到允许列表中。 有关更多信息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 访问要求

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
   <td> <p>您必须是 [!DNL Workfront] 管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 受支持的集成

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以配置以下集成来管理文档：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

  链接校样从 [!DNL Workfront Proof] 允许您创建最初在中创建的验证 [!DNL Workfront Proof] 可用范围 [!DNL Workfront]. 对于当前计划， [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要计划或更高版本。 对于新计划，此功能可用于所有计划。 有关各种可用计划的详细信息，请参阅 [Workfront计划](https://www.workfront.com/plans).

* [!DNL Microsoft SharePoint]

  有关集成的信息 [!DNL SharePoint]，请参见 [配置 [!DNL SharePoint] 集成](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 第三方云文档提供商：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google通道]

     <!--Quip-->

  >[!TIP]
  >
  >您可以验证和批准从外部云提供商链接的文档，就像验证和批准直接上传到的文档一样 [!DNL Workfront].

* 其他文档提供程序（通过自定义文档集成）。

  对于当前计划， [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要计划或更高版本。 对于新计划，此功能可用于所有计划。 有关各种可用计划的详细信息，请参阅 [Workfront计划](https://www.workfront.com/plans).

此外，您还可以增强 [!DNL Workfront] 使用本机数字资产管理(DAM)系统或使用第三方DAM集成提供文档体验。 管理员必须启用这些功能，用户才能将服务链接到他们的 [!DNL Workfront] 帐户。 有关Workfront DAM的更多信息，请参阅 [使用管理文档 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## 配置集成以管理文档

{{step-1-to-setup}}

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL 云提供商].**

1. （可选）将文档存储在文档服务应用程序中，而不是中 [!DNL Workfront]，选择 **[!UICONTROL 阻止用户在中存储文档 [!DNL Workfront]].**

1. 选择要启用的集成。
1. 单击&#x200B;**[!UICONTROL 保存]**。

如果您要设置与 [!DNL Workfront DAM]，您可以启用 [!DNL Workfront] 将元数据与文档包括在内。 有关映射元数据的信息，请参见 [设置元数据映射](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## 配置自定义文档集成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自定义文档集成允许 [!DNL Workfront] 要将文件链接到的用户 [!DNL Workfront] 几乎任何系统，前提是该系统能够与 [!DNL Workfront].

要使自定义集成可供用户使用，您首先需要构建集成。 有关如何构建要与一起使用的集成的信息 [!DNL Workfront]，请参见 [文档Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

构建自定义文档集成后，您可以将其提供给网站上的用户。

{{step-1-to-setup}}

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL 自定义集成]**.

1. 单击 **[!UICONTROL 添加自定义集成]**.
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
      <td>API调用的基本HTTP或安全HTTP URL。 例如， <code>https://documentprovider.com/api/v2</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL身份验证类型]</td> 
      <td> <p>对自定义集成进行授权的API调用时要使用的身份验证方法。</p> 
       <ul> 
        <li>如果您选择 <strong>[！UICONTROL OAuth]</strong>，继续执行步骤5。</li> 
        <li>如果您选择 <strong>[！UICONTROL ApiKey]</strong>，继续执行步骤6。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果您选择 **[!UICONTROL OAuth]** 的身份验证 **[!UICONTROL 身份验证类型]**，输入以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL身份验证URL]</td> 
      <td>用于用户身份验证的完整URL。 [!DNL Workfront] 在OAuth配置过程中将用户导航到此地址。</td> 
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
      <td> <p>输入要附加到每个API调用的查询字符串的可选值。 例如，access_type=offline。</p> <p>要添加多个请求参数，请单击 <strong>+添加请求参数</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >此 [!DNL Workfront] 显示在底部的重定向URI [!UICONTROL 自定义集成] 页面列出了用于将该集成注册到外部文档提供程序的URI。

1. （视情况而定）如果您选择 **[!UICONTROL ApiKey]** 的身份验证 **[!UICONTROL 身份验证类型]**，输入由自定义文档提供商颁发的API密钥。

   [!DNL Workfront] 使用此API密钥向文档提供商进行授权的API调用。

1. 单击 **[!UICONTROL 保存]** 以创建集成。

## 使用文档集成

有关用户如何使用的信息 [!DNL Workfront DAM]，请参见 [使用管理文档 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

有关用户如何使用验证的信息，请参阅 [创建验证](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs-in-wf.md).

有关用户在配置第三方文档集成后如何使用第三方文档集成的信息，请参阅 [链接来自外部应用程序的文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 配置 [!DNL Workfront] 将元数据发送到 [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

从发送文档时 [!DNL Workfront] 到 [!DNL Workfront DAM]，则还可以发送与该文档关联的信息。 有关文档的信息被映射到 [!DNL Workfront DAM] 作为元数据。

信息仅单向映射，从 [!DNL Workfront] 到 [!DNL Workfront DAM] 并且仅当文档上传到时才会传输 [!DNL Workfront DAM]. Workfront字段中的任何未来更改都不会更新中的元数据字段 [!DNL Workfront DAM] 在上传文档之后。\
您可以映射相同的 [!DNL Workfront] 字段至各种 [!DNL Workfront DAM] 字段，但不能使用相同的字段 [!DNL Workfront DAM] 多个字段 [!DNL Workfront] 字段。

如果必须配置多个 [!DNL Workfront] 要导出到其中的字段 [!DNL Workfront DAM] 字段，首先在中创建计算自定义字段 [!DNL Workfront] 显示对象的所有单个自定义字段。 然后，映射计算的 [!DNL Workfront] 字段到一 [!DNL Workfront DAM] 字段。\
有关计算的自定义字段的更多信息，请参阅 [将计算的数据添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

该映射会影响任何用户从上传的所有文档 [!DNL Workfront] 到 [!UICONTROL Workfront] 达姆。

作为 [!DNL Workfront] 管理员，您必须启用 [!DNL Workfront DAM] 之前，您需要先在Workfront中映射用于元数据映射过程的字段。

配置 [!DNL Workfront] 将元数据发送到 [!DNL Workfront DAM]：

{{step-1-to-setup}}

1. 单击 **[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**.

1. 在 **[!UICONTROL 选择要映射的源字段]** 字段中，开始键入要映射到的Workfront字段的名称 [!DNL Workfront DAM]，然后在列表中看到该复选框时将其选中。
1. 在 **[!UICONTROL 选择要映射的目标字段]**，选择 [!DNL Workfront DAM] 要用所选字段中的信息填充的字段 [!DNL Workfront] 字段。

   >[!NOTE]
   >
   > 所有文档发送至 [!DNL Workfront DAM] 如有权限的用户，其元数据将更新为 [!DNL Workfront] 这些字段上传到时，会在此处映射 [!DNL Workfront DAM].

1. 单击 **[!UICONTROL 添加映射]**.

1. 继续添加更多 [!UICONTROL Workfront] 字段和相应 [!DNL Workfront DAM] 字段。

### 删除映射字段

{{step-1-to-setup}}

1. 展开 **[!UICONTROL 文档]**，然后单击 **[!UICONTROL 元数据映射]**.

1. 在字段列表中，选择要从元数据映射中删除的任何字段。
1. 单击 **[!UICONTROL 删除]**.

   这些字段将从元数据映射中删除，并且其中包含的信息不会传输到 [!DNL Workfront DAM] 以及上传的文档。
