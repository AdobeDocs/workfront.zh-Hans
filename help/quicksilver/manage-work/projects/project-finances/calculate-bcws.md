---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 计算已计划工作的预算成本(BCWS)
description: “已计划的工作成本”(BCWS)也称为“计划值”，它是一个项目绩效量度，它表示在计算此量度时应该完成的任务量。
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 计算已计划工作的预算成本(BCWS)

## 已计划工作成本预算概览(BCWS)

“已计划的工作成本”(BCWS)也称为“计划值”，它是一个项目绩效量度，它表示在计算此量度时应该完成的任务量。

Adobe Workfront计算项目和任务的已计划工作成本(BCWS)。

在审核任务或项目上BCWS的值时，请考虑以下事项：

* Workfront根据您对项目的性能索引方法(PIM)的配置计算任务的BCWS。

   您可以配置项目以使用小时或成本计算PIM，并且BCWS也使用相同的值计算。

   有关配置如何计算BCWS的信息，请参阅部分 [配置BCWS的计算方式](#configure-how-bcws-is-calculated) 在本文中。

* Workfront通过添加项目上所有父任务和各个任务中的所有BCWS值来计算项目的BCWS。

   子任务的值不会添加到项目的BCWS中。

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

## 配置BCWS的计算方式 {#configure-how-bcws-is-calculated}

您可以通过配置项目的性能索引方法(PIM)的计算方式，配置BCWS是以小时计算还是以成本计算。

1. 转到项目并单击 **项目详细信息** 中。
1. 在 **金融** 区域，找到 **性能指数方法** 字段，然后双击该字段以对其进行编辑。

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 从以下选项中进行选择：

   | 选项 | 如何执行计算 |
   |---|---|
   | 基于小时 | Workfront使用任务的“计划小时数”计算BCWS。 |
   | 基于成本 | Workfront使用任务的“计划成本”计算BCWS。 |


1. 单击 **保存更改**.

   项目任务的BCWS使用小时数或成本计算。

## 计算BCWS

Workfront使用以下公式计算任务或项目的已计划工作成本(BCWS):

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

此计算中使用了以下值：

| 使用的值 | 所用值的描述 |
|---|---|
| 计划完成百分比 | 这是任务完成百分比应该是的，方法是查看任务开始到今天之间经过的时间。 |
| 任务预算 | 这是任务的“计划小时数”或“计划成本”的值。 |

例如，如果今天是2月12日，而某项任务计划在2月10日到2月20日之间持续，则该任务应在今天完成20%。 如果任务预算（计划成本）为$10,000，则任务的BCWS为：

```
Task BCWS = 20% x $10,000 = $2,000
```

## 找到项目或任务的BCWS

您可以通过向视图中添加BCWS列，在报表或列表中查看已计划的预算工作成本值。

1. 转到任务或项目列表。
1. 展开 **查看** 菜单和选择 **新建视图** 或 **自定义视图**.

1. 单击 **添加列**.
1. 在 **在此列中显示：** 字段开始键入 **BCWS** 并单击以在列表中显示时将其选中。

   ![](assets/bcws-in-project-view.png)

1. 单击 **保存视图**.
1. 的 **BCWS** 字段。
