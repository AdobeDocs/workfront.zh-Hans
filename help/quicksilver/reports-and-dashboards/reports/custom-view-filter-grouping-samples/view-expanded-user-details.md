---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：展開的使用者詳細資訊」
description: 此「使用者」檢視會顯示關於使用者的資訊。 除了其名稱、存取層級和公司之外，它還會顯示其「群組」、「團隊」和「工作角色」的清單。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# 檢視：展開的使用者詳細資訊

此「使用者」檢視會顯示關於使用者的資訊。 除了其名稱、存取層級和公司之外，它還會顯示其「群組」、「團隊」和「工作角色」的清單。

![expanded_user_view.png](assets/expanded-user-view-350x75.png)

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

## 檢視展開的使用者詳細資訊

若要套用此檢視：

1. 前往使用者清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，排除除一欄以外的所有欄。
1. 按一下剩餘欄的標頭，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionkey=name <br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=accesslevel<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=accessLevel：ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=accessLevel：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=accessLevel<br>column.1.listsort=string(displayName)<br>column.1.namekey=accesslevel<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=accessLevel：displayName<br>column.1.valueformat=HTML<br>column.1.viewalias=accessLevel：displayName<br>column.1.width=100<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=val(objCode)<br>column.2.listdelimiter=<br>column.2.listmethod=nested(userGroups)。lists<br>column.2.namekey=group.plural<br>column.2.stretch=50<br>column.2.type=iterate<br>column.2.valuefield=group：name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.displayname=Teams<br>column.3.listdelimiter=<br>column.3.listmethod=nested(teams)。lists<br>column.3.textmode=true<br>column.3.type=iterate<br>column.3.valueexpression={name}<br>column.3.valueformat=HTML<br>column.4.link.linkproperty.0.name=ID<br>column.4.link.linkproperty.0.valuefield=ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.value=val(objCode)<br>column.4.listdelimiter=<br>column.4.listmethod=nested(userRoles)。lists<br>column.4.namekey=jobrole.plural<br>column.4.stretch=50<br>column.4.type=iterate<br>column.4.valuefield=role：name<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=company<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=company：ID<br>column.5.link.linkproperty.0.valueformat=int<br>column.5.link.lookup=link.view<br>column.5.link.valuefield=company：objCode<br>column.5.link.valueformat=val<br>column.5.linkedname=company<br>column.5.listsort=nested(company)。string(name)<br>column.5.namekey=company<br>column.5.querysort=company：name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=company：name<br>column.5.valueformat=HTML<br>column.5.width=150</pre>

1. 按一下 **儲存檢視**.
