---
title: 設定檔案整合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 設定檔案整合
author: Courtney, Caroline
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: cf5c4e3d-b45f-46cd-a938-22e412d1c491
source-git-commit: 456c7b21835c96912e8974063f7797283dcb4e6d
workflow-type: tm+mt
source-wordcount: '1161'
ht-degree: 1%

---

# 設定檔案整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

作為 [!DNL Adobe Workfront] 管理員，您可以設定檔案整合以管理檔案 [!UICONTROL Workfront]. 您也可以設定 [!UICONTROL Workfront] 因此檔案只會儲存在document services應用程式中，而不會儲存在 [!UICONTROL Workfront] 本身。 如需詳細資訊，請參閱 [更新並連結檔案，從 [!UICONTROL Workfront] 至外部雲端提供者](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) 在 [從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

>[!NOTE]
>
>若要允許開啟以下專案之間的通訊： [!DNL Workfront Proof] 和 [!DNL Workfront] 伺服器，您可能需要將特定IP位址新增至允許清單。 如需詳細資訊，請參閱 [設定防火牆的允許清單](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 存取需求

您必須具備下列專案才能執行本文所述的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 授權</td> 
   <td>[！UICONTROL計畫]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>您必須是 [!DNL Workfront] 管理員。 有關以下專案的資訊： [!DNL Workfront] 管理員，請參閱 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予使用者完全管理存取權</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有哪些計畫、授權型別或存取權，請聯絡您的 [!DNL Workfront] 管理員。

## 支援的整合

<!--DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以設定下列整合來管理檔案：

<!--
  Experience Manager Assets Essentials </p>
  -->

* [!DNL Workfront DAM]

* [!DNL Workfront Proof]

   連結校樣從 [!DNL Workfront Proof] 可讓您製作原本在中建立的校樣 [!DNL Workfront Proof] 提供於 [!DNL Workfront]. A [!UICONTROL Pro] [!DNL Workfront] 需要計畫或更高版本才能使用此功能。 如需各種可用計畫的詳細資訊，請參閱 [Workfront計畫。](https://www.workfront.com/plans)

* [!DNL Microsoft SharePoint]

   如需整合的相關資訊，請參閱 [!DNL SharePoint]，請參閱 [設定 [!DNL SharePoint] 整合](../../administration-and-setup/configure-integrations/configure-sharepoint-integration.md).

* 第三方雲端檔案提供者：

   * [!DNL Box]
   * [!DNL Dropbox]
   * [!DNL Dropbox Business]
   * [!DNL WebDAM]
   * [!DNL Microsoft OneDrive]
   * [!DNL Microsoft SharePoint]
   * [!UICONTROL Google Drive]

      <!--Quip-->
   >[!TIP]
   >
   >您可以校訂和核准從外部雲端提供者連結的檔案，就像校訂和核准直接上傳到的檔案一樣 [!DNL Workfront].

* 其他檔案提供者（透過自訂檔案整合）。

   A [!UICONTROL Pro] [!DNL Workfront] 需要計畫或更高版本才能使用此功能。 如需各種可用計畫的詳細資訊，請參閱 [[!DNL Workfront] 計畫。](https://www.workfront.com/plans)

此外，您也可以增強 [!DNL Workfront] 原生數位資產管理(DAM)系統或協力廠商DAM整合的檔案體驗。 管理員必須啟用這些功能，使用者才能將服務連結至其 [!DNL Workfront] 帳戶。 如需Workfront DAM的詳細資訊，請參閱 [管理檔案，使用 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

## 設定整合以管理檔案

1. 登入 [!DNL Workfront] 以管理員身分。
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 雲端服務供應商].**

1. （選擇性）將檔案儲存在檔案服務應用程式中，但不儲存在 [!DNL Workfront]，選取 **[!UICONTROL 防止使用者將檔案儲存在 [!DNL Workfront]].**

1. 選取您要啟用的整合。
1. 单击&#x200B;**[!UICONTROL 保存]**。

如果您要設定與整合 [!DNL Workfront DAM]，您可以啟用 [!DNL Workfront] 以包含中繼資料與檔案。 如需對應中繼資料的相關資訊，請參閱 [設定中繼資料對應](../../administration-and-setup/configure-integrations/set-up-metadata-mapping.md).

## 設定自訂檔案整合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **)</p>
-->

自訂檔案整合允許 [!DNL Workfront] 要將檔案連結到的使用者 [!DNL Workfront] 幾乎任何系統，前提是系統能夠搭配使用 [!DNL Workfront].

若要讓使用者可以使用自訂整合，您首先需要建置整合。 如需如何建置要與搭配使用的整合的相關資訊 [!DNL Workfront]，請參閱 [檔案Webhooks API](../../wf-api/doc-wbhks-api/docu-webhook-api.md).

建立自訂檔案整合後，您可將它提供給您網站上的使用者。

1. 登入 [!DNL Workfront] 以管理員身分。
1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 在左側面板中，按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 自訂整合].**

1. 按一下 **[!UICONTROL 新增自訂整合]**.
1. 指定下列資訊以設定整合：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL名稱]</td> 
      <td>自訂整合的名稱。 這是使用者在Workfront中使用整合時看到的名稱。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL基本API URL] </td> 
      <td>API呼叫的基本HTTP或安全HTTP URL。 例如， <a class="link-https" title="https://documentprovider.com/api/v2" href="https://documentprovider.com/api/v2">https://documentprovider.com/api/v2</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL驗證型別]</td> 
      <td> <p>對自訂整合進行授權API呼叫時使用的驗證方法。</p> 
       <ul> 
        <li>如果您選擇 <strong>[！UICONTROL OAuth]</strong>，繼續步驟6。</li> 
        <li>如果您選擇 <strong>[！UICONTROL ApiKey]</strong>，請繼續步驟7。</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. （視條件而定）如果您已選取 **[!UICONTROL OAuth]** 驗證 **[!UICONTROL 驗證型別]**，請指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL驗證URL]</td> 
      <td>用於使用者驗證的完整URL。 [!DNL Workfront] 在OAuth布建程式中將使用者導覽至此位址。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL權杖端點URL]</td> 
      <td>用于检索 OAuth 令牌的完整 API URL。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端ID]</td> 
      <td>此整合的OAut使用者端ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL使用者端密碼]</td> 
      <td>此整合的OAut使用者端密碼。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL要求引數]</td> 
      <td> <p>指定要附加至每個API呼叫之查詢字串的選用值。 例如，access_type=offline。</p> <p>若要新增多個請求引數，請按一下 <strong>+新增請求引數</strong>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >此 [!DNL Workfront] 顯示在底部的重新導向URI [!UICONTROL 自訂整合] 頁面會列出用來向外部檔案提供者註冊此整合的URI。

1. （視條件而定）如果您已選取 **[!UICONTROL ApiKey]** 驗證 **[!UICONTROL 驗證型別]**，指定自訂檔案提供者所發出的API金鑰。

   [!DNL Workfront] 使用此API金鑰對檔案提供者進行授權的API呼叫。

1. 按一下 **[!UICONTROL 儲存]** 以建立整合。

## 使用檔案整合

如需使用者如何使用的詳細資訊 [!DNL Workfront DAM]，請參閱 [管理檔案，使用 [!DNL Adobe Workfront DAM]](../../documents/workfront-dam-within-workfront/manage-docs-with-wf-dam.md).

如需使用者如何使用校訂的詳細資訊，請參閱 [建立校樣](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md).

如需有關在您設定協力廠商檔案整合後使用者如何使用協力廠商檔案整合的資訊，請參閱 [從外部應用程式連結檔案](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 設定 [!DNL Workfront] 將中繼資料傳送至 [!UICONTROL [!DNL Workfront] DAM] {#configure-workfront-to-send-metadata-to-workfront-dam}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ***DON'T DELETE, DRAFT OR HIDE THIS SECTION IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **) </p>
-->

從傳送檔案時 [!DNL Workfront] 至 [!DNL Workfront DAM]，您也可以傳送與該檔案相關聯的資訊。 檔案的相關資訊已對應至 [!DNL Workfront DAM] 作為中繼資料。

資訊只會單向對應，從 [!DNL Workfront] 至 [!DNL Workfront DAM] 而且僅當檔案上傳到時才會傳輸 [!DNL Workfront DAM]. Workfront欄位中的任何未來變更都不會更新以下專案的中繼資料欄位： [!DNL Workfront DAM] 檔案上傳後。\
您可以對應相同的 [!DNL Workfront] 欄位至各種 [!DNL Workfront DAM] 欄位，但您不能使用相同的 [!DNL Workfront DAM] 多個欄位 [!DNL Workfront] 欄位。

如果您必須設定多個 [!DNL Workfront] 要匯出至一個的欄位 [!DNL Workfront DAM] 欄位，請先在中建立計算自訂欄位 [!DNL Workfront] 以顯示物件的所有個別自訂欄位。 然後，對應計算的 [!DNL Workfront] 欄位至一 [!DNL Workfront DAM] 欄位。\
如需有關已計算自訂欄位的詳細資訊，請參閱 [將計算資料新增至自訂表單](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

對應會影響任何使用者從上傳的所有檔案 [!DNL Workfront] 至 [!UICONTROL Workfront] DAM。

As a [!DNL Workfront] 管理員，您必須啟用 [!DNL Workfront DAM] 前往Workfront中對應中繼資料對應程式的欄位。 如需如何啟用的詳細資訊 [!DNL Workfront DAM]，請參閱 [設定Workfront將中繼資料傳送至 [!DNL Workfront DAM]](#configure-workfront-to-send-metadata-to-workfront-dam).

進行設定 [!DNL Workfront] 將中繼資料傳送至 [!DNL Workfront DAM]：

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 按一下 **[!UICONTROL 檔案]** > **[!UICONTROL 中繼資料對應]**.

1. 在 **[!UICONTROL 選取要對應的來源欄位]** 欄位，開始輸入您要對應到的Workfront欄位名稱 [!DNL Workfront DAM]，然後在清單中看到該區段時加以選取。
1. 在 **[!UICONTROL 選擇要對應的目標欄位]**，選取 [!DNL Workfront DAM] 要填入所選欄位中資訊的欄位 [!DNL Workfront] 欄位。

   >[!NOTE]
   >
   > 所有傳送至的檔案 [!DNL Workfront DAM] 如有許可權的使用者，其中繼資料會更新為 [!DNL Workfront] 當欄位上傳至時，會在此處對應欄位 [!DNL Workfront DAM].

1. 按一下 **[!UICONTROL 新增對應]**.

1. 繼續新增更多 [!UICONTROL Workfront] 欄位和對應的 [!DNL Workfront DAM] 欄位。

### 刪除對應的欄位

1. 按一下 **[!UICONTROL 主要功能表]** 圖示 ![](assets/main-menu-icon.png) 右上角的 [!DNL Adobe Workfront]，然後按一下 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 展開 **[!UICONTROL 檔案]**，然後按一下 **[!UICONTROL 中繼資料對應]**.

1. 在欄位清單中，選取您要從中繼資料對應中移除的任何欄位。
1. 按一下 **[!UICONTROL 刪除]**.

   欄位會從中繼資料對應中移除，且其中包含的資訊不會傳輸至 [!DNL Workfront DAM] 以及上傳的檔案。
