---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「群組：時數的專案贊助者」
description: 此時數分組會依時數記錄所在的專案贊助者組織時數。 時數分組的標準Report Builder介面不提供專案贊助者欄位的對應。 您必須使用文字模式介面才能存取此欄位。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 0%

---

# 分組：時數的專案贊助者

此時數分組會依時數記錄所在的專案贊助者組織時數。 時數分組的標準Report Builder介面不提供專案贊助者欄位的對應。 您必須使用文字模式介面才能存取此欄位。

![hour_report_grouped_by_sponder.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## 按專案贊助者分組（小時）

若要套用此群組：

1. 前往時數清單。
1. 從 **分組** 下拉式功能表，選取 **新群組**.

1. 按一下&#x200B;**切換至文字模式**.
1. 移除 **將報表分組** 區域。

1. 將文字取代為下列程式碼：

   <pre>group.0.linkedname=project:sponsor:名稱<br>group.0.name=<br>group.0.valuefield=project:sponsor:名稱<br>group.0.valueformat=HTML<br>textmode=true<br></pre>

1. 按一下 **儲存群組**.
