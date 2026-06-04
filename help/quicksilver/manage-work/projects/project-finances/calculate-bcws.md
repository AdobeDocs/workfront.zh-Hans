---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算计划工作的预算成本(BCWS)
description: 计划工作预算成本(BCWS)也称为计划值，是一个项目性能量度，它表示计算此量度时应该完成的任务数量。
author: Lisa
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
TQID: https://experienceleague.adobe.com/Nt0HZv7YfcMsAXZr3xRlkGXtCrQPJeJd4IQB0BuhbVM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 600
ht-degree: 4%

---

# 计算计划工作的预算成本(BCWS)

## 计划工作预算成本(BCWS)概览

计划工作预算成本(BCWS)也称为计划值，是一个项目性能量度，它表示计算此量度时应该完成的任务数量。

Adobe Workfront计算项目和任务的计划工作预算成本(BCWS)。

在查看任务或项目上的BCWS的值时，请考虑以下事项：

* Workfront会根据您对项目绩效指数方法(PIM)的配置计算任务的BCWS。

  您可以将项目配置为使用小时数或成本计算PIM，并且使用相同的值计算BCWS。

  有关配置BCWS计算方式的信息，请参阅本文中的[配置BCWS计算方式](#configure-how-bcws-is-calculated)部分。

* Workfront计算项目的BCWS时，会将项目中所有父任务和单个任务的所有BCWS值相加。

  子任务的值不会添加到项目的BCWS。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对项目的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理项目的权限</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置BCWS的计算方式 {#configure-how-bcws-is-calculated}

通过配置项目绩效指数方法(PIM)的计算方式，可以配置BCWS是以小时还是成本计算的。

1. 转到某个项目，然后单击左侧面板中的&#x200B;**项目详细信息**。
1. 在&#x200B;**财务**&#x200B;区域中，找到&#x200B;**绩效索引方法**&#x200B;字段并双击它以进行编辑。

   ![PIM选项](assets/pim-options-hour-cost-based-nwe.png)

1. 从以下选项中选择：

   | 选项 | 如何执行计算 |
   |---|---|
   | 基于小时 | Workfront使用任务的已计划小时数计算BCWS。 |
   | 基于成本 | Workfront使用任务的计划成本计算BCWS。 |


1. 单击&#x200B;**保存更改**。

   项目上任务的BCWS使用小时数或成本进行计算。

## 计算BCWS

Workfront使用以下公式计算任务或项目的计划工作预算成本(BCWS)：

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

在此计算中使用以下值：

| 使用的值 | 使用的值描述 |
|---|---|
| 计划完成百分比 | 通过查看从任务开始到今天之间的间隔时间，可以得出任务的完成百分比。 |
| 任务预算 | 这是任务的计划小时数或计划成本的值。 |

例如，如果时间为今天2月12日，并且任务计划从2月10日持续到2月20日，则任务应于今天完成20%。 如果任务预算（计划成本）为$10,000，则任务的BCWS为：

```
Task BCWS = 20% x $10,000 = $2,000
```

## 找到项目或任务的BCWS

通过将BCWS列添加到视图，您可以在报表或列表中查看计划工作的预算成本值。

1. 转到任务或项目列表。
1. 展开&#x200B;**视图**&#x200B;菜单并选择&#x200B;**新建视图**&#x200B;或&#x200B;**自定义视图**。

1. 单击&#x200B;**添加列**。
1. 在&#x200B;**在此列显示：**&#x200B;字段中，开始键入&#x200B;**BCWS**，然后单击以将其选中。

   项目视图中的![BCWS](assets/bcws-in-project-view.png)

1. 单击&#x200B;**保存视图**。
1. **BCWS**&#x200B;字段显示在视图中。
