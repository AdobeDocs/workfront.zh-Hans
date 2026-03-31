---
product-area: requests
navigation-topic: create-requests
title: 删除已提交的请求或请求草稿
description: 您可以在Adobe Workfront中删除已提交的请求或请求草稿。
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 3%

---

# 删除提交的请求或请求草稿

您可以删除已提交的Adobe Workfront或Adobe Workfront Planning请求，或您已创建或拥有管理权限的请求草稿。

Workfront管理员和Workfront Planning工作区管理员还可以删除未创建的请求和请求草稿。

您无法在旧版请求体验中查看Planning请求。

本文介绍了如何在新的请求体验中删除请求草稿。 删除Workfront和Planning请求或其草稿是相同的。

有关更多信息，请参阅：

* [创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [从草稿创建请求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [提交Adobe Workfront Planning请求以创建记录](/help/quicksilver/planning/requests/submit-requests.md)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何Workfront或工作流包</p>

<p>用于管理Planning请求的任何Workfront规划包 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员或Planning工作区管理员才能删除未创建的请求。</p><p>您必须具有“编辑”权限才能访问问题。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>您必须已创建请求或草稿才能在新的请求中将其删除，或者您必须是Workfront管理员或Planning工作区管理员才能删除未提交的请求草稿。
   </p><p>您必须对要删除的问题具有“编辑”权限。</p>  </td> 
  </tr>

</tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除新请求体验中的请求或请求草稿

您可以删除以下区域中的请求和草稿：

* 在Workfront的“请求”区域
* 在主页的“我的请求”小组件中
* 从请求页面

以下用户可以删除请求草稿：

* Workfront管理员可以删除他们或其他人提交的请求和草稿。
* Workfront Planning工作区管理员可以删除Planning工作区中由其管理的请求和草稿。
* 用户可以删除他们提交的请求和草稿。

### 从请求区域或主页中的我的请求小组件中删除请求或草稿

{{step1-to-requests}}

1. 要在&#x200B;**主页**&#x200B;中访问&#x200B;**我的请求**&#x200B;小组件，请执行以下操作：

   {{step1-to-home}}

   1. 找到&#x200B;**我的请求**&#x200B;构件。

      有关&#x200B;**我的请求**&#x200B;小组件的详细信息，请参阅[使用我的请求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在&#x200B;**请求**&#x200B;列表或&#x200B;**主页**&#x200B;中的&#x200B;**我的请求**&#x200B;小组件中，将鼠标悬停在要删除的请求或草稿上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)

1. 单击&#x200B;**删除**

   或

   右键单击选定的请求，然后单击&#x200B;**删除**。

   >[!TIP]
   >
   >当您无权创建问题时，您会收到一则警告，指出管理员限制您创建请求。

1. 在打开的对话框中，单击&#x200B;**删除**。

   删除请求或草稿。

   已删除的请求将保存在回收站中，Workfront管理员最多可以恢复30天。 无法恢复草稿。

### 从列表中批量删除请求

{{step1-to-requests}}

1. 要在&#x200B;**主页**&#x200B;中访问&#x200B;**我的请求**&#x200B;小组件，请执行以下操作：

   {{step1-to-home}}

   1. 找到&#x200B;**我的请求**&#x200B;构件。

      有关“我的请求”小组件的详细信息，请参阅[使用我的请求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在&#x200B;**请求**&#x200B;列表或&#x200B;**我的请求**&#x200B;构件中，单击要删除的每个请求左侧的框。
1. 在页面底部的蓝色栏中，单击&#x200B;**删除**。

   >[!NOTE]
   >
   >如果&#x200B;**删除**&#x200B;选项在蓝色条中不可见，则您没有权限删除一个或多个选定的请求。

### 删除请求草稿的先决条件

您必须先执行以下操作，然后才能删除请求草稿：

* 开始创建请求。 这会自动将请求保存为“草稿”部分中的草稿。

  有关创建请求的信息，请参阅[创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

## 删除旧版请求体验中的请求草稿

如果不再认为草稿相关，您可以在草稿形式保存后删除草稿请求。 无法恢复已删除的草稿请求。

无法从旧版请求体验访问Planning请求或其草稿。

{{step1-to-requests}}

1. 单击左侧面板中的&#x200B;**草稿**。

   所有请求队列的所有草稿都将显示在此列表中。

1. 在列表中选择草稿，然后单击列表顶部的&#x200B;**删除**。
1. 单击&#x200B;**是，将其删除**。

   草稿已删除，无法恢复。






