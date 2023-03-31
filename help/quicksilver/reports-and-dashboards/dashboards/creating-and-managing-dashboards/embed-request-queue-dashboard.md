---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: 在功能板中嵌入请求队列
description: 您可以在功能板中嵌入新请求队列，以便向用户提供对请求队列的直接访问，而无需转到“请求”区域。
author: Nolan
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 2894161b61a00dab04c17ef642ace4a45179eb17
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# 在功能板中嵌入请求队列

您可以在功能板中嵌入新请求队列，以便向用户提供对请求队列的直接访问，而无需转到“请求”区域。 

例如，如果您有一个请求队列，该请求队列对整个组织开放，如“帮助台队列”或每个人都必须定期访问的PTO请求队列，则直接将请求队列插入其功能板中以便快速、轻松地访问可能会很方便。 此设置过程与在功能板中创建外部页面的过程类似。

首先，您需要获取请求队列的URL。 其次，您可以通过添加外部页面将URL嵌入功能板。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理功能板的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建以下两项，然后才能在功能板中嵌入请求队列：

* **功能板**:有关创建功能板的信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).
* **请求队列**:有关创建请求队列的信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## 获取请求队列的URL {#obtain-the-url-of-the-request-queue}

您可以通过多种方式获取请求队列的URL，具体取决于用户从功能板访问请求队列时要向用户显示的请求队列的哪个部分。

* [获取指向特定队列主题的链接，以便能够更改请求类型](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)
* [获取指向请求队列的链接并能够更改请求类型](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)
* [获取指向请求队列的链接，但无法更改请求类型](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### 获取指向特定队列主题的链接，以便能够更改请求类型 {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

与其他用户共享指向特定队列主题的链接时，将在他们提交请求所需的确切队列主题处打开请求表单。 当用户在记录特定请求队列的请求时可能不确定要选择哪个队列主题时，此功能非常有用。

用户可以更改请求类型或根据需要选择其他主题。 此时还会显示“请求”区域的导航。

1. 单击 **主菜单** > **请求** > **新请求**.
1. 如果要共享特定队列，请继续选择主题组和队列主题，直到您到达要在功能板上共享的队列为止。 有关提交请求的信息，请参阅 [创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >选择主题组和队列主题是可选的。

1. 单击 **共享路径** 中。

   此操作会复制在屏幕上显示请求队列或队列主题的链接。 用户可以更新请求类型或任何可用的主题组和队列主题。

   ![](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### 获取指向请求队列的链接并能够更改请求类型 {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

当您共享指向请求类型的链接时，将为用户选择请求类型。 当用户需要从同一请求类型的多个主题组或队列主题中进行选择时，此功能非常有用。 用户可以更改请求类型并选择另一个请求类型。 此时还会显示“请求”区域的导航。

1. 转到指定为请求队列的项目。

   有关从项目创建请求队列的信息，请转到 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 转到 **队列详细信息**.
1. 复制您在 **直接访问URL** 字段。

   该代码应类似于以下内容：

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   这是指与选定项目关联的请求队列的链接。 预选请求类型。

   用户可以选择所需的任何主题组或队列主题，也可以选择其他请求类型。

   ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### 获取指向请求队列的链接，但无法更改请求类型 {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

当您共享指向预先选择的请求类型的链接时，将为用户选择请求类型，并且无法更改（灰显）。 用户可以选择他们需要的主题组或队列主题。 当您不希望用户查看和选择其他请求类型时，此功能会很有帮助。 “请求”区域的导航不显示。

1. 转到指定为请求队列的项目。

   有关从项目创建请求队列的信息，请转到 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. 转到 **队列详细信息**.
1. 复制您在 **嵌入代码** 字段。

   该代码应类似于以下内容：

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. 编辑代码以仅保留以下信息：

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >您可以添加 `<samp>iframe </samp>` 标记时。

   这是指与选定项目关联的请求队列的链接。 请求类型已预选，无法更改。

   用户可以选择所选请求类型所需的任何主题组或队列主题。 用户无法选择其他请求类型。

   ![](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## 在功能板中嵌入请求队列

您可以将指向请求队列或嵌套在请求队列下的队列主题的链接嵌入功能板，以便用户直接访问进入请求。

1. 使用 [获取请求队列的URL](#obtain-the-url-of-the-request-queue) 本文章的章节。
1. 单击 **主菜单** > **功能板** > **新功能板**.
1. 键入 **名称** 中。 这是必填字段。
1. 单击 **添加外部页面**.

   ![](assets/add-external-page-highlighted---nwe-350x214.png)

1. 在 **添加外部页面** 框中，编辑以下字段：

   * **名称**:输入您希望请求队列在功能板中显示的名称。 这是必填字段。

   * **描述**:输入有关此外部页面显示的描述。 这不是必填字段，并且只有出于报告目的才重要。 它不会显示在功能板中。
   * **URL**:粘贴您使用步骤1中所述的方法之一获取的URL。

      <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <MadCap:conditionalText data-mc-conditions="">   
     (NOTE: ensure this stays accurate)   
     </MadCap:conditionalText>   
     </MadCap:conditionalText>   
     -->

   * **高度**:输入外部页面的高度。 这定义包含请求队列的外部页面在功能板上占用的空间。 这是必填字段，默认值为500。

1. 单击&#x200B;**保存**。
1. 单击 **保存并关闭**. 

   请求队列在功能板中显示为单独的功能板组件。

   ![](assets/new-dashboard-with-embedded-request-queue-nwe-350x260.png)

1. （可选）单击 **功能板操作**，则 **编辑** 将报表、日历或其他外部页面添加到同一功能板。\
   有关将组件添加到功能板的信息，请参阅 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

 

 

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted - old information)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
