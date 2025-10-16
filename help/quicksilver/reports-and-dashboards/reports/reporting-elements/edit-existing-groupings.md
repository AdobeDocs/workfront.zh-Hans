---
title: 编辑现有分组
description: 编辑现有分组
author: Nolan
feature: Reports and Dashboards
exl-id: bd9e6794-3196-4a73-a86a-9ba6048e613b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# 编辑现有分组

<!-- Audited: 11/2024 -->

<!--NOTE: This is the third part of a former article split in 3: two how-tos and one reference article about creating and customizing groupings)-->

您可以自定义最初创建或与您共享的现有分组。 然后，您可以将其另存为新分组。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</strong></td> 
   <td> 
    <p>参与者或更高版本</p>
    <p>请求或更高版本</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板、日历的访问权限以编辑报告中的分组</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
    <td> <p>管理对报告的权限以编辑报告中的分组</p> <p>管理分组的权限</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 先决条件

必须先创建分组，然后才能对其进行编辑。

有关创建分组的信息，请参阅[在Adobe Workfront中创建分组](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)。

## 操作步骤

1. 转到包含要自定义的分组的对象列表。
1. 单击&#x200B;**分组**&#x200B;图标。
1. 选择要自定义的分组，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

   ![选择编辑图标。](assets/customizegrouping-nwe-standard-350x291.png)

   用于自定义分组的界面生成器将打开。

1. 在&#x200B;**分组预览**&#x200B;部分中，单击&#x200B;**添加分组**&#x200B;以定义您希望如何整理报告中的信息。 下面显示了报告中的分组预览。

1. 开始键入字段的名称，该名称表示要在报表中组织信息的方式，然后在信息出现在下拉列表中时单击它。
1. （可选且有条件）查看更新的列表时，如果希望分组的结果以折叠方式显示而不是展开，请选择&#x200B;**默认情况下折叠此分组**。 默认情况下，此设置处于禁用状态，分组的结果始终显示在展开列表中。

   有关更新列表和旧版列表的信息，请参阅[Adobe Workfront中的列表入门](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)一文中的“更新列表和旧版列表之间的差异”部分。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create grouping article and Common uses of text mode)</p>
   -->

   >[!TIP]
   >
   >* 当您在查看列表时手动调整分组时，Workfront会记住您的手动首选项，直到您注销。 重新登录时，将根据此设置显示列表。
   >* 从图表元素或旧版列表中访问分组结果后，这些结果始终以展开形式显示。 在这些情况下，此设置将被忽略。

1. 重复步骤4、5和6以定义其他分组。\
   您最多可以定义三个分组来组织信息。 通过创建矩阵报告，您最多可以将信息分为四组。 有关矩阵报表的详细信息，请参阅[创建矩阵报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md)。

1. 单击&#x200B;**保存分组**&#x200B;以使用更改替换当前分组。
