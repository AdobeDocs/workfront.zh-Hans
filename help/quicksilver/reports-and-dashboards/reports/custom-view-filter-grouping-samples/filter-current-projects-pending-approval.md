---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：顯示您目前擱置核准的專案」
description: 下列專案篩選器會顯示「目前 — 未決核准」狀態的專案，其中登入的使用者是專案贊助者或Portfolio經理。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# 篩選：顯示您目前擱置核准的專案

下列專案篩選器會顯示「目前 — 未決核准」狀態的專案，其中登入的使用者是專案贊助者或Portfolio經理。

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

## 篩選目前擱置核准的專案

若要套用此篩選器：

1. 前往專案清單。
1. 從 **篩選** 下拉式功能表，選取 **新增篩選器**.

1. 按一下&#x200B;**切換至文字模式**.
1. 在 **設定報告的篩選規則** 區域，複製並貼上下列程式碼：
   <pre>status=CUR：A<br>sponsorID=$$USER.ID<br>或:a:status=CUR：A<br>或:a:portfolio：ownerID=$$USER.ID</pre>

1. 按一下 **儲存篩選器**.
