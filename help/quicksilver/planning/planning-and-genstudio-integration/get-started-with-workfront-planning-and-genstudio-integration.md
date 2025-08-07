---
title: Workfront规划和GenStudio for Performance Marketing集成快速入门
description: 当您的公司同时购买这两个产品时，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作区。 了解有关如何使用此集成简化工作流的一些基础知识。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: b366841f3994468624a0c9b07d9de6f2f274cbe0
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 1%

---

# Workfront Planning与GenStudio for Performance Marketing集成入门

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->

同时使用Adobe Workfront Planning和Adobe GenStudio for Performance Marketing的组织通常会比GenStudio默认支持的更详细地定义营销概念，如促销活动、产品和角色。

GenStudio for Performance Marketing与Workfront Planning之间存在本机集成。 此集成允许Workfront Planning中的用户管理GenStudio中使用的促销活动、产品、角色、激活、渠道和区域。 它还允许他们配置GenStudio以引用Workfront Planning中的现有记录类型，从而创建更加互联和一致的营销工作流。

此集成帮助您避免重复的数据输入，保持规划和激活工作的一致性，并支持您的营销记录系统。

当您的公司同时购买这两个产品时，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作区。

通过Workfront Planning与GenStudio for Performance Marketing之间的集成，您可以：

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* 在Workfront Planning中查看GenStudio工作区。
* 在GenStudio中修改营销活动，并在Workfront Planning中实时更新相同信息。
* 在Workfront Planning中修改促销活动，并在GenStudio中实时更新相同信息。

## 访问要求

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p> 系统管理员</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>向工作区和记录类型提供或更高权限  </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。


## 集成要求

* 必须将Workfront和GenStudio for Performance Marketing启用到同一组织。
* 当您的公司有多个GenStudio实例时，Workfront Planning中将无法使用Workfront。<!--this will change-->

* Workfront实例是Adobe Unified Experience的一部分，包括使用Identity Management System (IMS)。

  有关信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 同时使用Planning和GenStudio的用户只能属于IMS组织中的一个Workfront实例。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->


## 在Workfront Planning中管理GenStudio工作区的注意事项

* 贵组织必须先购买Adobe GenStudio for Performance Marketing，然后才能在Workfront Planning中查看GenStudio工作区。

  有关GenStudio的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

  有关GenStudio与Workfront Planning集成的详细信息，请参阅[Workfront Planning与GenStudio for Performance Marketing集成入门](/help/quicksilver/planning/planning-and-genstudio-integration/get-started-with-workfront-planning-and-genstudio-integration.md)

* Workfront用户必须有权访问GenStudio，才能在Workfront Planning中查看GenStudio工作区。


* 以下部分介绍了在Workfront Planning的GenStudio工作区中，您可以和无法管理哪些内容的一些限制。

### Workfront规划中的GenStudio工作区

* 如果您的组织有多个Workfront实例，则只有一个Workfront实例可以显示您的GenStudio工作区。
* GenStudio工作区会显示一个可视指示器，以明确表示该工作区是从GenStudio导入的。

### 记录类型

* 您不能在Workfront Planning中从GenStudio编辑记录类型。
* 您无法从GenStudio与其他用户共享记录类型。 Workfront管理员可以在他们的规划区域中查看GenStudio工作区。
* 与GenStudio同步的记录类型会显示一个视觉标志，以明确表示记录类型是从GenStudio导入的。
* 在Planning中查看GenStudio工作区的用户可以与其他人共享其记录类型。

### 记录

* 您可以在GenStudio中添加或删除记录，这些记录将在Workfront Planning中可见（或从中删除）。
您可以在Workfront Planning中添加或删除记录，记录将在GenStudio中可见（或从中删除）。
* 您可以通过以下方式从Workfront Planning添加记录：

   * 手动，从头开始
   * 通过使用CSV或Excel文件导入它们

  有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* 您无法从Workfront Planning中创建或删除激活记录。
* 您可以在Workfront Planning的任何可见字段中编辑GenStudio工作区中所有记录的记录信息。

  有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

### 字段

* 所有记录字段均从GenStudio导入，无法编辑字段设置。
* 只有在GenStudio中拥有系统管理员访问权限时，才能在Workfront Planning中为GenStudio记录类型创建字段。
* 您可以在Planning中为GenStudio记录类型创建字段。 以下区域将显示这些字段：
   * Planning视图
   * Planning记录详细信息页面
   * GenStudio记录详细信息页面

  >[!TIP]
  >
  >在Workfront Planning中创建的字段在GenStudio列表视图中不可见。

* 您可以在Planning中隐藏GenStudio记录类型的表视图中的字段，但不能从Workfront Planning中删除字段。


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### 视图

* 您可以为GenStudio记录类型创建视图。 您无法编辑自动从GenStudio导入的视图，但可以更改GenStudio表格视图的视图元素。 例如，您可以修改表格视图中的筛选器、排序、分组、行颜色和行高。

  有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

* 您可以通过以下方式共享GenStudio记录类型的视图：

   * 复制视图链接
   * 将视图导出到文件（仅适用于表格视图）

### 连接

* 您无法从Planning中的GenStudio记录类型连接其他记录或对象类型。
* 您可以从Planning中的其他记录类型连接到GenStudio记录类型。
