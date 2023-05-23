---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：任務和專案的原始問題詳細資訊」
description: 當問題轉換為任務或專案時，會在任務或專案與問題之間建立解決物件關係。 此檢視顯示任務或專案完成時自動完成問題的下列欄位 — 編輯我。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5fefb174-3a18-408f-aa12-3f4aff23acfa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---

# 檢視：任務和專案的原始問題詳細資訊

當問題轉換為任務或專案時，會在任務或專案與問題之間建立解決物件關係。 此檢視顯示任務或專案完成時自動完成之問題的下列欄位：

* 名称
* 输入日期
* 计划完成日期
* 实际完成日期
* 请求类型
* 建立者名稱
* 指派給使用者

![task_with_resolving_issue_fields.png](assets/task-with-resolving-issue-fields-350x38.png)

如需詳細資訊，另請參閱 [檢視：在任務和專案清單上顯示原始問題資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md).

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

## 檢視任務和專案的原始問題詳細資訊

1. 前往任務清單或專案清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，排除除一欄以外的所有欄。
1. 按一下剩餘欄的標頭，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 按一下 **儲存檢視**.
