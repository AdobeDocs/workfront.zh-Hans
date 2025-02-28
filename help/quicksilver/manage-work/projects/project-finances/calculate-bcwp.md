---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算已执行工作的预算成本(BCWP)
description: 预算执行工作成本(BCWP)也称为实现值，是一个项目绩效指标，它表示计算此指标时实际完成的任务数量。
author: Lisa
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# 计算已执行工作的预算成本(BCWP)

## 已执行工作的预算成本概览(BCWP)

预算执行工作成本(BCWP)也称为实现值，是一个项目绩效指标，它表示计算此指标时实际完成的任务数量。

Adobe Workfront计算项目和任务的已执行工作预算成本(BCWP)。

在查看任务或项目上的BCWP的值时，请考虑以下事项：

* Workfront根据您对项目绩效指数方法(PMI)的配置计算任务的BCWP。

  您可以将项目配置为使用小时数或成本计算PMI，并且使用相同的值计算BCWP。

  有关配置BCWP计算方式的信息，请参阅本文中的[配置BCWP计算方式](#configure-how-bcwp-is-calculated)部分。

* Workfront通过添加项目上所有父任务和单个任务的所有BCWP值来计算项目的BCWP。

  子任务的值未添加到项目的BCWP。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>编辑对项目的访问权限</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理项目的权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置BCWP的计算方式 {#configure-how-bcwp-is-calculated}

通过配置项目绩效指数方法(PIM)的计算方式，可以配置BCWP是以小时还是成本计算的。

1. 转到某个项目，然后展开左侧面板中的&#x200B;**项目详细信息**。
1. 在&#x200B;**财务**&#x200B;区域中，找到&#x200B;**绩效索引方法**&#x200B;字段并双击以对其进行编辑。

   ![PIM选项](assets/pim-options-hour-cost-based-nwe.png)

1. 从以下选项中选择：

   | 选项 | 如何执行计算 |
   |---|---|
   | 基于小时 | Workfront使用任务的已计划小时数计算BCWP。 |
   | 基于成本 | Workfront使用任务的计划成本计算BCWP。 |

1. 单击&#x200B;**保存更改**。

项目上任务的BCWP使用小时数或成本计算。

## 计算BCWP

Workfront使用以下公式计算任务或项目的已执行工作预算成本(BCWP)：

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

以下值用于这些计算：

| 使用的值 | 所用值的描述 |
|---|---|
| 实际完成百分比 | 这是显示在Workfront中的任务的实际完成百分比。 |
| 任务预算 | 这是任务的计划小时数或计划成本的值。 |

例如，如果任务的实际完成百分比为25%，任务预算或计划成本为$10,000，则任务的BCWP为：

```
BCWP = 25% x $10,000 = $2,500
```

## 为项目或任务找到BCWP

通过将BCWP列添加到视图，您可以在报表或列表中查看已执行工作的预算成本值。

1. 转到任务或项目列表。
1. 展开&#x200B;**视图**&#x200B;菜单并选择&#x200B;**新建视图**&#x200B;或&#x200B;**自定义视图**。

1. 单击&#x200B;**添加列**。
1. 在&#x200B;**在此列显示：**&#x200B;字段中，开始键入&#x200B;**BCWP**，然后单击以将其选中。

   项目视图中的![BCWP](assets/bcwp-project-view.png)

1. 单击&#x200B;**保存视图**。
1. BCWP字段将显示在视图中。
