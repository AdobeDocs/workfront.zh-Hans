---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：使用者工作角色的FTE可用性百分比」
description: 您可以在使用者清單的檢視中新增欄位，以顯示與使用者相關聯的工作角色清單，以及每個工作角色的FTE可用性百分比（如使用者設定檔中所定義）。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 檢視：使用者職務角色的FTE可用性百分比

您可以在使用者清單的檢視中新增欄位，以顯示與使用者相關聯的工作角色清單，以及每個工作角色的FTE可用性百分比（如使用者設定檔中所定義）。

如需定義使用者FTE可用性百分比的相關資訊，請參閱 [編輯使用者的設定檔](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_availability_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

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

## 檢視FTE可用性的使用者工作角色百分比

1. 前往使用者清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，按一下 **新增欄**.

1. 按一下新欄的標題，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：

   <pre>displayname=角色時間百分比<br>清單分隔符號=<p><br>listmethod=nested(userRoles)。lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role}，'-'，{timePercentage}，'%')<br>valueformat=HTML</pre>

1. 按一下 **儲存**，則 **儲存檢視**.

1. （選用）指定檢視的名稱，然後按一下 **儲存檢視**.
