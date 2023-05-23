---
product-area: reporting
navigation-topic: reporting-elements
title: 在檢視中使用條件式格式
description: 當您在Adobe Workfront中與其他使用者共用報表時，請考慮自訂報表檢視、讓某些資訊更易於閱讀或突出。
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '1150'
ht-degree: 2%

---

# 在檢視中使用條件式格式

當您在Adobe Workfront中與其他使用者共用報表時，請考慮自訂報表檢視、讓某些資訊更易於閱讀或突出。

您可以新增特殊或條件式格式至報表的檢視，以自訂報表的詳細資訊標籤。

您必須擁有報表的管理許可權，才能編輯報表及將特殊格式新增至檢視。

如需建立報表的詳細資訊，請參閱文章 [建立自訂報表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

透過有條件地格式化報表檢視中的欄，您可以設定影響報表顯示方式的規則。 當滿足這些條件或規則時，將套用特殊格式。

例如，如果任務的完成百分比小於20%，您可以反白顯示以粗體、紅色文字和黃色背景顏色表示的百分比數字。

使用條件式格式檢視，您可以：

* 變更欄的標題。
* 將欄的值變更為自訂文字或影像。
* 變更字型型別、顏色、對齊方式或背景顏色，格式化欄位顯示。

您在報表檢視中所做的變更只有在報表的詳細資訊標籤中才會生效。 這些變更不會影響報告的「摘要」、「矩陣」或「圖表」標籤。

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
   <td> <p>編輯篩選器、檢視、群組的存取權</p> <p>編輯報告、儀表板、行事曆的存取權，以便編輯報告中的檢視</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>物件許可權</strong></td> 
   <td> <p>管理報表的許可權，以建立或編輯報表中的檢視</p> <p>管理檢視的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 必要條件

您必須先建立報表，才能在其中新增條件式格式。

如需建立報告的詳細資訊，請參閱 [建立報告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 建立條件式格式化檢視

1. 按一下 **主要功能表** 圖示 ![](assets/main-menu-icon.png) Workfront右上角，然後按一下 **報表**.

1. 按一下您要建立條件式格式檢視的報表名稱。

   或

   按一下 **報表動作**，然後按一下 **編輯**.

1. （視條件而定）如果您編輯了報表，請選取現有欄或建立新欄。
1. 按一下 **進階選項**.

1. 指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>自定义列标签</strong></td> 
      <td> <p>指定資料行的名稱。</p> <p>如果您正在編輯現有資料欄，在此指定名稱會變更現有資料欄名稱。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>字段格式</strong></td> 
      <td>選擇欄中值的顯示格式。 視欄欄位而定，這可讓您設定日期、數字或貨幣的顯示方式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>在仪表板上显示此列</strong></td> 
      <td>如果您希望報表置於儀表板時欄顯示，請選取此欄位。 當您在儀表板外檢視報表時，欄始終顯示。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **為此欄新增規則**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 在 **當：** 區段，設定欄的條件陳述式。 例如：當任務完成百分比等於（區分大小寫） 50時。
1. 在 **顯示欄位如下：** 區段會指定當上述定義的條件符合時，此欄位會是什麼樣子。

   指定下列資訊：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>文本颜色</strong></td> 
      <td> <p>選取顯示文字的顏色。 有8種顏色可供使用。</p> <p>注意：如果欄位包含超連結，則文字顏色選取範圍不會套用至此欄位。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文本格式</strong></td> 
      <td>選取要以粗體或斜體顯示文字。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文本对齐</strong></td> 
      <td>選取文字在欄內靠右、置中或靠左對齊。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>背景</strong></td> 
      <td>選取文字背景的顏色。 有8種顏色可供使用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>顯示圖示</strong></td> 
      <td>如果您想要顯示圖示而非此欄的實際值，請從16個圖示中選擇一個。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>显示文本</strong></td> 
      <td> <p>選取此選項以顯示此欄的自訂標籤，而不是其實際值。 指定要顯示的文字，而不是提供的欄位中的值。</p> <p>重要：選取 <strong>顯示文字</strong> 停用內聯編輯此欄中文字的功能。<br>此外，您無法變更「前置任務」欄的值，因為它包含內建邏輯。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>应用于整行</strong></td> 
      <td>選取此選項可將設定套用至整列，而非僅將設定套用至選取的欄。</td> 
     </tr> 
    </tbody> 
   </table>

1. 按一下 **新增規則**.\
   您可以將其他規則新增至相同欄，或將規則新增至其他欄。

   規則會依照其建立順序套用。 它們會合併，但不會互相覆寫，不過欄規則會優先於相同儲存格上的列規則。

   範例1：您可以先建立一個規則，說明專案狀態為建置時，文字顏色為紫色和粗體。 然後您建立第二個規則，說明任務名稱非空白、文字顏色為紅色和斜體，背景顏色為綠色的情況。 在此範例中，會發生下列情況：

   * 專案狀態為「正在建立」的任務會以紫色和粗體文字顯示。 如果任務名稱不是空白的，任務也會有綠色背景。
   * 「專案狀態」為「建置」以外任何專案（且「任務名稱」非空白）的任務會以紅色和斜體字顯示，且背景為綠色。

   範例2：在專案計畫完成日期建立會影響整列的規則，如果專案已取消（狀態=「廢棄」），則會將背景變灰。 然後建立一個欄規則，當專案計畫完成日期小於今天（表示專案延遲）時，將背景變成紅色。 在此範例中，如果取消的專案有延遲完成日期，則該儲存格會顯示為紅色，即使列中的其他儲存格為灰色。 若要更正此格式：

   * 編輯規劃完成日期的格式，並刪除延遲專案紅色背景的欄規則。
   * 新增格式與列規則相同的欄規則（專案狀態=「廢棄」時為灰色背景）。
   * 再次為延遲專案的紅色背景新增欄規則。
   * 當您儲存規則和檢視時，紅色背景不會套用至已取消的專案。


1. 按一下 **完成**.
1. 按一下 **儲存+關閉**.\
   在報表上，如果滿足指定的條件，使用者會看到格式的變更。
