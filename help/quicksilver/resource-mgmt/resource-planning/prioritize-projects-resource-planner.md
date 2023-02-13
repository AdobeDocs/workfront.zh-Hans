---
product-area: resource-management;projects
navigation-topic: resource-planning
title: 在资源计划器中排定项目优先级
description: 项目按优先级顺序在资源计划器中列出，其中最重要的项目位于顶部。
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# 在资源计划器中排定项目优先级

项目按优先级顺序在资源计划器中列出，其中最重要的项目位于顶部。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，包括对资源计划员中“编辑优先级”和“预算小时数”的访问权限</p> <p>编辑对财务数据、项目和用户的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要预算信息的项目的权限，并能够管理财务</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 资源计划器中项目的默认顺序

默认情况下，考虑以下标准后，这些项目会列在资源计划员的项目视图中。

>[!IMPORTANT]
>
>只有在您第一次打开资源计划器时，才会根据以下三个标准列出项目。 但是，此默认优先级会自动成为您的自定义优先级，并且在您执行以下任一操作时，该优先级将无法还原为原始优先级：
>
>* 随时单击保存。
>* 手动更改项目计划优先级时。 有关手动更改项目计划优先级的信息，请参阅部分 [人工更改项目计划优先级](#manually-change-the-project-planning-priority) 在本文中。
>
>在项目优先级成为您的自定义优先级后，项目信息中的任何更改将不再影响使用这些标准进行项目排序的过程。 在此之后，您只能手动排定项目的优先级。

在“项目视图”中列出项目的原始默认标准如下所示：

1. 按项目的“对齐分数”。\
   有关项目的“对齐分数”的更多信息，请参阅 [将记分卡应用于项目并生成对齐分数](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. 按项目的计划起始日期（如果“对齐”字段为空或与多个项目相同）。
1. 按字母顺序（如果“对齐”字段为空或相同，并且多个项目的“计划起始日期”相同）。

在资源计划器中处理项目优先级时，请考虑以下事项：

* 只有在应用“项目视图”时，才能手动自定义项目优先级。 这也会更改资源计划器中项目的顺序。
* 在资源计划器中应用“角色”或“用户”视图时，项目将按在“项目视图”中建立的优先级顺序显示。
* 资源计划器中项目的顺序对您而言是唯一的。 其他用户可以在资源计划器中查看相同的项目，但按不同的顺序查看。 您无法报告“项目计划优先级”字段。 此标记仅在资源计划器中可见，并用作对项目进行优先级排序的标记。

与项目组合关联的项目可能具有项目组合级别的优先级。 除了“资源计划员”优先级外，您还可以在“资源计划员”中查看项目的组合优先级。 您还可以根据项目组合的优先级来对项目进行排序。

## 人工更改项目计划优先级 {#manually-change-the-project-planning-priority}

要在资源计划器中对项目重新排序，您必须具有“编辑”资源管理访问权限和“管理项目”权限。

通过为项目赋予新的优先级，您可以按重要性对项目进行排名。

要编辑项目计划优先级，请执行以下操作：

1. 转到 **资源计划员**.

1. 在项目名称左侧的字段中单击包含数字的，然后输入一个数字以更改计划优先级，然后按Enter。\
   ![](assets/mceclip4.png)\
   或\
   将鼠标悬停在项目名称上，然后单击项目名称左侧的指示器，并将其拖放到正确的位置，以更改优先级。

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   当您选择项目优先级的数字时，请为较高（更重要）的优先级选择较低的数字，为较低（不太重要）的优先级选择较高的数字。 当将项目的优先级编号更改为较低的编号（优先级较高）时，“资源计划器”中的所有其他项目将在列表中向下移动（变得不那么重要）。\
   当将项目的优先级编号更改为较高的编号（较低的优先级）时，“资源计划器”中的所有其他项目将在列表中向上移动（变得更加重要）。

1. 单击&#x200B;**保存**。\
   项目的顺序会根据您的选择而更改，这将成为资源计划器中的自定义项目优先级。 其他用户在资源计划器中看不到项目的优先级顺序，不过他们可能能够在其资源计划器中查看相同项目。

## 在资源计划器中根据项目的Portfolio优先级对项目进行排序

>[!IMPORTANT]
>
>您的公司必须拥有业务或更高级别的Workfront计划，才能在Portfolio优化器中对项目进行优先排序。
>
>有关Workfront计划的更多信息，请参阅 [我们的计划](https://www.workfront.com/plans).
>
>有关在Portfolio优化器中对项目进行优先级排序的信息，请参阅 [在Portfolio优化器中排定项目的优先级](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. 打开 **资源计划员** 在 **项目视图**.
1. 单击 **设置** 图标。
1. 启用 **显示Portfolio优先级** 设置以根据项目分配给的Portfolio显示项目优先级。 根据项目组合的项目优先级显示在“资源计划员”优先级旁边。 默认情况下，此设置处于禁用状态。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   项目的组合优先级仅在资源计划员的“项目”视图中显示。

1. 单击 **订购** 根据项目组合的优先次序对项目进行排序。

   如果您的项目属于多个项目组合，则可以在资源计划器中看到具有相同项目组合优先级的多个项目。 在这种情况下，具有相同项目组合优先级的项目按以下顺序按以下标准列出：

   1. 一致性分数
   1. 计划开始日期
   1. 项目名称

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. 单击&#x200B;**保存**。

## 更改项目计划优先级对用户可用时间的影响

项目计划优先级会影响用户的可用小时数。 与具有最高优先级的项目关联的用户会根据其计划显示此项目的“可用小时数(AVL)”列的最大可用性。

按优先级顺序与第二个项目关联的同一用户将显示可用小时数值，该值是其可用小时数的全部金额与已在“已编入预算的小时数”列中为第一个项目编入预算的小时数之差，等等。 有关资源计划员中预算资源的信息，请参阅 [使用“项目”和“职责”视图在资源计划员中预算资源](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

如果用户没有为第一个项目（按优先级顺序）预算小时数，但为同一用户为第二个项目预算小时数，则用户将显示两个项目的全部可用小时数。

我们建议按资源计划器中项目的顺序为用户更新“预算小时数”列，以确保您随时都能准确地看到用户的可用小时数。

>[!NOTE]
>
>由于项目计划优先级对每个资源管理器都是唯一的，因此您的第二个优先级项目可能是另一个用户在其资源计划器中查看相同项目的第一个优先级项目。 如果另一个资源管理器为其第一个项目预算资源，则该资源的可用小时数将根据该更改而减少用于第一个项目的可用小时数。
>
>预算小时数的用户首先会分配该资源，并减少整个系统中该资源的可用小时数。 在资源计划器中为某个资源保存预算小时数后，所有用户的可用小时数应立即更新。
>
>有关可用小时数的更多信息，请参阅 [资源的可用性和分配](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
