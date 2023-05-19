---
product-area: reporting
navigation-topic: text-mode-reporting
title: 文字模式語法概觀
description: 您可以使用文字模式介面在清單和報告中建立更複雜的檢視、篩選器、分組和自訂提示。 透過使用文字模式，您可以存取在標準模式介面中無法使用的欄位及其屬性。
author: Nolan
feature: Reports and Dashboards
exl-id: f24430e1-c5f7-4925-93df-0e956a03c863
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '1478'
ht-degree: 0%

---

# 文字模式語法概觀

您可以使用文字模式介面在清單和報告中建立更複雜的檢視、篩選器、分組和自訂提示。 透過使用文字模式，您可以存取在標準模式介面中無法使用的欄位及其屬性。

有關開始前文字模式的資訊和考量事項，請參閱 [文字模式概觀](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

如需所有可報告欄位及其屬性的完整清單，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

## 有關文字模式語法的考量事項

* 您必須先瞭解Adobe Workfront語法，才能開始以文字模式建立報表元素。 文字模式的Workfront語法是此應用程式所獨有的，並具有您必須熟悉的獨特特性。
* 在報表中開始使用文字模式之前，強烈建議您先參加進階報表的課程，以更深入地瞭解我們的文字模式語言。 <!--outdated link: For training materials on reporting see [Workfront Reports and Dashboards Learning Paths](https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ).-->
* 您可以使用標準模式介面自訂檢視、篩選器和群組。 不過，您只能使用文字模式來建立「自訂提示」。

## 以文字模式建立報表元素的通用准則

以文字模式建立任何報告或清單元素時，以下是常見准則：

* 參考Workfront資料庫中的物件或屬性時，請一律使用駝峰式大小寫。
* 請記住Workfront中的物件階層。 檢視、篩選器和群組之間有下列差異：

   * 您可以在檢視中顯示一個物件，該物件與報表或清單物件相距三個物件。
   * 您不能在群組、篩選或自訂提示中參照遠離主要物件2個以上的物件。

   **範例：** 您可以在任務檢視中顯示Portfolio擁有者的名稱或GUID：

   ```
   valuefield=project:portfolio:ownerID
   ```

   您不能在任務檢視中群組、篩選或提示Portfolio擁有者：

   ```
   project:portfolio:ownerID=5808f4bc00790b270a9629dd128e63fa
   ```

   在這些範例中，Portfolio擁有者ID是清單物件之外的三個物件。

   如需Workfront中物件階層的相關資訊，請參閱：

   * [瞭解Adobe Workfront中的物件](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
   * [API總管](../../../wf-api/general/api-explorer.md)


* 儘可能使用萬用字元，讓您的報告和清單更動態，並避免針對不同使用者和類似時間表重複這些報告。

## 駝峰式大小寫概觀

在文字模式中參照Workfront欄位或其屬性時，Workfront會要求您以駝峰式大小寫輸入其名稱。 在此情況下，單一名稱欄位的拼字會變成小寫。 複合欄位的拼字方式如下：

```
camelCaseSyntax
```

>[!IMPORTANT]
>
>所有報告元素都遵循此大小寫模式。

駝峰式大小寫的特點是：

* 第一個字詞一律以小寫字母開頭。
* 下列字詞一律以大寫字母開頭。
* 字詞之間沒有空格。

**範例：** 若要參考專案的實際完成日期，您在建立文字模式報表元素時可使用的欄位名稱是

```
actualCompletionDate
```

。

## 各種報表元素的文字模式語法

使用文字模式建立下列報表元素集合時，其語法之間有下列相似性：

* 檢視和分組的程式碼行和語法類似。

   如需以文字模式建立檢視和分組時，檢視和分組的程式碼關鍵行的相關資訊，請參閱：

   * [使用文字模式編輯檢視](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)
   * [編輯群組中的文字模式](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md)

* 篩選和自訂提示的程式碼和語法行類似。

   如需詳細資訊，請參閱：

   * [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)
   * [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

### 檢視和群組的語法

您可能會注意到建立檢視和分組時的程式碼行類似。

如需建立檢視和群組的相關資訊，請參閱下列文章：

* [Adobe Workfront中的檢視概觀](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Adobe Workfront中的群組概觀](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

檢視或分組最重要的程式碼行是用來識別檢視欄或分組中參考之物件的行。 視此欄位是Workfront資料庫欄位的直接參照，還是數個欄位之間的計算而定，程式碼行開頭可能會是

```
valuefield
```

或

```
valueexpression
```

。

* [檢視和分組的Valuefield語法概觀](#valuefield-syntax-overview-for-views-and-groupings)
* [檢視和群組的值運算式語法概觀](#valueexpression-syntax-overview-for-views-and-groupings)

>[!TIP]
>
>* 雖然下列範例中的程式碼行在檢視和分組之間類似，請永遠記住，分組的每行程式碼都以分組編號開頭。
>
>  若要依專案清單或報表中的專案名稱分組，請針對第一層分組使用下列行：
>
>  
```>
>  group.0.valuefield=name
>  ```>
>* If you edit multiple columns in a view in the same column (as it is the case of shared columns), remember that every line of code for each column starts with the column number. 
>
>  
Use the following format to identify the first column of a view: 
>
>  
```>
>  column.0.valuefield=name
>  ```>
>  For information about sharing columns, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 
>



```
Valuefield
```

檢視和群組的語法概觀 {#valuefield-syntax-overview-for-views-and-groupings}

```
Valuefield=
```

是檢視和分組中的關鍵程式碼行，可識別您直接參照的物件。

分組和檢視的直接參考欄位語法相同。

使用參照Workfront物件時，適用下列規則

```
valuefield
```

行：

* 使用駝峰式大小寫直接參考欄位。

   **範例：** 若要在任務檢視中參照「任務實際完成日期」，請使用下列行：

   ```
   valuefield=actualCompletionDate
   ```

* 使用駝峰式大小寫和冒號來分隔相同物件彼此相關的欄位。

   **範例：** 若要在任務檢視中參照「專案計畫完成日期」，請使用下列行：

   ```
   valuefield=project:plannedCompletionDate
   ```

   如需物件在Workfront資料庫中如何相互參照的詳細資訊，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

* 參考自訂欄位時，請完全按照介面中顯示的欄位名稱來使用。

   **範例：** 若要在任務檢視中參照標示為「其他詳細資訊」的專案自訂欄位，請使用以下行：

   ```
   valuefield=project:Additional Details
   ```

 

```
Valueexpression
```

檢視和群組的語法概觀 {#valueexpression-syntax-overview-for-views-and-groupings}

您可以取代

```
valuefield=
```

程式碼行

```
valueexpression=
```

當您想要在2個或更多欄位之間參考計算時，在文字模式中建立檢視和群組時。

>[!TIP]
>
>雖然您可以建立可在報表中顯示的計算欄位，但計算檢視和分組更動態。 每次執行報表或顯示清單時，計算的檢視和群組都會重新整理為新資訊。
>
>如需有關在檢視中建立計算欄的資訊，請參閱 [計算自訂欄位與計算欄的比較](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

建立計算群組類似於在檢視中建立計算欄。

使用參照Workfront物件時，適用下列規則

```
valueexpression
```

行：

* 使用駝峰式大小寫直接參考欄位，並以大括弧括住每個欄位。

   **範例：** 若要使用在工作列中顯示任務名稱欄位

   ```
   valueexpression
   ```

   ，使用下列行：

   ```
   valueexpression={name}
   ```

* 使用駝峰式大小寫和句點來分隔彼此相關的欄位。

   **範例：** 若要在任務報表中顯示與任務名稱串連的專案名稱，請使用下列行：

   * 在檢視中：

      ```
      valueexpression=CONCAT({project}.{name},' - ',{name})
      ```

   * 在群組中：

      ```
      group.0.valueexpression=CONCAT({project}.{name},' - ',{name})
      ```
   如需物件在Workfront資料庫中如何相互參照的詳細資訊，請參閱 [API總管](../../../wf-api/general/api-explorer.md).

* 參考自訂欄位時，請使用下列規則：

   * 使用與介面中顯示的欄位名稱完全相同的名稱。
   * 在欄位名稱前面加上「DE：」。
   * 用大括弧括住欄位。
   * 依照句點分隔與物件相關的欄位。

   **範例：** 若要在valueexpression行的任務檢視中顯示「其他詳細資訊」專案自訂欄位，請使用下列行：

   ```
   valueexpression={project}.{DE:Additional Details}
   ```

* 您可以在中使用萬用字元

   ```
   valueexpression
   ```

   但不在

   ```
   valuefield
   ```

   行。

   如需萬用字元的詳細資訊，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

```
Valueformat
```

概觀

檢視或分組中第二重要的一行程式碼為

```
valueformat=
```

行。 這會告訴Workfront以哪種格式傳回您在

```
valuefield
```

或valueexpression行。 雖然您可以使用各種格式來

```
valueformat
```

行數，我們建議您在使用時

```
valueexpression
```

:

```
valueformat=HTML
```

### 篩選和自訂提示的語法

建立篩選器的語法與建立自訂提示的語法類似。

>[!TIP]
>
>您可以先為要包含在提示中的陳述式建立篩選器，以建立自訂提示。 以「&amp;」連線篩選器中的所有程式碼行，且行與之間沒有空格，這會成為您的自訂提示。

如需建立篩選器和自訂提示的詳細資訊，請參閱：

* [Adobe Workfront中的篩選器概觀](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [新增提示至報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)

如需有關在文字模式中建立篩選的資訊，請參閱 [使用文字模式編輯篩選器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

您可以使用以下元素在文字模式中建立篩選和自訂提示：

* 一行程式碼，參照filter陳述式的物件。 篩選物件使用駝峰式大小寫。
* 一行程式碼，參考濾鏡物件及濾鏡物件值的修飾元。 此行中的濾鏡物件使用駝峰式大小寫。

   >[!TIP]
   >
   >參考範圍時，這需要2個修正因子明細行。

* 連線多個篩選陳述式的陳述式聯結器：

   * 和

      這是篩選器陳述式之間的預設聯結器。

   * 或

      >[!TIP]
      >
      >陳述式聯結器區分大小寫，且一律大寫。 文字模式中可省略&quot;AND&quot;。

* 萬用字元，讓篩選器更動態，並針對目前時間或登入的使用者自訂篩選器。 如需萬用字元的詳細資訊，請參閱 [萬用字元篩選變數](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).
