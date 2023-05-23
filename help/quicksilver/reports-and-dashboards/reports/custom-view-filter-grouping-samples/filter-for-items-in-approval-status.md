---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：僅顯示處於核准狀態的專案」
description: 您只能顯示目前處於「未決核准」中特定狀態的專案。 這對具有核准狀態的任何其他物件具有相同作用。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# 篩選：僅顯示處於核准狀態的專案

您只能顯示目前處於「未決核准」中特定狀態的專案。 這對具有核准狀態的任何其他物件具有相同作用。

您可以將下列物件置於核准狀態：

* 任务
* 问题
* 项目

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

## 僅顯示處於核准狀態的專案

1. 例如，前往您要為專案清單自訂的篩選器。
1. 按一下 **新增篩選規則** 的 **狀態** 清單中物件的欄位。\
   例如，在專案報告中，新增 **狀態等於Planning**，如果您只想顯示處於以下狀態的專案： **計畫 — 未決核准**.

1. 按一下 **切換至文字模式**.
1. 修改

   ```
   status
   ```

   藉由新增行 **：A** 至狀態的3字母金鑰：
   <pre>status=PLN：A<br>status_Mod=in</pre>

1. 按一下 **完成**，則 **儲存篩選器**.

   清單僅顯示處於「計畫 — 未決核准」狀態的專案。
