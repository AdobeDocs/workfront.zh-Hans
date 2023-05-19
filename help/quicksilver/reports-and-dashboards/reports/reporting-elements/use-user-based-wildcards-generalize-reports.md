---
product-area: reporting
navigation-topic: reporting-elements
title: 使用以使用者為基礎的萬用字元來概括報告
description: 建立特定報表元素時，您可以使用萬用字元而非特定資訊來概括報表。
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# 使用以使用者為基礎的萬用字元來概括報告

建立特定報表元素時，您可以使用萬用字元而非特定資訊來概括報表。 例如，如果您想建立一個顯示指派給特定使用者的任務的報告，您可以在篩選器的指派給欄位中使用使用者的名稱。 不過，如果您想要建立顯示指派給登入使用者之任務的報告，而不論該使用者是誰，您可以使用萬用字元來表示當有人檢視報告時，它只會顯示與他們相關的資訊。 這樣的話，報表只需建立一次，但由於您在篩選器中使用萬用字元，因此每當其他人讀取報表時，都會產生不同的結果。

建置下列報表元素時，您可以使用使用者型萬用字元：

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

您必須先建立報表，才能在其中新增萬用字元變數。

如需建立報告的指示，請參閱 [建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 操作步驟

若要在報表中插入以使用者為基礎的萬用字元：

1. 前往您要插入使用者型萬用字元的報表。
1. 按一下 **報表動作**，則 **編輯**.

1. 按一下 **篩選器** 標籤。
1. 按一下 **新增篩選規則**.
1. 開始輸入您要作為篩選依據的欄位名稱。\
   您必須輸入參考使用者物件或使用者相關資訊的欄位。
1. 選取 **等於** ，此專案位於篩選器變數的下拉式功能表中。

   >[!TIP]
   >
   >您必須一律選取 **等於** 在Adobe Workfront中使用萬用字元時篩選變數。

1. 在 **開始輸入名稱……** 方塊，輸入： `$$USER.ID` 或 `$$USER.name` 如果您希望報表根據登入使用者的名稱顯示有關該使用者的資訊。 您可以插入參照登入使用者群組、團隊、公司或其他資訊的其他萬用字元。

   如需使用者型萬用字元的完整清單，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. 按一下 **儲存+關閉**.

## 其他信息

另請參閱：

<!--outdated: * [Basic Report Creation Program](https://one.workfront.com/s/basic-report-creation-program) -->
* [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [在Adobe Workfront中建立或編輯篩選器](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [在檢視中使用條件式格式](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
