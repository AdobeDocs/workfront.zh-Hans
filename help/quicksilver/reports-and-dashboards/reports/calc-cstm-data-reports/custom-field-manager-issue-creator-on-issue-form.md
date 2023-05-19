---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 「計算自訂欄位範例：在問題自訂表單上顯示問題建立者的經理」
description: 使用計算出的自訂欄位，您可以在附加到問題的自訂表單上顯示問題建立者的經理姓名。 使用相同的陳述式，您可以為專案、問題和其他物件建立類似的計算欄位。
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 888c938e5d649557df69374a55d4e4ecc2da6f55
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 計算自訂欄位範例：在問題自訂表單上顯示問題建立者的管理員

使用計算出的自訂欄位，您可以在附加到問題的自訂表單上顯示問題建立者的經理姓名。 使用相同的陳述式，您可以為專案、問題和其他物件建立類似的計算欄位。

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## 存取需求

您必須具有下列存取權才能執行本文中的步驟：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront計畫*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront授權*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>存取層級設定*</td> 
   <td> <p>管理自訂表單的存取權<br>如需有關從存取層級授予管理存取許可權的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予使用者對特定區域的管理存取權</a>.</p> <p>注意：如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需Workfront管理員如何變更存取層級的詳細資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>物件許可權</p> </td> 
   <td> <p>為已附加表單的物件提供「編輯自訂表單」的存取權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 在問題自訂表單上顯示問題建立者的經理

以下步驟顯示如何為問題自訂表單建立計算欄位，您可以在其中擷取建立問題的使用者經理姓名。 例如，當您想要擷取建立任務、專案和投資組合之使用者的經理姓名時，程式是相同的。

1. 建立問題自訂表單，並在其中新增計算欄位。

   如需建立自訂表單及新增計算欄位的詳細資訊，請參閱下列文章：

   * [建立或編輯自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. 將下列文字模式程式碼複製並貼到 **計算** 自訂表單的欄位：

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >自訂欄位計算區分大小寫。

1. 按一下 **完成**，則 **儲存+關閉**.

   當包含欄位的表單附加到問題時，建立問題的使用者的管理員顯示在計算欄位中。
