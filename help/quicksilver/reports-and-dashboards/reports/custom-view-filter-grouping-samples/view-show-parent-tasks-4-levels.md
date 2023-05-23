---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：顯示上層任務最多4層深」
description: 此任務檢視在第一欄中顯示任務名稱，並在相同清單的不同欄中顯示最多4個父任務（如果存在）。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 檢視：顯示最多4層深的父系任務

此任務檢視在第一欄中顯示任務名稱，並在相同清單的不同欄中顯示最多4個父任務（如果存在）。

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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

## 顯示最多4層深的父系任務

1. 前往工作清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，排除除一欄以外的所有欄。
1. 按一下剩餘欄的標頭，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：

   ```
   column.0.descriptionkey=name
   ```

   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=parent<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=parent：ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=parent：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=parent<br>column.1.listsort=nested(parent)。string(name)<br>column.1.namekey=parent<br>column.1.querysort=parent：name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=parent：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=Parent Parent<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=parent:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=parent:parent:物件代碼<br>column.2.link.valueformat=val<br>column.2.linkedname=parent<br>column.2.listsort=nested(parent：parent)。string(name)<br>column.2.name=Parent Parent<br>column.2.querysort=parent:parent:名稱<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=parent:parent:名稱<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=Parent Parent Parent<br>column.3.link.linkproperty.0.name=ID<br>column.3.link.linkproperty.0.valuefield=parent:parent:parent：ID<br>column.3.link.linkproperty.0.valueformat=int<br>column.3.link.lookup=link.view<br>column.3.link.valuefield=parent:parent:parent：objCode<br>column.3.link.valueformat=val<br>column.3.linkedname=parent<br>column.3.listsort=nested(parent:parent:parent)。string(name)<br>column.3.name=Parent Parent Parent<br>column.3.querysort=parent:parent:parent：name<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=parent:parent:parent：name<br>column.3.valueformat=HTML<br>column.3.width=150<br>column.4.description=Parent Parent Parent Parent<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valuefield=parent:parent:父級:parent:ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.valuefield=parent:parent:父級:parent:物件代碼<br>column.4.link.valueformat=val<br>column.4.linkedname=parent<br>column.4.listsort=nested(parent:parent:parent：parent)。string(name)<br>column.4.name=Parent Parent Parent Parent<br>column.4.querysort=parent:parent:父級:parent:名稱<br>column.4.shortview=false<br>column.4.stretch=100<br>column.4.valuefield=parent:parent:父級:parent:名稱<br>column.4.valueformat=HTML<br>column.4.width=150</pre>

1. 按一下 **儲存檢視**.

   任務名稱會顯示在第一欄中，如果任務有任何父項，則最多會有4個父項顯示在剩餘的欄中。
