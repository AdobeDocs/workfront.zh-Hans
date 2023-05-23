---
content-type: reference
product-area: reporting;projects
keywords: 計算，彙總，進階，檢視
navigation-topic: custom-view-filter-and-grouping-samples
title: 「分組：顯示分組中多個計算值的彙總結果」
description: 您可以使用欄中的文字模式，在報表或清單檢視中的兩個欄位之間顯示計算。 每一行會顯示報告或清單中每個物件的計算。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e67c0b10-af9f-4657-8f99-8b63ae3c0865
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 0%

---

# 分組：顯示分組中彙總多個計算值的結果

您可以使用欄中的文字模式，在報表或清單檢視中的兩個欄位之間顯示計算。 每一行會顯示報告或清單中每個物件的計算。

例如，您可以在任務報告中針對每個任務，在名為「工作平衡」的第三欄中顯示實際時數與計畫時數之間的差異。 如需有關計算資料運算式的詳細資訊，請參閱 [計算資料運算式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

您可以將計算新增至群組的相同欄，以顯示多個已計算檢視專案的彙總值。 `aggregator` 包含計算值的欄行。 例如，您可以彙總（顯示總和）報告分組或「工作餘額」欄位清單中所有任務的「工作餘額」時數金額。 本文會說明如何執行此操作。

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
   <td> <p>請求修改群組 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改群組</p> <p><b>注释</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 顯示群組內彙總多個計算值的結果

1. 前往任務報告，按一下 **報表動作** > **編輯**.
1. 在 **群組** 標籤，按一下 **新增群組**，並開始輸入 **專案名稱** 在 **將報表分組** > **第一人** 欄位，然後在清單中顯示時選取它。

1. 在 **欄（檢視）** 標籤，按一下 **新增欄**，然後開始輸入 **計畫時數** 在 **顯示在此欄中** 欄位，然後在清單中顯示時選取它。

   >[!TIP]
   >
   >在文字模式中編輯資訊之前，請一律開始使用「標準」介面新增資訊。 新增最接近或包含最多資訊的欄位，以用於您嘗試進行的計算。

1. 在 **此欄的摘要方式** 欄位，選取 **總和**，然後按一下 **完成**.
1. 按一下 **切換至文字模式** 在您新增的欄中。
1. 暫留在文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 取代 `valuefield ` 和 `aggregator.valuefield` 在下列文字模式範例中反白的行：

   ```
   valueformat=compound
   aggregator.displayformat=minutesAsHoursString
   aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2)
   aggregator.function=SUM
   aggregator.valueformat=val
   aggregator.namekey=workrequired
   linkedname=direct
   textmode=true
   valuefield=workRequired
   namekey=workrequired
   valueexpression=CONCAT(ROUND(({workRequired}-{actualWorkRequired})/60,2)," Hours") 
   viewalias=workrequired 
   displayname=Work Balance
   ```

   >[!TIP]
   >
   >若要在群組內取得彙總值，以顯示計畫時數與實際時數欄位之間的彙總差異，請將相同的方程式輸入到 `aggregator.valuefield` 行。 此 `aggregator.displayformat` 用於「計畫時數」欄會將分鐘數轉換為時數。 由於計畫時數欄位已用作預留位置，因此不需要調整此行。
   >
   >
   >此 `minutesAsHoursString` 的定義 `aggregator.displayformat` 行表示不需要將每個欄位除以60，如同在 `valueexpression` 以取得結果。 在此 `aggregator.valuefield=workRequired` 會變成： `aggregator.valueexpression=ROUND(({workRequired}-{actualWorkRequired}),2`.

1. 按一下 **儲存+關閉**.
