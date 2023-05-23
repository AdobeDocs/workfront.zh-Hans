---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：在欄中新增任務後續任務清單」
description: 您可以將欄新增至任務檢視，以顯示任務的後續任務清單。 「任務後續任務」欄包含後續任務的編號和名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# 檢視：在欄中新增任務後續任務清單

您可以將欄新增至任務檢視，以顯示任務的後續任務清單。 此 **任務後置任務** 欄包含後置任務編號以及名稱。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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

## 在欄中新增任務後續任務清單

若要將此欄新增至工作檢視：

1. 前往現有任務檢視。
1. 展開「檢視」下拉式功能表，然後選取「 」 **自訂檢視**.
1. 按一下 **新增欄**.
1. 按一下 **切換至文字模式**.
1. 將滑鼠移至 **顯示在此欄中** 區域，然後按一下 **按一下以編輯文字**.

1. 移除「文字模式」方塊中的所有文字，並以下列程式碼取代：

   <pre>displayname=任務後續任務<br>清單分隔符號=<br><br>listmethod=nested(successors)。lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({succeast}。{taskNumber}，' - '，{subleast}。{name})<br>valueformat=HTML</pre>

1. 按一下 **儲存檢視**.
