---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: 校对与GenStudio for Performance Marketing集成快速入门
description: 校对与GenStudio for Performance Marketing集成快速入门
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: e67446c6fb3e90d5dc45dd446988e5d02291f775
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# 校对与GenStudio for Performance Marketing集成快速入门

通过校对和GenStudio for Performance Marketing之间的集成，您可以

* 使用Workfront验证模板定义审阅和批准工作流

* 在验证查看器中审阅和批准GenStudio草稿内容

* 在GenStudio中查看审核决策以进行最终批准和发布


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> 
   <p>任何</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
   <p>当前：标准 </p> 
   <p>旧版：计划 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td> 
   <p> 您必须具有GenStudio for Performance Marketing，并且您必须在Admin Console中作为用户添加到产品中。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 集成要求

* Workfront和GenStudio for Performance Marketing必须部署到同一IMS组织。

* 用户只能属于IMS组织中的一个Workfront实例。

* 必须在Adobe Unified Experience上启用Workfront实例。

* 必须在Workfront设置区域中启用集成。


## 在Workfront中启用集成

1. 单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**[!UICONTROL 设置]**![设置图标](/help/_includes/assets/gear-icon-setup.png)。
1. 在左侧面板中，单击&#x200B;**审核和批准** > **Adobe GenStudio**。
1. 启用&#x200B;**使用校对审批**。
   ![为GenStudio启用校对](assets/enable-proofing-gs.png)

## 使用Workfront验证模板定义审批工作流

如果贵组织的内容审核流程经常重复或由同一人员审核，则可以使用验证模板来自动执行审核和批准工作流。

您可以仅为一个或两个审阅人创建简单的单阶段模板，也可以为具有许多阶段和依赖关系的复杂审阅创建自动的多阶段模板。

当用户在GenStudio中启动审核时，他们只需选择所需的模板即可。 用户可以随时轻松更改任何验证工作流模板，添加或删除审阅人和阶段。

使用验证工作流模板，您可以

* 添加特定用户并为每个用户分配指定的验证角色
* 设置截止日期
* 选择阶段激活时间
* 在阶段完成后锁定阶段
* 只需要一个决策
* 指定主要决策者
* 等等

有关自动化工作流和模板的详细信息，请参阅

* [自动化工作流概述](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [创建和管理自动化工作流模板](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

## 在验证查看器中审阅和批准GenStudio草稿内容

您可以在验证查看器中直接在GenStudio中查看和批准GenStudio草稿内容。

使用验证查看器，您可以

* 发表评论
* 标记草稿，显示需要更改的内容
* 做出决定

有关GenStudio中的审阅和批准的详细信息，请参阅<!--[Workfront Proof integration with GenStudio for Performance Marketing]().-->

## 在GenStudio中查看审核决策以进行最终批准和发布

资产完成审阅和批准流程后，您可以直接从GenStudio查看审阅决策并发布内容。

有关详细信息，请参阅<!--[link to GS docs]().-->
