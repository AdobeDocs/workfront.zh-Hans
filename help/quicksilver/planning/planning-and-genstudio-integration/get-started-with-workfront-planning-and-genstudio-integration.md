---
title: Workfront规划和GenStudio for Performance Marketing集成快速入门
description: 当您的公司同时购买这两个产品时，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作区。 了解有关如何使用此集成简化工作流的一些基础知识。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 9df59ea9b44baaf38c8db8f709f6b2fef1dc7c52
workflow-type: tm+mt
source-wordcount: '1357'
ht-degree: 0%

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

## 集成要求

* 必须将Workfront和GenStudio for Performance Marketing启用到同一组织。

  有关GenStudio的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)。

* 当您的公司有多个GenStudio实例时，Workfront Planning中将无法使用Workfront。<!--this will change-->

* Workfront实例是Adobe Unified Experience的一部分，包括使用Identity Management System (IMS)。

  有关信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 同时使用Planning和GenStudio的用户只能属于IMS组织中的一个Workfront实例。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

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
   <li><p> Adobe GenStudio for Performance Marketing</p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront Workflow包</p>  
<p>任何Workfront规划包</p>
   </td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio包</p></td> 
   <td> 
<p>???</p>

</td> </tr>

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
   <td role="rowheader"><p>Adobe GenStudio许可证</p></td> 
   <td><p> ???</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>  
   <p>GenStudio的配置： ???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  
   <p>在Workfront规划中： </p>
   <ul>
   <li><p>向工作区和记录类型提供或更高权限  </p> </li> 
   <li><p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p></li>
   </ul>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何权限</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中创建权限以创建项目</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
*有关Adobe GenStudio for Performance Marketing的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home)。


## Workfront Planning与GenStudio集成概述

以下各节描述了以下内容：

* 用于从GenStudio更新Workfront Planning信息的功能
* 用于从Workfront Planning更新GenStudio信息的功能
* 关于在GenStudio工作区中通过Workfront Planning可以管理或无法管理的内容的限制。

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### Workfront规划中的GenStudio工作区

* 如果贵组织有多个Workfront实例，则不会在任何Workfront实例中看到GenStudio工作区。<!-- this might change-->
* GenStudio工作区会显示一个可视指示器，以明确表示该工作区是从GenStudio导入的。 有关信息，请参阅[在Adobe Workfront规划中管理GenStudio工作区](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。
* 所有有权访问GenStudio和Workfront Planning的用户也可以在Workfront Planning中看到GenStudio工作区。
* Workfront Planning用户必须通过Adobe Identity Management System (IMS)进行管理，才能从Workfront查看和使用GenStudio工作区。

  仅Workfront用户无法查看GenStudio工作区，即使它在Workfront中可用也是如此。

  有关信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。


### 记录类型

* 您可以在Workfront Planning中从GenStudio编辑记录类型信息（例如其外观）。
* 您可以在Planning中与其他人共享GenStudio记录类型。
* 您可以在GenStudio工作区中从Planning创建记录类型。 这些记录类型仅保留在Planning中。 它们不会显示在GenStudio中。
* 与GenStudio同步的记录类型在Workfront Planning中显示一个视觉标志，明确表示记录类型是从GenStudio导入的。

### 记录

* 您可以在GenStudio中添加或删除记录，这些记录将在Workfront Planning中可见（或从中删除）。
* 您可以在Workfront Planning中添加或删除记录，记录将在GenStudio中可见（或从中删除）。
* 从Workfront Planning或GenStudio中删除记录时，这些记录将被放置在“最近删除”框中30天。 GenStudio没有最近删除的纸盒。
* 从“最近删除”框中恢复记录会将它们放回Workfront Planning和GenStudio。
* 您可以通过以下方式从Workfront Planning添加记录：

   * 使用“新建记录”按钮从任何视图中手动、从头开始
   * 通过使用CSV或Excel文件导入它们
   * 手动、内联、在表格视图中
   * 手动，直接在时间轴视图中

  有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* 您无法从Workfront Planning中创建或删除激活记录。
* 您可以在Planning的GenStudio工作区中，在Workfront Planning的任何可见字段中编辑有关所有记录的记录信息。

  有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

  <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### 字段

* 记录字段是从GenStudio导入的。 您可以在Workfront Planning中编辑字段设置。
* 如果您在Gen Studio中具有“管理”权限，则可以在Workfront Planning中为GenStudio记录类型创建字段。
* 在Planning中为GenStudio记录类型创建字段时，可从以下区域看到它们：
   * Planning视图
   * Planning记录详细信息页面
   * GenStudio记录详细信息页面

  >[!TIP]
  >
  >在Workfront Planning中创建的字段在GenStudio列表视图中不可见。

* 您可以在Planning中隐藏GenStudio记录类型的表视图中的字段。
* 您无法删除从Workfront Planning的GenStudio中导入的字段。
* 您可以从Workfront Planning中删除在Workfront Planning中为GenStudio记录类型创建的字段。


### “创建者”和“批准者”字段

* 您可以从Workfront Planning为Workfront Planning中的GenStudio记录类型添加“创建者”和“批准者”字段。
* 在“渠道”和“区域”记录类型中显示的记录将“系统”显示为由用户创建。 在Workfront Planning中创建GenStudio工作区时，会自动创建这些记录。
* 在Workfront Planning中提供工作区后在GenStudio中创建的记录将显示在创建者字段中创建该记录的IMS用户的名称，即使该用户在GenStudio中创建了这些记录且不是Workfront用户也是如此。
* 在提交请求表单以创建记录时，“批准者”字段显示批准者的姓名。

### 视图

* 您可以为GenStudio记录类型创建视图。

  有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

* 当您要共享Planning记录类型的视图时，可以共享GenStudio记录类型的视图。
* 无法在GenStudio中创建多个视图。

### 连接

* 您可以在GenStudio记录类型与Workfront Planning中的其他记录或对象类型之间建立以下连接：

   * 两种GenStudio记录类型
   * 来自同一工作区的GenStudio记录类型和Planning记录类型
   * 如果记录类型配置为从另一个工作区连接，则为来自另一个工作区的GenStudio记录类型和Planning记录类型。
   * GenStudio记录类型和Workfront对象类型（项目、项目组合、项目、公司、组）
   * GenStudio记录类型和AEM Assets对象类型。

### 请求表单和自动化

* 您可以在Workfront Planning中向GenStudio记录类型添加请求表单和自动化。

### 预览环境

* 可从生产环境访问的GenStudio工作区也会显示在预览环境中。
* 您可以在预览环境中在Workfront Planning的GenStudio工作区上执行本文中描述的所有活动，但这些更改不会转移到GenStudio。
只有您对生产环境中的项目所做的更改才会在Workfront Planning和GenStudio之间同步。
GenStudio没有“预览”环境。

