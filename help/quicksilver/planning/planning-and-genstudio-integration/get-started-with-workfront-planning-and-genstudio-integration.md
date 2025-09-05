---
title: Workfront规划和GenStudio for Performance Marketing集成快速入门
description: 当您的公司同时购买这两个产品时，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作区。 了解有关如何使用此集成简化工作流的一些基础知识。
hide: true
hidefromtoc: true
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
source-git-commit: 4745b93e02c9de087afbee752e0303280e52d688
workflow-type: tm+mt
source-wordcount: '1765'
ht-degree: 0%

---

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


# Adobe Workfront Planning与Adobe GenStudio for Performance Marketing集成入门

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

同时使用Adobe Workfront Planning和Adobe GenStudio for Performance Marketing的组织通常会比GenStudio默认支持的更详细地定义营销概念，如促销活动、产品和角色。

GenStudio for Performance Marketing与Workfront Planning之间存在本机集成。 此集成允许Workfront Planning中的用户管理GenStudio中使用的促销活动、产品、角色、激活、渠道和区域。 它还允许他们配置GenStudio以引用Workfront Planning中的现有记录类型，从而创建更加互联和一致的营销工作流。

当您的公司同时购买这两个产品时，即可在Adobe Workfront Planning中使用GenStudio for Performance Marketing工作区。

## 集成优势

通过Workfront Planning与GenStudio for Performance Marketing之间的集成，您可以：

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* 在Workfront Planning中查看GenStudio工作区。
* 在GenStudio中修改营销活动，并在Workfront Planning中实时更新相同信息。
* 在Workfront Planning中修改促销活动，并在GenStudio中实时更新相同信息。
* 避免输入重复的数据。
* 保持规划和激活工作的一致性。

## 集成要求

贵组织必须满足以下要求，Workfront Planning与GenStudio for Performance Marketing之间的集成才能存在：

* 必须将Workfront和GenStudio for Performance Marketing启用到同一组织。

  有关GenStudio的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* 您的Workfront实例是Adobe Unified Experience的一部分，包括使用Identity Management System (IMS)。

  有关信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。

* 同时使用Planning和GenStudio的用户必须只属于IMS组织中的一个Workfront实例。

  仅Workfront用户无法查看GenStudio工作区，即使它在Workfront中可用也是如此。

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## 访问要求

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<p>任何Workfront包</p>
<p>任何规划包</p>

</td> </tr>
   <tr> 
<td> 
   <p> 其他产品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p> 标准</p>
  </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing用户角色</p></td> 
   <td><p><ul><li>用于访问营销活动、产品和角色的任何GenStudio用户角色</li>
   <li>GenSudio System Manager访问激活和事件</li></ul>
   有关信息，请参阅<a href="https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">用户角色和权限</a>。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  
   <p>在Workfront规划中： </p>
   <ul>
   <li><p>管理GenStudio工作区的权限以更改工作区的架构、记录类型和字段</p></li>
   <li><p>向GenStudio工作区分配在GenStudio记录空间中添加、更新或删除记录的权限</p> </li>  
   </ul>
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <li><p> Adobe GenStudio for Performance Marketing中的任何权限</p></li>
   <li><p> 在Adobe GenStudio for Performance Marketing中创建权限以创建项目</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table>

有关Adobe Workfront Planning访问权限的信息，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。

有关Adobe GenStudio for Performance Marketing的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。


## Workfront Planning和GenStudio集成功能概述

根据贵组织拥有的Workfront实例数量，您在Planning中自动对GenStudio工作区具有以下权限：

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>一个Workfront实例</p></td> 
   <td> 
<p>Workfront Planning中有一个GenStudio工作区</p>
<p>所有有权访问GenStudio和Workfront Planning的用户都拥有GenStudio工作区的“管理”权限</p> 
</td> </tr>
   <tr> 
<td> 
   <p> Workfront的多个实例</p> </td> 
   <td> 
   <p>每个Workfront Planning实例都有一个GenStudio工作区</p>
<p>所有有权访问GenStudio和Workfront Planning的用户都拥有每个实例的GenStudio工作区的Contribute权限</p> </td> 
  </tr>

</tbody> 
</table>

有关Workfront Planning权限的信息，请参阅[在Adobe Workfront Planning中共享权限概述](/help/quicksilver/planning/access/sharing-permissions-overview.md)。

以下各节描述了以下内容：

* 用于从GenStudio更新Workfront Planning信息的功能
* 用于从Workfront Planning更新GenStudio信息的功能
* 关于在GenStudio工作区中通过Workfront Planning可以管理或无法管理的内容的限制。

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### GenStudio工作区

* 当您在GenStudio中更新GenStudio工作区时，更改在Planning的GenStudio工作区中可见。
* GenStudio工作区在Workfront Planning中显示一个视觉指示器，以标识它。

  Planning中的![GenStudio卡](assets/genstudio-card-with-tag-highlighted.png)

  有关信息，请参阅[在Adobe Workfront规划中管理GenStudio工作区](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md)。
* 当您在Planning中拥有GenStudio工作区的管理权限时，您可以：

   * 在Planning中更新GenStudio工作区（名称、描述、图标）
   * 创建分区
   * 添加记录类型
   * 与其他人共享

     您可以与没有GenStudio帐户的其他人共享GenStudio工作区。 您只能与组织的Identity Management System (IMS)中可用的用户共享它。<!--check to see this is correct-->
     <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* 当您在Planning中拥有GenStudio工作区的Contribute权限时，无法从Planning中修改工作区。

### GenStudio工作区中的记录类型

* 在GenStudio中编辑GenStudio记录类型时，更改在Planning的GenStudio工作区中可见。
* 在GenStudio和Planning中可见的记录类型在Workfront Planning中具有GenStudio指示器。

  Workfront Planning中的![GenStudio记录类型卡片](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* 当您在Planning中拥有GenStudio工作区的管理权限时，您可以从Workfront Planning执行以下操作：
   * 编辑GenStudio记录类型信息（其外观、高级设置）。
   * 与其他人共享GenStudio记录类型。
   * 创建记录类型。 这些记录类型仅保留在Workfront Planning中。 它们不会显示在GenStudio中。
* 当您在Planning中拥有GenStudio工作区的Contribute权限时，无法从Planning中修改GenStudio记录类型。

### GenStudio工作区中的记录

* 在GenStudio中编辑GenStudio记录时，更改在所有Workfront实例中的所有GenStudio工作区中均可见。
* 您无法从Workfront Planning中创建或删除激活记录。
* 当您在Planning中拥有GenStudio工作区的“管理”或“贡献”权限时，您可以从Workfront Planning执行以下操作：
   * 添加或删除记录，记录便会在GenStudio中可见（或从中删除）。

     从Workfront Planning或GenStudio中删除的记录将放在Workfront Planning最近删除的框中30天。 GenStudio没有最近删除的纸盒。
   * 从最近删除的站中恢复记录。 恢复已删除的记录会将它们放回Workfront Planning和GenStudio。
   * 通过以下方式添加记录：

      * 使用“新建记录”按钮从任何视图中手动、从头开始
      * 通过在表视图中使用CSV或Excel文件导入它们
      * 在Workfront Planning的任意视图中手动
      * 向Workfront中的记录类型请求表单提交请求。

  有关信息，请参阅[创建记录](/help/quicksilver/planning/records/create-records.md)。
* 您可以从Workfront Planning中编辑GenStudio工作区中所有记录的记录信息。

  有关信息，请参阅[编辑记录](/help/quicksilver/planning/records/edit-records.md)。

### GenStudio工作区中记录类型的字段

* 默认情况下，GenStudio记录字段会导入到Workfront Planning。
* 您不能在GenStudio中添加字段以记录类型。
* 当您在Planning中拥有GenStudio工作区的管理权限时，您可以从Workfront Planning执行以下操作：

   * 编辑GenStudio字段设置。
   * 如果您在Gen Studio中具有“管理”权限，请为GenStudio记录类型创建字段。

     在Planning中为GenStudio记录类型创建字段时，可从以下区域看到它们：

      * Workfront Planning视图
      * Workfront Planning记录详细信息页面
      * GenStudio记录详细信息页面

     >[!TIP]
     >
     >在Workfront Planning中创建的字段在GenStudio列表视图中不可见。

   * 在Planning中隐藏GenStudio记录类型的表视图中的字段。
&lt;！—*从Workfront Planning中删除在Workfront Planning中为GenStudio记录类型创建的字段。  — 根据Iskuhi，这是不可能的；链接存在，但会生成错误 — >

  <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* 在Planning中拥有GenStudio工作区的“Contribute”权限时：

   * 在Workfront Planning中，您无法从GenStudio工作区中编辑字段设置、删除或添加字段。
   * 您可以在Workfront Planning的表格视图中隐藏字段。

#### “创建者”和“批准者”字段

* 您可以从Workfront Planning为Workfront Planning中的GenStudio记录类型添加“创建者”和“批准者”字段。
* 在“渠道”和“区域”记录类型中显示的记录将“系统”显示为由用户创建。 在Workfront Planning中创建GenStudio工作区时，会自动创建这些记录。
* 在Workfront Planning中提供工作区后在GenStudio中创建的记录将显示在创建者字段中创建该记录的IMS用户的名称，即使该用户在GenStudio中创建了这些记录且不是Workfront用户也是如此。
* 在提交请求表单以在Workfront Planning的GenStudio记录类型中创建记录时，“批准者”字段显示批准者的名称。

### 在GenStudio工作区中记录视图

>[!NOTE]
>
>GenStudio记录类型显示在从GenStudio导入的默认表格视图中。
>
>您无法删除默认从GenStudio导入的原始表格视图。

* 无法在GenStudio中创建多个视图。

* 当您在Planning中拥有GenStudio工作区的管理权限时，您可以在Workfront Planning中执行以下操作：

   * 为GenStudio记录类型创建视图。

     有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

   * 重命名、共享、导出、复制或删除GenStudio记录类型中的任何自定义视图。

* 在Planning中拥有GenStudio工作区的Contribute权限后，您可以在Workfront Planning中执行以下操作：

   * 为GenStudio记录类型创建视图。

     有关信息，请参阅[管理记录视图](/help/quicksilver/planning/views/manage-record-views.md)。

   * 重命名、导出、复制或删除GenStudio记录类型中的自定义视图。

     在Workfront Planning中，您无法从GenStudio工作区共享视图

### 在GenStudio工作区中记录连接

您可以在具有“管理”权限的GenStudio工作区中的记录类型之间创建连接。

您可以在GenStudio记录类型与Workfront Planning中的其他记录或对象类型之间建立以下连接：

* 两种GenStudio记录类型
* 来自同一工作区的GenStudio记录类型和Planning记录类型
* 如果记录类型配置为从另一个工作区连接，则为来自另一个工作区的GenStudio记录类型和Planning记录类型。
* GenStudio记录类型和Workfront对象类型（项目、项目组合、项目、公司、组）
* GenStudio记录类型和AEM Assets对象类型。

### GenStudio记录类型的请求表单和自动化

* 您可以在Workfront Planning中将请求表单添加到GenStudio记录类型。

  有关信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。
* 您可以在Workfront Planning中为GenStudio记录类型配置自动化。

  有关信息，请参阅[配置Adobe Workfront计划自动化](/help/quicksilver/planning/records/configure-automations-to-create-records.md)。

## 预览环境

* 可从生产环境访问的GenStudio工作区也会显示在同一Workfront实例的“预览”环境中。
* 您可以在“预览”环境中的Workfront Planning的GenStudio工作区上执行本文中描述的所有活动，但这些更改不会从GenStudio中可见。

  只有您对生产环境中的项目所做的更改才会在Workfront Planning和GenStudio之间同步。

  GenStudio没有“预览”环境。

