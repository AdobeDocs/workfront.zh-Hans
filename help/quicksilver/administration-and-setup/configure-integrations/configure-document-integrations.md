---
title: 配置文档集成
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 配置文档集成
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: ceda437684f565b91dbb8b02f6b03cbe8d27a70a
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# 配置文档集成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作为 [!DNL Adobe Workfront] 管理员，您可以配置文档集成以在 [!UICONTROL Workfront]. 您还可以配置 [!UICONTROL Workfront] 以便文档仅存储在文档服务应用程序中，而不存储在 [!UICONTROL Workfront] 自己。 有关更多信息，请参阅 [更新并链接来自 [!UICONTROL Workfront] 到外部云提供程序](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) in [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>允许在 [!DNL Workfront Proof] 和 [!DNL Workfront] 服务器，则可能需要向添加某些IP地允许列表址。 有关更多信息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 受支持的集成

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以配置以下集成以管理文档：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   从链接校样 [!DNL Workfront Proof] 用于制作最初在 [!DNL Workfront Proof] 可在 [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要计划或更高版本。 有关各种可用计划的更多信息，请参阅 [Workfront计划。](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   有关与集成的信息 [!DNL SharePoint]，请参阅 [配置 [!DNL SharePoint] 集成](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 第三方云文档提供程序：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >您可以采用与校样和批准已直接上传到的文档相同的方式，对从外部云提供商链接的文档进行校样和批准 [!DNL Workfront].

* 其他文档提供程序（通过自定义文档集成）。

   A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要计划或更高版本。 有关各种可用计划的更多信息，请参阅 [[!DNL Workfront] 计划。](https://www.workfront.com/plans)

此外，您还可以 [!DNL Workfront] 使用本机数字资产管理(DAM)系统或第三方DAM集成记录体验。 管理员必须启用这些功能，才能将用户的服务链接到其 [!DNL Workfront] 帐户。 有关Workfront DAM的更多信息，请参阅 [使用管理文档 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## 配置集成以管理文档

1. 登录到 [!DNL Workfront] 作为管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL 云提供商].**

1. （可选）将文档存储在文档服务应用程序中，而不是 [!DNL Workfront]，选择 **[!UICONTROL 阻止用户在 [!DNL Workfront]].**

1. 选择要启用的集成。
1. 单击&#x200B;**[!UICONTROL 保存]**。

如果您要设置与的集成 [!DNL Workfront DAM]，则您可以 [!DNL Workfront] 将元数据包含在文档中。 有关映射元数据的信息，请参阅 [设置元数据映射](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## 配置自定义文档集成

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自定义文档集成允许 [!DNL Workfront] 将文件链接到 [!DNL Workfront] 从几乎任何系统，只要系统是与 [!DNL Workfront].

要使自定义集成可供用户使用，您首先需要构建集成。 有关如何构建要与 [!DNL Workfront]，请参阅 [文档Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

构建自定义文档集成后，您可以将其提供给网站上的用户。

1. 登录到 [!DNL Workfront] 作为管理员。
1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **[!UICONTROL 文档]** > **[!UICONTROL 自定义集成].**

1. 单击 **[!UICONTROL 添加自定义集成]**.
1. 指定以下信息以配置集成：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名称]</td> 
      <td>自定义集成的名称。 这是用户在Workfront中使用集成时看到的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Base API URL] </td> 
      <td>用于API调用的基本HTTP或安全HTTP URL。 例如， <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL身份验证类型]</td> 
      <td> <p>对自定义集成进行授权API调用时要使用的身份验证方法。</p> 
       <ul> 
        <li>如果您选择 <strong>[!UICONTROL OAuth]</strong>，继续步骤6。</li> 
        <li>如果您选择 <strong>[!UICONTROL ApiKey]</strong>，继续步骤7。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）如果您选择 **[!UICONTROL OAuth]** 身份验证 **[!UICONTROL 身份验证类型]**，请指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL身份验证URL]</td> 
      <td>用于用户身份验证的完整URL。 [!DNL Workfront] 在OAuth配置过程中，将用户导航到此地址。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL令牌端点URL]</td> 
      <td>用于检索 OAuth 令牌的完整 API URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客户端ID]</td> 
      <td>此集成的OAut客户端ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL客户端密钥]</td> 
      <td>此集成的OAut客户端密钥。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL请求参数]</td> 
      <td> <p>指定要附加到每个API调用查询字符串的可选值。 例如， access_type=offline。</p> <p>要添加多个请求参数，请单击 <strong>+添加请求参数</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >的 [!DNL Workfront] 重定向URI，显示在 [!UICONTROL 自定义集成] 页面列出了用于注册此集成与外部文档提供程序的URI。

1. （视情况而定）如果您选择 **[!UICONTROL ApiKey]** 身份验证 **[!UICONTROL 身份验证类型]**，指定由自定义文档提供程序颁发的API密钥。

   [!DNL Workfront] 使用此API密钥对文档提供程序进行授权API调用。

1. 单击 **[!UICONTROL 保存]** 创建集成。

## 使用文档集成

有关用户如何使用的信息 [!DNL Workfront DAM]，请参阅 [使用管理文档 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

有关用户如何使用校样的信息，请参阅 [创建校样](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

有关用户在配置后如何使用第三方文档集成的信息，请参阅 [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 配置 [!DNL Workfront] 将元数据发送到 [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

从发送文档时 [!DNL Workfront] to [!DNL Workfront DAM]，则还可以发送与该文档关联的信息。 有关文档的信息已映射到 [!DNL Workfront DAM] 作为元数据。

信息仅通过单向映射(从 [!DNL Workfront] to [!DNL Workfront DAM] 并且只有在将文档上传到时，才会将其转移 [!DNL Workfront DAM]. Workfront字段中的任何未来更改都不会更新 [!DNL Workfront DAM] 在文档已上传之后。\
您可以映射相同的 [!DNL Workfront] 字段 [!DNL Workfront DAM] 字段，但不能使用相同的 [!DNL Workfront DAM] 字段 [!DNL Workfront] 字段。

如果必须配置多个 [!DNL Workfront] 导出到一个字段 [!DNL Workfront DAM] 字段，首先在 [!DNL Workfront] 以显示对象的所有单个自定义字段。 然后，映射计算出的 [!DNL Workfront] 字段至1 [!DNL Workfront DAM] 字段。\
有关计算自定义字段的更多信息，请参阅 [将计算数据添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

映射会影响任何用户从 [!DNL Workfront] to [!UICONTROL Workfront] DAM。

As a [!DNL Workfront] 管理员，必须启用 [!DNL Workfront DAM] 在Workfront中，才能映射元数据映射流程的字段。 有关如何启用的更多信息 [!DNL Workfront DAM]，请参阅 [配置Workfront以将元数据发送到 [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

配置 [!DNL Workfront] 将元数据发送到 [!DNL Workfront DAM]:

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 文档]** > **[!UICONTROL 元数据映射]**.

1. 在 **[!UICONTROL 为映射选择源字段]** 字段中，开始键入要映射到的Workfront字段的名称 [!DNL Workfront DAM]，然后在列表中看到时将其选中。
1. 在 **[!UICONTROL 选择要映射的目标字段]**，选择 [!DNL Workfront DAM] 要填充的字段中的 [!DNL Workfront] 字段。

   >[!NOTE]
   >
   > 所有发送到的文档 [!DNL Workfront DAM] 有权执行此操作的用户的元数据将更新为 [!DNL Workfront] 映射到此处的字段，当它们上传到 [!DNL Workfront DAM].

1. 单击 **[!UICONTROL 添加映射]**.

1. 继续添加更多 [!UICONTROL Workfront] 字段和对应的 [!DNL Workfront DAM] 字段。

### 删除映射的字段

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 展开 **[!UICONTROL 文档]**，然后单击 **[!UICONTROL 元数据映射]**.

1. 在字段列表中，选择要从元数据映射中删除的任意字段。
1. 单击 **[!UICONTROL 删除]**.

   这些字段将从元数据映射中删除，并且其中包含的信息不会传输到 [!DNL Workfront DAM] 上传的文档。
