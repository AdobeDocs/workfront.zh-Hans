---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：解析物件詳細資料時發生問題」
description: 此問題檢視顯示問題的解決物件的名稱和完成百分比，即使沒有解決任務或專案的存取權，問題建立者也可以洞察問題的進度。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# 檢視：解析物件詳細資料時發生問題

此問題檢視顯示問題的解決物件的名稱和完成百分比，即使沒有解決任務或專案的存取權，問題建立者也可以洞察問題的進度。

此檢視使用

```
sharecol=true
```

標籤以組合相同欄標題下的多個欄位。 如需詳細資訊，請參閱

```
sharecol
```

標籤，請參閱 [檢視：合併一個共用欄中多個欄的資訊](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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

## 檢視解析物件詳細資料的問題

1. 前往問題清單。
1. 從 **檢視** 下拉式功能表，選取 **新增檢視**.

1. 在&#x200B;**欄預覽** 區域，排除除一欄以外的所有欄。
1. 按一下剩餘欄的標頭，然後按一下 **切換至文字模式**.
1. 將滑鼠移到文字模式區域上，然後按一下 **按一下以編輯文字**.
1. 移除您在「 」中找到的文字 **文字模式** 方塊，並以下列程式碼取代：<pre>column.0.querysort=name</pre><pre>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=sourceobject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject)。HTML(name)<br>column.1.namekey=sourceobject.abbr<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=referenceObject：name<br>column.1.valueformat=HTML<br>column.1.viewalias=source<br>column.1.width=100<br>column.2.descriptionkey=assignedto<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=assignedTo：ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=assignedTo：objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo)。string(name)<br>column.2.namekey=assignedto<br>column.2.querysort=assignedTo：name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=assignedTo：name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=entryDate<br>column.3.valueformat=atDate<br>column.3.width=150<br>column.4.descriptionkey=description<br>column.4.linkedname=direct<br>column.4.listsort=string(description)<br>column.4.namekey=description.abbr<br>column.4.querysort=description<br>column.4.shortview=false<br>column.4.stretch=75<br>column.4.valuefield=description<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listsort=string(status)<br>column.5.namekey=status.abbr<br>column.5.querysort=status<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.type=enum<br>column.5.valuefield=status<br>column.5.valueformat=val<br>column.5.width=150<br>column.6.displayname=解析物件名稱<br>column.6.linkedname=resolveTask<br>column.6.namekey=view.relatedcolumn<br>column.6.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column.6.querysort=resolveTask：name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valuefield=resolveTask：name<br>column.6.valueformat=HTML<br>column.7.displayname=<br>column.7.linkedname=resolveOpTask<br>column.7.namekey=view.relatedcolumn<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask：name<br>column.7.sharecol=true<br>column.7.textmode=true<br>column.7.valuefield=resolveOpTask：name<br>column.7.valueformat=HTML<br>column.8.displayname=<br>column.8.linkedname=resolveProject<br>column.8.namekey=view.relatedcolumn<br>column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject：name<br>column.8.textmode=true<br>column.8.valuefield=resolveProject：name<br>column.8.valueformat=HTML<br>column.9.displayname=解析物件完成百分比<br>column.9.textmode=true<br>column.9.valueexpression=IF(ISBLANK({resolveTask})。{ID})，{resolveProject}。{percentComplete}，IF(ISBLANK({resolveProject})。{ID})，{resolveTask}。{percentComplete}，&quot;))<br>column.9.valueformat=doubleAsPercentRounded</pre>

1. 按一下 **儲存檢視**.
