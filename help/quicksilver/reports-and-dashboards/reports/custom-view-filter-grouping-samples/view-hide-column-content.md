---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：隱藏欄的內容」
description: 您可能想要隱藏檢視欄中的資訊。 您可以修改欄的文字模式來完成此操作。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# 檢視：隱藏欄的內容

您可能想要隱藏檢視欄中的資訊。 您可以修改欄的文字模式來完成此操作。

>[!TIP]
>
>* 您可以使用隱藏欄，依您不想顯示在檢視中的特定物件來排序。\
   >  例如，您可以在任務檢視中依「任務編號」排序，並從檢視中隱藏「任務編號」資訊。 在此情況下，欄中參照的物件有助於排序檢視，但該物件的資訊不會顯示在檢視中。
>* 當您隱藏欄時，請注意欄中的資訊是隱藏的，但該欄仍然存在於檢視中。
>


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
   <td> <p>請求修改檢視 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改檢視</p> <p><b>注释</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 範例：排序並隱藏任務檢視中的「任務編號」欄：

1. 前往工作清單。
1. 從 **檢視** 下拉式功能表，按一下 **新增檢視**.

1. 按一下 **新增欄** 並開始輸入「任務編號」 **顯示在此欄中** 欄位，然後在清單中顯示時選取它。

1. 按一下 **切換至文字模式**.
1. 暫留在文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：

   <pre><strong>displayname=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueformat=int<br><strong>width=0</strong></pre>此程式碼中使欄隱藏的重要變更包括：

   ```
   displayname
   ```

   此行必須為空白。

   ```
   valuefield
   ```

   此項已取代為 *值*、和必須空白。

   ```
   width
   ```

   ：根據欄位，此欄位的值必須為 *0* 或 *1*.

1. 按一下 **儲存**，則 **儲存檢視**.
