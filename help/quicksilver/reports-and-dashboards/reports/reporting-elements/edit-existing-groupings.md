---
title: 编辑现有分组
description: 编辑现有分组
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# 编辑现有分组

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is the third part of a former artcle split in 3: two how-tos and one refernece article about creating and customizing groupings)</p>
-->

您可以自定义最初创建或与您共享的现有分组。 然后，可将其另存为新分组。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的分组</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理报表的权限以编辑报表中的分组</p> <p>管理分组的权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

您必须先创建分组，然后才能对其进行编辑。

有关创建分组的信息，请参阅 [在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

## 操作步骤

1. 转到包含要自定义的分组的对象列表。
1. 单击 **分组** 图标。
1. 选择要自定义的分组，然后单击 **编辑** 图标。

   ![选择编辑图标。](assets/customizegrouping-nwe-standard-350x291.png)

   随即会打开用于自定义分组的界面生成器。

1. 在 **分组预览** ，单击 **添加分组** 定义您希望如何组织报表中的信息。 下面显示了分组在报表中的预览。

1. 开始键入表示您希望以何种方式组织报表中的信息的字段名称，然后在下拉列表中显示时单击该名称。
1. （可选和视情况而定）查看更新列表时，请选择 **默认情况下折叠此分组** 如果希望分组中的结果显示折叠而不是展开。 默认情况下，此设置处于禁用状态，分组结果始终显示在扩展列表中。

   有关更新列表和旧版列表的信息，请参阅文章中的“更新列表和旧版列表之间的差异”部分 [开始使用Adobe Workfront中的列表](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 当您在查看列表时手动调整分组时，Workfront会在您注销之前记住您的手动首选项。 当您重新登录时，将根据此设置显示列表。
   >* 在从图表元素或旧列表中访问分组后，分组结果始终会显示为已展开。 在这些情况下，将忽略此设置。


1. 重复步骤4、5和6以定义其他分组。\
   您最多可以定义三个分组来组织信息。 通过创建矩阵报告，您最多可以通过四个分组来进一步组织信息。 有关矩阵报表的更多信息，请参阅 [创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. 单击 **另存为新分组** 将当前分组替换为更改。
