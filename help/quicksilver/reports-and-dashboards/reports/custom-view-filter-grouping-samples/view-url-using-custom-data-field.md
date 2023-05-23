---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「檢視：使用自訂資料欄位的外部URL」
description: 您可以在任務檢視中使用名為「自訂URL」的計算自訂欄位，顯示內部自訂URL的連結。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# 檢視：使用自訂資料欄位的外部URL

您可以使用來顯示內部自訂URL的連結。 **計算自訂欄位** 在中命名為「自訂URL」 **任務檢視**.

這可協助您直接從報表快速從檢視中的特定物件連結至應用程式的某些區域。

建立計算自訂欄位時，您必須先建立欄位，然後建立檢視。

以下小節是任務的計算自訂欄位範例。 此自訂欄位稱為自訂URL。 自訂檢視會顯示欄位的值以及 **URL** 工作列位。

使用相同的步驟，您可以為系統中具有「自訂表單」的所有物件建立類似的計算自訂欄位和自訂檢視。

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

## 建立「自訂URL」計算自訂欄位

如需建立計算自訂欄位的詳細資訊，請參閱文章 [將計算資料新增至自訂表單](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

如果您有建立自訂表單的存取權，可以為名為「自訂URL」的任務建立計算自訂欄位。 此欄位會直接連結至 **概觀** 內的子標籤 **任務詳細資訊** 標籤。

1. 建立計算自訂欄位。
1. 在「計算」欄位中輸入下列代碼：

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;，&quot;/&quot;，&quot;task/&quot;，ID，&quot;/overview&quot;)

1. 取代&quot;`<domain>`」加上您的實際網域名稱，不帶括弧。

   此

   ```
   /overview
   ```

   此URL的一部分會將連結導向至 **概觀** 區段。

1. 建立您的 **計算自訂欄位**，附加 **自訂表單** 使用此欄位檢視Adobe Workfront中您想要在新檢視中顯示的多個任務。

## 建立檢視，顯示任務的「自訂URL」和「URL」欄位

任務 **檢視** 在以下範例中，顯示 **計算自訂欄位** 「自訂URL」稱為 **概觀** 任務中的子標籤&#x200B;**詳細資料** 標籤，以及 **URL** 任務的欄位。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

若要自訂此檢視：

1. 前往工作清單。
1. 展開 **檢視** 下拉式清單（位於工作清單頂端）。
1. 按一下 **自訂檢視**.
1. 移除檢視內的所有欄（第一欄除外）。
1. 按一下第一欄的標頭。
1. 按一下 **切換至文字模式** 位於介面的右上角。
1. 按一下 **按一下以編輯文字**.
1. 將下方的文字模式貼到一欄中。\
   在此範例中，&#39;column.1.&#39; 在「自訂URL」欄位中顯示值，作為任務的連結 **概觀**. &#39;欄。2.&#39; 顯示儲存在 **url欄位** 任務的。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=自訂URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString（自訂URL）<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString（自訂URL）<br>column.1.name=自訂URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=自訂URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. 按一下 **儲存檢視**.
