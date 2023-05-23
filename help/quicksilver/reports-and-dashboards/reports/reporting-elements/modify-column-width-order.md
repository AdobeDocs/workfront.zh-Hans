---
product-area: reporting
navigation-topic: reporting-elements
title: 修改欄寬和順序
description: 請參閱本文章，瞭解欄寬指引，以及如何在Workfront中變更欄寬和順序。
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# 修改欄寬和順序

以下是有關欄寬在Adobe Workfront中如何運作的准則：

* Workfront預設會定義清單和報告中的欄寬。
* Workfront會根據 `valueformat`除非在欄的文字模式中另外指定，否則所有清單和報告中的資訊。

   >[!NOTE]
   >
   >Workfront不會根據 `valueformat` 「設定」和「報告」區域中可用清單中的資訊。

   此 `valueformat` value會定義欄中顯示的資訊型別。 例如，顯示數字的欄比顯示「說明」欄位的欄窄。

* 您可以根據要在欄中顯示的資訊型別，自訂Workfront清單和報告中的欄寬，以符合您的需求。

   您可以在檢視清單或報表時暫時修改欄寬，或是透過在檢視產生器中調整欄寬來永久修改。 如需暫時修改欄寬的相關資訊，請參閱 [暫時修改欄寬和順序時的注意事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) 章節。

* 內建檢視中顯示的欄具有先前由Workfront定義並以硬式編碼的寬度。 若要修改這些寬度，您必須使用檢視產生器中的文字模式，手動更新這些欄的寬度。

   如需有關在文字模式中修改欄的資訊，請參閱 [檢視：永久編輯欄寬](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront計畫*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront授權*</strong></td> 
   <td> <p>要求或以上 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的檢視</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權以編輯報表中的檢視</p> <p>管理檢視的許可權以進行編輯</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 修改欄寬和順序

您可以透過下列方式修改報表中的欄寬和順序：

* [暫時修改欄寬和順序](#modify-width-and-order-of-columns-temporarily)
* [永久修改欄寬和順序](#modify-width-and-order-of-columns-permanently)

### 暫時修改欄寬和順序 {#modify-width-and-order-of-columns-temporarily}

您可以拖曳欄框線來調整欄大小，以及拖放欄以暫時在整個Workfront網站的大部分清單中重新排序。 這包括報告、檢視、儀表板的報告和甘特圖。

如需Workfront清單的詳細資訊，請參閱文章 [開始使用Adobe Workfront中的清單](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [暫時修改欄寬和順序時的注意事項](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [暫時調整欄大小](#resize-columns-temporarily)
* [暫時重新排序欄](#reorder-columns-temporarily)

#### 暫時修改欄寬和順序時的注意事項 {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

您可以暫時修改清單中欄的寬度和順序，而無需編輯其檢視。

暫時調整欄大小和排序欄時，請注意下列事項：

* 重新調整欄大小時新欄大小會儲存在瀏覽器的本機儲存空間中，並依預設儲存。 使用不同的瀏覽器、清除快取或瀏覽資料會導致欄大小恢復為預設值。 重新整理頁面會保留您對欄寬所做的變更。
* 重新排序欄時，只會維持您選擇的順序，直到您離開清單或重新整理瀏覽器頁面為止。 離開清單或重新整理瀏覽器頁面後，欄會回到其預設順序。
* 為獲得最佳效能，您重新排序的欄在清單中不應超過100個專案。
* 當您調整欄大小時，您的變更只會套用至您目前使用的檢視，而且只有您能看見。 與其他使用者共用檢視時，不會共用您已定義的欄大小。
* 當您將欄的邊框拖曳到右邊來調整欄大小後，除了下列情況外，相鄰欄的寬度會保留：

   * 設定區域
   * 報告區域
   * 檔案清單和報告

   >[!NOTE]
   >
   >您無法將欄的左邊框移動到任何清單中相鄰欄的左邊框之外。

* 如果您將任何清單匯出至檔案，欄的暫時順序不會轉移到匯出的檔案。 在重新排序欄之前，匯出的檔案會顯示原始清單中的欄順序。

如需從清單和報告匯出資料的詳細資訊，請參閱文章 [匯出資料](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### 暫時調整欄大小 {#resize-columns-temporarily}

1. 前往您要修改的清單。
1. 拖曳欄的框線，直到欄達到所需大小。\
   ![](assets/column-resize-350x124.png)

#### 暫時重新排序欄 {#reorder-columns-temporarily}

1. 前往您要修改的清單。
1. 按一下要移至其他位置的欄，挑選該欄。
1. 將欄拖曳到正確的位置。
1. 將欄拖放到位置以移動它。

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>這在同時檢視甘特圖和清單檢視時特別有用。 檢視甘特圖時，欄可能會變成隱藏。 若要在顯示甘特圖時檢視欄，只要拖曳您要檢視的欄，使其顯示在頁面左側即可。

### 永久修改欄寬和順序 {#modify-width-and-order-of-columns-permanently}

若要永久重新排序欄，請參閱區段 [建立或自訂標準檢視](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) 在文章中 [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

您只能使用文字模式來永久修改欄寬。

如需有關使用文字模式及永久修改欄寬的詳細資訊，請參閱文章 [文字模式的常見用途概觀](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
