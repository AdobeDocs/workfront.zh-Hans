---
product-area: requests
navigation-topic: create-requests
title: 删除已提交的请求重新请求草稿
description: 您可以删除已提交的请求或请求草稿。
author: Becky
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
source-git-commit: b58814d68d582a08457d1d4685d110c2bdd2087c
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 3%

---

# 删除提交的请求或请求草稿

您可以删除在新请求体验中创建的已提交的请求或请求草稿。 Workfront管理员和Planning工作区管理员也可以删除请求。

在旧版请求体验中，您可以删除请求草稿。 您无法删除已提交的请求。

有关信息，请参阅：

* [创建并提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [从草稿创建请求](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>参与者或更高版本</p>
   <p>请求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员或Planning工作区管理员才能删除未创建的请求。</p><p>您必须具有问题的编辑权限才能删除旧版请求体验中的草稿。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>您必须已创建请求或草稿才能在新的请求体验中删除它。</p><p>您必须具有问题的编辑权限才能删除旧版请求体验中的草稿。</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> 产品</td> 
   <td> <ul><li>Adobe Workfront</li><li>您必须拥有Adobe Workfront Planning才能查看Planning请求或请求表单</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除新请求体验中的请求或请求草稿

您可以在Workfront的请求区域或主页的“我的请求”小组件中删除请求。

* Workfront管理员可以删除其组织中的请求和草稿。
* Workfront Planning工作区管理员可以删除Planning工作区中他们管理的请求和草稿。
* 用户可以删除他们提交的请求和草稿。

### 从三个圆点式菜单中删除请求

{{step1-to-requests}}

1. 要在主页访问“我的请求”小组件，请执行以下操作：

   {{step1-to-home}}

   1. 找到“我的请求”构件。

      有关“我的请求”小组件的详细信息，请参阅[使用我的请求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在“请求”列表或“我的请求”小部件中，将鼠标悬停在要删除的请求或草稿上。

   出现“More（更多）”三点菜单。
   ![](assets/more-menu.png)

1. 单击请求或草稿名称右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**删除**。

   或

   右键单击选定的请求，然后单击&#x200B;**删除**。

   >[!TIP]
   >
   >当您无权创建问题时，您会收到一则警告，指出管理员限制您创建请求。

1. 在打开的对话框中，单击&#x200B;**删除**。

   删除请求或草稿。

### 批量删除请求

{{step1-to-requests}}

1. 要在主页访问“我的请求”小组件，请执行以下操作：

   {{step1-to-home}}

   1. 找到“我的请求”构件。

      有关“我的请求”小组件的详细信息，请参阅[使用我的请求](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md)。

1. 在请求列表或我的请求小部件中，单击要删除的每个请求左侧的框。
1. 在页面底部的蓝色栏中，单击&#x200B;**删除**。

   >[!NOTE]
   >
   >如果“删除”选项在蓝色栏中不可见，则您没有权限删除一个或多个选定的请求。

</div>

## 删除旧版请求体验中的请求草稿

如果不再认为草稿相关，您可以在草稿形式保存后删除草稿请求。 无法恢复已删除的草稿请求。

### 删除请求草稿的先决条件

您必须先执行以下操作，然后才能删除请求草稿：

* 开始创建请求。 这会自动在草稿部分中将请求另存为草稿。

  有关创建请求的信息，请参阅[创建和提交Adobe Workfront请求](../../../manage-work/requests/create-requests/create-submit-requests.md)。

### 删除请求草稿

{{step1-to-requests}}

1. 在左侧面板中选择&#x200B;**草稿**。

   所有请求队列的所有草稿都将显示在此列表中。

1. （可选）单击草稿列表右上角的&#x200B;**按请求类型筛选**，然后选择包含要显示的草稿的请求队列。
1. 在列表中选择草稿，然后单击列表顶部的&#x200B;**删除**。
1. 单击&#x200B;**是，将其删除**。

   草稿已删除，无法恢复。
