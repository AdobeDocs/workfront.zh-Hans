---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：檔案報告，包含校訂連結」
description: 「檢視：檔案報告，包含校訂連結」
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# 檢視：包含校訂連結的檔案報告

在此檔案檢視中，您可以插入指向檔案目前版本的校訂的連結。

![](assets/view-document-with-proof-link-350x92.png)

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

## 檢視包含校訂連結的檔案報告

若要套用此檢視：

1. 前往檔案清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 按一下 **新增欄**.
1. 按一下 **切換至文字模式**.
1. 暫留在文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：

   ```
   displayname=Proof Link
   
   shortview=true
   
   textmode=true
   
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   
   valueformat=HTML
   ```

   >[!TIP]
   >
   >將「您的網域」取代為您的實際Workfront網域。 例如，如果貴公司的Workfront URL為 *Company.my.workfront.com*，您的網域為「公司」。

1. 按一下 **儲存**，則 **儲存檢視**.
1. 輸入檢視的名稱，然後按一下 **儲存檢視**.
1. （可選）若要確保只顯示含有校樣的檔案，請執行下列操作以新增篩選器：

   1. 按一下 **篩選** 下拉式功能表，然後按一下 **新增篩選器**.
   1. 按一下 **新增篩選規則** 並開始輸入校訂所有者，然後選取 **校訂所有者ID** 它會顯示在清單中。
   1. 選取 **不為空白** （篩選修飾元）。
   1. 按一下 **儲存篩選器**，輸入篩選器的名稱，然後按一下 **儲存篩選器**.

1. 按一下校訂連結欄中的連結以存取檔案最新版本的校訂。
