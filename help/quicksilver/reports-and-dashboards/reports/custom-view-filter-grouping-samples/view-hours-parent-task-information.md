---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：具有父系任務資訊的時數」
description: 此時數檢視會顯示記錄時數的任務名稱以及父系任務的名稱。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c24555fc-3bae-451b-8a44-28a8158199d1
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 0%

---

# 檢視：含有父系任務資訊的時數

此時數檢視會顯示記錄時數的任務名稱以及父系任務的名稱。

![custom_hour_view_with_task_and_parent_task_info.png](assets/custom-hour-view-with-task-and-parent-task-info-350x55.png)

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

## 檢視具有父系任務資訊的時數

1. 前往時數清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，排除除一欄以外的所有欄。
1. 按一下剩餘欄的標頭，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：
   <pre>column.0.aggregator.displayformat=doubleAsString<br>column.0.aggregator.function=SUM<br>column.0.aggregator.namekey=hours<br>column.0.aggregator.valuefield=hours<br>column.0.aggregator.valueformat=doubleAsDouble<br>column.0.descriptionkey=hours<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=doubleAsDouble(hours)<br>column.0.namekey=hours.abbr<br>column.0.querysort=hours<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=hours<br>column.0.valueformat=doubleAsString<br>column.0.width=150<br>column.1.descriptionkey=task<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=task：ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=task：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=task<br>column.1.listsort=nested(task)。string(name)<br>column.1.namekey=task<br>column.1.querysort=task：name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=task：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.description=父系任務名稱<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=task:parent:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=task：objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=task<br>column.2.listsort=nested(task：parent)。string(name)<br>column.2.name=父系任務名稱<br>column.2.querysort=task:parent:名稱<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=task:parent:名稱<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 按一下 **儲存檢視**.
