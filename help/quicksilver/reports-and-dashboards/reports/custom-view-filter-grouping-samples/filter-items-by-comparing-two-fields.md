---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：比較兩個欄位來排除清單中的專案」
description: 您可以比較清單中專案的兩個欄位，藉此從清單中篩選專案。 例如，您只能顯示任務的「實際完成日期」晚於「計畫完成日期」的任務。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# 篩選：比較兩個欄位來排除清單中的專案

您可以比較清單中專案的兩個欄位，藉此從清單中篩選專案。 例如，您只能顯示任務的「實際完成日期」晚於「計畫完成日期」的任務。

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
   <td> <p>請求修改篩選器 </p>
   <p>計畫修改報告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改篩選器</p> <p><b>注释</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 比較兩個欄位以篩選專案

1. 前往工作清單。
1. 從 **篩選** 下拉式功能表，選取 **新增篩選器**.

1. 按一下 **新增篩選規則** 並新增 **實際完成日期** >**大於** > **選取日期**.

   >[!TIP]
   >
   >選擇您要用於所選欄位的篩選修正因子（若有的話）。

1. 按一下 **切換至文字模式**.
1. 在 **設定報告的篩選規則** 區域，新增下列程式碼：

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. 按一下 **完成**，則 **儲存篩選器**.
