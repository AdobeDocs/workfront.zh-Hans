---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：將父系任務的名稱顯示為全部大寫」
description: 您可以將此欄新增至工作檢視，以所有大寫字母顯示父系工作的名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# 檢視：將父系任務的名稱顯示為全部大寫

您可以將此欄新增至工作檢視，以所有大寫字母顯示父系工作的名稱。

![](assets/column-task-with-all-caps-parent-350x112.png)

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
   <td> <p>請求修改篩選器、檢視和群組 </p>
   <p>計畫修改報表</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">存取層級設定*</td> 
   <td> <p>編輯報告、儀表板、行事曆的存取權以修改報告</p> <p>編輯對篩選器、檢視、群組的存取權以修改個別的檢視</p> <p><b>注释</b>

如果您仍然沒有存取權，請詢問您的Workfront管理員是否對您的存取層級設定了其他限制。 如需有關Workfront管理員如何修改您的存取層級的資訊，請參閱 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">建立或修改自訂存取層級</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">物件許可權</td> 
   <td> <p>管理報表的許可權</p> <p>如需請求其他存取許可權的詳細資訊，請參閱 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">要求物件的存取權 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;若要瞭解您擁有的計畫、授權型別或存取權，請聯絡您的Workfront管理員。

## 將父系任務的名稱顯示為全部大寫

若要在任務檢視中建立此欄：

1. 前往工作清單。
1. 從 **檢視** 下拉式功能表，選取 **自訂檢視**.\
   或\
   從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，按一下顯示清單中工作名稱的欄標題。
1. 按一下&#x200B;**切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代： <pre>descriptionkey=name<br>displayname=任務名稱<br>textmode=true<br>valueexpression=IF({numberOfChildren}>&quot;0&quot;，UPPER({name})，{name})<br>valueformat=HTML<br>width=150<br></pre>

1. 按一下 **儲存檢視**.
