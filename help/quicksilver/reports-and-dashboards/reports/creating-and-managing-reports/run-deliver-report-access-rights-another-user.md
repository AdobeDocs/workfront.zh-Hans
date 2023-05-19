---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 使用其他使用者的存取許可權執行並傳遞報告
description: 依預設，使用者只能看見他們有權檢視的報表中的物件。
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: e68e470da3b03e418584898c4098f0be302c68ec
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 0%

---

# 使用其他使用者的存取許可權執行並傳遞報告

依預設，使用者只能看見他們有權檢視的報表中的物件。

您可以允許所有使用者以其他使用者的身分在報告中檢視相同的結果，無論其對報告內物件的存取層級或許可權層級為何。

如果您使用其他擁有較高存取許可權的使用者的存取許可權(例如，Adobe Workfront管理員的存取許可權)來執行報表，則所有擁有檢視報表許可權的使用者，都可以以Report Builder中指定的使用者的身分，檢視報表中的資訊。 您可以為使用者在Workfront介面中找到的兩個報表，或是以電子郵件附件的形式傳送給使用者的報表，設定此專案。

>[!TIP]
>
>您應取代 **使用此報告的存取許可權為：** 欄位中的有效使用者，前提是您希望報表能顯示該使用者的存取許可權。 例如，工作授權使用者可能沒有許可權檢視計畫授權使用者或系統管理員建立的報告中的所有專案，除非該報告顯示時具有供需規劃員或系統管理員的存取許可權。\
如果與具有類似存取許可權的使用者共用報告，則該使用者可在 **使用此報告的存取許可權為：** 欄位，您可以將此欄位留空。

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront計畫*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront授權*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯對報告、儀表板、行事曆的存取權</p> <p>編輯篩選器、檢視、群組的存取權</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>檢視報表的許可權（檢視傳遞的報表）</p> <p>管理報告的許可權（執行報告）</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 顯示具有其他使用者存取許可權的報告

填入 **使用此報告的存取許可權為：** 欄位可確保報表包含相同的資料，無論哪個使用者正在存取該報表。 報表會依指定使用者的顯示方式顯示。

存取報告的使用者必須至少具有報告的檢視許可權，才能看到報告。 如果使用者列在 **使用此報告的存取許可權為：** 欄位已停用，該報表不再顯示給共用該報表的任何其他使用者。

若要使用其他使用者的存取許可權執行報告：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **報表**.

1. 選取您要以其他使用者的存取許可權顯示的報表。
1. 按一下 **報表動作**，然後按一下 **編輯**.

1. 按一下 **報表設定**.

1. 在 **使用此報告的存取許可權為：** 欄位，開始輸入您希望報表顯示成的使用者名稱，然後在清單中看到時選取它。\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   存取層級較低、可建置報表的使用者，除了他們自己之外，無法為 **使用此報告的存取許可權為：** 欄位。

1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.\
   現在，與其共用報表的所有使用者皆可看見該報表，就像該報表已由中指定的使用者檢視一樣。 **使用此報告的存取許可權為：** 欄位。

>[!IMPORTANT]
輸入非登入使用者的使用者 **使用此報告的存取許可權為：** 如果報表包含使用萬用字元指出登入使用者的篩選器，欄位會影響報表中顯示的資訊。 報表會依據中指定的值顯示 **使用此報告的存取許可權為：** 欄位，而不是萬用字元篩選器中定義的內容。
如需使用者欄位萬用字元的詳細資訊，請參閱以下的「使用者型變數」一節： [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 傳遞具有其他使用者存取許可權的報告

您可以設定要作為電子郵件附件傳送的報表。 您可以設定這些傳遞的報表在針對較高存取層級的使用者顯示時顯示，讓所有使用者都可以在傳遞的報表中看到相同的資訊。 將會看到以電子郵件傳送之報告的使用者，必須新增至報告傳送內的「傳送至」收件者清單。 如需設定傳送報告的詳細資訊，請參閱文章 [報告傳遞概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

若要傳送具有其他使用者存取許可權的報告：

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **報表**.

1. 選取您要傳送且有其他使用者存取許可權的報告。
1. 按一下報表名稱以選取它。
1. 按一下 **報表動作**.
1. 按一下 **傳送報告**.

1. 在 **提供此報告的存取許可權為：** 欄位，開始輸入您希望報表在電子郵件中傳送時顯示的使用者名稱，然後在清單中看到報表時選取該名稱。 預設值為建立報表的使用者名稱。\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   存取層級較低、可建置報表的使用者，除了他們自己之外，無法為 **提供此報告並具備以下存取許可權：** 欄位。

1. 選取 **格式** 您想要報表顯示在電子郵件中：

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. 按一下 **立即傳送** 立即傳送。\
   或\
   按一下 **建立重複傳遞** 排程報表的循環傳送。\
   如需報告傳送的詳細資訊，請參閱文章 [報告傳遞概觀](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 具有來源欄的報表限制

下列報表會顯示「來源」欄，您可以在其中檢視父物件的相關資訊：

* 問題報告
* 小時報告
* 檔案報告

如果使用者無權存取問題、小時或檔案的父物件，則報告的「來源」欄會顯示空白，即使報告已設定為顯示，或要使用其他使用者的存取許可權傳送。

為了在報告中顯示有關父物件的資訊，我們建議為父物件新增一欄，您可以在其中顯示父物件的名稱。

例如，您可以新增下列任何專案至具有來源欄的報表：

* 檔案或時數報告的「專案名稱」、「任務名稱」或「問題名稱」欄。
* 問題報告的「專案名稱」或「任務名稱」欄。
* 使用參照所有三個物件的文字模式運算式的欄。 以下是時數報告的範例：

   `displayname=Custom Source`

   `linkedname=opTask`

   `namekey=view.relatedcolumn`

   `namekeyargkey.0=opTask`

   `namekeyargkey.1=name`

   `textmode=true`

   `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

   `valueformat=HTML`

   如需文字模式檢視的相關資訊，請參閱 [使用文字模式編輯檢視](../text-mode/edit-text-mode-in-view.md).