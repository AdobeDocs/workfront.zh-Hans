---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「篩選：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案」
description: 您可以讓任務狀態指派給群組A命名的新狀態，並使用3個字母的索引鍵NST。 您可能會有另一個任務狀態指派給群組B，也命名為「新狀態」，帶有3個字母的索引鍵NES。 雖然2個狀態的名稱可以相同，但3個字母的代碼永遠都是唯一的。 如需群組狀態的詳細資訊，請參閱建立或編輯群組狀態。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# 篩選：當狀態與不同群組相關聯時，依相同名稱狀態顯示專案

您可以將任務狀態指派給名為的「群組A」 *新狀態* 使用3字母金鑰 *NST*. 您可能有另一個任務狀態指派給群組B，也命名為 *新狀態* 使用3字母金鑰 *無。* 雖然2個狀態的名稱可以相同，但3個字母的代碼永遠都是唯一的。\
如需群組狀態的詳細資訊，請參閱 [建立或編輯群組狀態](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

使用篩選產生器時，您無法識別2個同名狀態。 您必須使用「文字模式」來區分2種狀態。

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

## 當狀態與不同群組相關聯時，依同名狀態顯示專案

1. 例如，前往您要自訂的篩選器以取得工作清單。\
   這同樣適用於專案和問題。
1. 按一下 **新增篩選規則** 的 **狀態** 清單中物件的欄位。\
   例如，在任務報告中，新增 **狀態等於新狀態**，如果您只想顯示處於以下狀態的任務 **新狀態**.

   >[!TIP]
   >
   >請注意，您只有一個名為「新狀態」的狀態選項。

1. 按一下 **切換至文字模式**.\
   應顯示下列程式碼：

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >此處只顯示一個狀態。 狀態行會顯示其中一個狀態的3個字母的其中一個。

1. 新增下列2行程式碼，以新增篩選器中缺少的狀態：

   <pre>或:1:status=NES<br>或:1:status_Mod=in</pre>

1. 按一下 **完成**，則 **儲存篩選器**.

   清單會顯示群組A中狀態為「新狀態」以及群組B中狀態為「新狀態」的任務。
