---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：指派使用者的公司和主群組」
description: 此任務檢視會顯示任務之主要擁有者的公司和主群組。 這些值在標準介面中無法使用，但可透過文字模式存取。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 818c1f3a-4e82-4dc3-af86-4f9dcf5c11a4
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 檢視：指派使用者的公司和主群組

此任務檢視會顯示任務之主要擁有者的公司和主群組。 這些值在標準介面中無法使用，但可透過文字模式存取。

![](assets/view--assigned-user-s-company-and-home-group-350x80.png)

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

## 檢視指派使用者的公司和主群組

1. 前往工作清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，排除除一欄以外的所有欄。
1. 按一下剩餘欄的標頭，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：
   <pre>column.0.descriptionkey=name<br> column.0.link.linkproperty.0.name=ID<br> column.0.link.linkproperty.0.valuefield=ID<br> column.0.link.linkproperty.0.valueformat=int<br> column.0.link.lookup=link.view<br> column.0.link.valuefield=objCode<br> column.0.link.valueformat=val<br> column.0.linkedname=direct<br> column.0.listsort=string(name)<br> column.0.namekey=name.abbr<br> column.0.querysort=name<br> column.0.shortview=false<br> column.0.stretch=100<br> column.0.valuefield=name<br> column.0.valueformat=HTML<br> column.0.width=150<br> column.1.descriptionkey=assignedto<br> column.1.link.linkproperty.0.name=ID<br> column.1.link.linkproperty.0.valuefield=assignedTo：ID<br> column.1.link.linkproperty.0.valueformat=int<br> column.1.link.lookup=link.view<br> column.1.link.valuefield=assignedTo：objCode<br> column.1.link.valueformat=val<br> column.1.linkedname=assignedTo<br> column.1.listsort=nested(assignedTo)。string(name)<br> column.1.namekey=assignedto<br> column.1.querysort=assignedTo：name<br> column.1.shortview=false<br> column.1.stretch=0<br> column.1.valuefield=assignedTo：name<br> column.1.valueformat=HTML<br> column.1.width=150<br> column.2.description=指派給公司<br> column.2.displayname=指派給公司<br> column.2.linkedname=assignedTo：company<br> column.2.listsort=nested(assignedTo：company)。string(name)<br> column.2.namekey=assignedto<br> column.2.querysort=assignedTo:company:名稱<br> column.2.shortview=false<br> column.2.stretch=0<br> column.2.valuefield=assignedTo:company:名稱<br> column.2.valueformat=HTML<br> column.2.width=150<br> column.3.description=指派給主群組<br> column.3.displayname=指派給主群組<br> column.3.linkedname=assignedTo：homeGroup<br> column.3.listsort=nested(assignedTo：homeGroup)。string(name)<br> column.3.namekey=assignedto<br> column.3.querysort=assignedTo:homeGroup:名稱<br> column.3.shortview=false<br> column.3.stretch=0<br> column.3.valuefield=assignedTo:homeGroup:名稱<br> column.3.valueformat=HTML<br> column.3.width=150</pre>

1. 按一下 **儲存變更**.
