---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: “过滤器：显示父任务
description: 您可以应用下面的任务过滤器来显示工作任务。 工作任务是可以独立工作的任务，而不是其他任务的父任务。 在一个示例中，过滤器标识了可能是父代的子任务。 在这种情况下，它们不是工作任务。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 过滤器：显示父任务

您可以应用下面的任务过滤器来显示工作任务。 工作任务是可以独立工作的任务，而不是其他任务的父任务。 在一个示例中，过滤器标识了可能是父代的子任务。 在这种情况下，它们不是工作任务。

>[!TIP]
>
>* 如果您考虑向报表添加多个过滤器，我们建议您使用报表生成器界面添加所有过滤器，并在添加所有其他过滤器规则后单击切换到文本模式。 然后，您可以为父任务筛选器添加代码，如上所述。 
* 我们还建议您为项目名称添加分组，以便更便于阅读报表。 有关将分组添加到报表的更多信息，请参阅文章 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>


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
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 显示没有子项的任务（它们可以有父项）

您可以将以下过滤器应用到任务报表，以显示没有子项的任务。 他们可以有自己的父母，也可以有其他工作的子女。

1. 从 **主菜单** ![](assets/main-menu-icon.png)，单击 **报表。**

1. 单击 **新建报表**.
1. 选择 **任务报表**.
1. 单击 **过滤器**.
1. 单击 **添加过滤器规则**.
1. 在 **开始键入字段名称……** 行，开始键入 **子项数量**.

1. 选择 **等于（区分大小写）** 对于修改量，输入 **0** 孩子的数量。\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   或

   单击 **切换到文本模式**，然后在文本编辑窗口中复制并粘贴以下文本： 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. 单击 **保存并关闭**.

   此操作将提取系统中所有正在工作任务的报表。 其中一些任务可能具有父项，但它们本身不是父项任务。

## 与父代一起显示任务（他们可以有子代）

您可以将以下过滤器应用到任务报表，以显示具有父代的任务，即子代任务。 但是，这些任务也可能具有自己的子项，因为过滤器不会排除其子项。 其他任务的父项子任务不被视为工作任务。

1. 从 **主菜单** ![](assets/main-menu-icon.png)，单击**报表。
1. 单击 **新建报表**.
1. 选择 **任务报表**.
1. 单击 **过滤器**.
1. 单击 **添加过滤器规则**.
1. 在 **开始键入字段名称……** 行，开始键入 **父ID**.
1. 选择 **不为空** 的URL。

   ![](assets/filter-parent-id-not-blank-350x100.png)

   或

   单击 **切换到文本模式**，然后在文本编辑窗口中复制并粘贴以下文本： 

   `parentID_Mod=notblank`

1. 单击 **保存并关闭**.

   这会为系统中具有父项和这些父项的子项任务的所有任务提取报表。 其中一些任务可能是父项本身。

## 显示无子项和无父项的任务（独立任务）

您可以将以下过滤器应用到任务报表以显示独立的工作任务。 这些任务没有父母，也没有自己的子女。

1. 从 **主菜单** ![](assets/main-menu-icon.png)，单击 **报表。**
1. 单击 **新建报表**.
1. 选择 **任务报表**.
1. 单击 **过滤器**.
1. 单击 **添加过滤器规则** 和 **开始键入字段名称……** 开始键入 **子项数量** 选择 **等于（区分大小写）** 对于修改量，输入 **0** 孩子的数量。
1. 单击 **添加其他过滤器规则** 和 **开始键入字段名称……** 开始键入 **父ID**，然后选择 **为空**.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   或

   单击，而不是步骤6-7 **切换到文本模式** 在文本编辑窗口中，复制并粘贴以下文本： 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. 单击 **保存并关闭**.

   这会为系统中没有父项或子项的所有任务提取报表。 这些是独立的工作任务。
