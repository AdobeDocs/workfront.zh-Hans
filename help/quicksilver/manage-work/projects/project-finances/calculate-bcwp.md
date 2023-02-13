---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算已执行工作的预算成本(BCWP)
description: “已得值”(Reared Value， Budgeded Work of Performed， BCWP)是一个项目绩效量度，它表示在计算此量度时实际完成的任务量。
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 计算已执行工作的预算成本(BCWP)

## 已编入预算的工作成本概览

“已得值”(Reared Value， Budgeded Work of Performed， BCWP)是一个项目绩效量度，它表示在计算此量度时实际完成的任务量。

Adobe Workfront计算项目和任务的预算执行工作成本(BCWP)。

在审核任务或项目上BCWP的值时，请考虑以下事项：

* Workfront根据您对项目的性能索引方法(PMI)的配置计算任务的BCWP。

   您可以配置项目以使用小时或成本计算PMI，并且BCWP也使用相同的值计算。

   有关配置如何计算BCWP的信息，请参阅部分 [配置BCWP的计算方式](#configure-how-bcwp-is-calculated) 在本文中。

* Workfront通过添加项目上所有父任务和单个任务的所有BCWP值来计算项目的BCWP。

   子任务的值不会添加到项目的BCWP中。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 配置BCWP的计算方式 {#configure-how-bcwp-is-calculated}

您可以通过配置项目的性能索引方法(PIM)的计算方式，配置BCWP是以小时计算还是以成本计算。

1. 转到项目并展开 **项目详细信息** 中。
1. 在 **金融** 区域，找到 **性能指数方法** ，然后双击以编辑该字段。

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 从以下选项中进行选择：

   | 选项 | 如何执行计算 |
   |---|---|
   | 基于小时 | Workfront使用任务的“计划小时数”计算BCWP。 |
   | 基于成本 | Workfront使用任务的“计划成本”计算BCWP。 |

1. 单击 **保存更改**.

项目任务的BCWP使用小时或成本计算。

## 计算BCWP

Workfront使用以下公式计算任务或项目的已执行工作的预算成本(BCWP):

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

以下值用于这些计算：

| 使用的值 | 所用值的描述 |
|---|---|
| 实际完成百分比 | 这是任务在Workfront中显示的实际完成百分比。 |
| 任务预算 | 这是任务的“计划小时数”或“计划成本”的值。 |

例如，如果任务的实际完成百分比为25%，而任务预算或计划成本为$10,000，则任务的BCWP为：

```
BCWP = 25% x $10,000 = $2,500
```

## 找到项目或任务的BCWP

您可以通过向视图中添加BCWP列，在报表或列表中查看已执行的预算工作成本值。

1. 转到任务或项目列表。
1. 展开 **查看** 菜单和选择 **新建视图** 或 **自定义视图**.

1. 单击 **添加列**.
1. 在 **在此列中显示：** 字段开始键入 **BCWP** 并单击以在列表中显示时将其选中。

   ![](assets/bcwp-project-view.png)

1. 单击 **保存视图**.
1. BCWP字段将显示在视图中。
