---
product-area: reporting
navigation-topic: reporting-elements
title: 使用以日期為基礎的萬用字元來概括報表
description: 建立特定報表元素時，您可以使用萬用字元而非特定資訊來概括報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 759b0bea-729e-4206-808c-0a7216ded4ff
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# 使用以日期為基礎的萬用字元來概括報表

建立特定報表元素時，您可以使用萬用字元而非特定資訊來概括報表。

例如，如果要建立顯示具有特定計劃開始日期之任務的報表，您可以使用篩選器中的行事曆日期選擇器來選取特定日期。 不過，如果您想要建立一份報告，顯示自存取報告日期起特定時間範圍內具有規劃開始日期的任務，您可以使用萬用字元來指示當有人檢視報告時，它顯示與檢視報告之時相關的時間範圍資訊。

例如，在上一週、去年、未來兩週等。 這樣的話，報表只需建置一次，但由於您在篩選中使用萬用字元，每次有人讀取報表時，就會產生不同的結果，因為這會隨著執行報表的日期而改變。

建置下列報表元素時，您可以使用日期型萬用字元：

* 过滤器
* 自訂提示
* 為欄新增規則時的檢視

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>存取層級設定*</strong></td> 
   <td> <p>編輯篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以編輯報告中的報告元素</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以編輯報表中的報表元素</p> <p>管理檢視或篩選的許可權以進行編輯</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立報表，才能新增萬用字元變數。

如需建立報告的詳細資訊，請參閱 [建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步驟

若要在報表中插入以日期為基礎的萬用字元：

1. 前往您要插入日期型萬用字元的報表。
1. 按一下 **報表動作**，則 **編輯**.

1. 按一下 **篩選器** 標籤。
1. 按一下 **新增篩選規則**.
1. 開始輸入您要作為篩選依據的欄位名稱。\
   您必須輸入參考日期的欄位。
1. 選取 **等於** ，此專案位於篩選器變數的下拉式功能表中。

   >[!TIP]
   >
   >您必須一律選取 **等於** 在Adobe Workfront中使用萬用字元時篩選變數。

1. 在 **開始輸入名稱……** 方塊，輸入： `$$TODAY` 如果您想要顯示報表執行當天發生的事件相關資訊。

   或

   型別 `$$NOW` 如果您想要顯示與報表執行日期及時間同時發生的事件相關資訊。

   此日期一律不同，因為它會隨著使用者實際檢視報表的日期而變更。 因此，報表中的資訊每天都不同。

1. （選用）如果要顯示報表執行日期後某個時間範圍內發生的資訊，請輸入 `$$TODAY+1w` 來顯示下一週的資訊，或 `$$TODAY+2m` 以便在接下來的兩個月內顯示資訊。 您也可以指出季度、小時、天或年的時間範圍。
1. （選用）如果您想要顯示報表執行日期之前某個時間範圍內所發生事件的相關資訊，請輸入 `$$TODAY-1w` 顯示前一週的資訊，或 `$$TODAY-2m` 以顯示前兩個月的資訊。 您也可以指出季度、小時、天或年的時間範圍。

   如需您可以在日期型萬用字元中使用的屬性、限定詞和運運算元的完整清單，請參閱文章 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/video-date-based-wildcard-in-task-filter-350x81.png)

1. 按一下 **儲存+關閉**.

## 其他信息

另請參閱：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
