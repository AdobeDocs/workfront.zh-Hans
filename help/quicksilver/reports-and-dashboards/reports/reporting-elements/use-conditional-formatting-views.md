---
product-area: reporting
navigation-topic: reporting-elements
title: 在视图中使用条件格式
description: 在您与Adobe Workfront中的其他用户共享报表时，请考虑自定义报表视图、简化某些信息的阅读过程，或者干脆脱颖而出。
author: Lisa
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 2%

---

# 在视图中使用条件格式

在您与Adobe Workfront中的其他用户共享报表时，请考虑自定义报表视图、简化某些信息的阅读过程，或者干脆脱颖而出。

您可以通过向报表视图添加特殊或条件格式来自定义报表的详细信息选项卡。

您必须拥有报表的“管理”权限，才能编辑报表并为视图添加特殊格式。

有关创建报告的更多信息，请参阅文章 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

通过有条件地设置报表视图中的列格式，您可以设置影响报表显示方式的规则。 当满足这些条件或规则时，将应用特殊格式。

例如，如果任务完成百分比小于20%，则可以通过以粗体、红色文本和黄色背景颜色显示百分比数字来突出显示该字段。

通过有条件格式的视图，您可以：

* 更改列的标题。
* 将列的值更改为自定义文本或图像。
* 通过更改背景的字体类型、颜色、对齐方式或颜色来设置字段显示的格式。

您在报表视图中所做的更改仅在报表的“详细信息”选项卡中生效。 这些更改不会影响报表的“摘要”、“矩阵”或“图表”选项卡。

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
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以编辑报表中的视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理报表的权限以创建或编辑报表中的视图</p> <p>管理视图的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

您必须先创建报表，然后才能向其添加条件格式。

有关创建报表的信息，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## 创建有条件格式的视图

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **报表**.

1. 单击要在其中创建有条件格式视图的报表名称。

   或

   单击 **报表操作**，然后单击 **编辑**.

1. （视情况而定）如果您编辑了报表，请选择现有列，或创建新列。
1. 单击 **高级选项**.

1. 指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>自定义列标签</strong></td> 
      <td> <p>指定列的名称。</p> <p>如果正在编辑现有列，则在此处指定名称会更改现有列名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>字段格式</strong></td> 
      <td>选择列中显示值的格式。 根据列字段的内容，可设置日期、数字或货币的显示方式。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>在仪表板上显示此列</strong></td> 
      <td>如果希望在将报表置于功能板上时显示列，请选择此字段。 当您查看功能板外的报表时，将始终显示列。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **为此列添加规则**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 在 **当：** 中，为列设置条件语句。 例如：当任务完成百分比等于（区分大小写）50时。
1. 在 **显示如下字段：** 部分指定满足上述定义的条件时此字段的外观。

   指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>文本颜色</strong></td> 
      <td> <p>选择显示文本的颜色。 有8种颜色可供使用。</p> <p>注意：如果字段包含超链接，则文本颜色选择不会应用于此字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文本格式</strong></td> 
      <td>选择是显示粗体还是斜体文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文本对齐</strong></td> 
      <td>选择是将文本与列中的右对齐、居中对齐还是左对齐。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>背景</strong></td> 
      <td>选择文本的背景颜色。 有8种颜色可供使用。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>“显示”图标</strong></td> 
      <td>如果要显示图标而不是此列的实际值，请从16个图标中选择一个。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>显示文本</strong></td> 
      <td> <p>选择此选项可显示此列的自定义标签，而不是其实际值。 在提供的字段中指定要显示的文本，而不是值。</p> <p>重要信息：选择 <strong>显示文本</strong> 禁用内联编辑此列中文本的功能。<br>此外，您无法更改前置列的值，因为它包含内置逻辑。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>应用于整行</strong></td> 
      <td>选择此选项可将设置应用于整行，而不是仅将设置应用于选定列。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **添加规则**.\
   您可以向同一列添加其他规则，或向其他列添加规则。

   规则按创建顺序应用。 虽然列规则优先于同一单元格中的行规则，但它们会合并，但不会相互覆盖。

   示例1:您可以首先创建一个规则，规定当“项目状态”为“正在构建”时，文本颜色为紫色和粗体。 然后，再创建一个规则，规定“任务名称”不为空、文本颜色为红色和斜体，背景颜色为绿色。 在本例中，会发生以下情况：

   * 项目状态为“正在构建”的任务将以紫色和粗体文本显示。 如果任务名称不为空，则任务的背景也为绿色。
   * 其“项目状态”为“正在构建”以外的任何内容（“任务名称”不为空）的任务将以红色和斜体文本显示，背景为绿色。

   示例2:在项目计划完成日期上创建一个规则，该规则会影响整行，如果取消项目，则背景将变灰（状态=“无效”）。 然后，创建一个列规则，当项目计划完成日期小于今天时（即项目延迟），该列规则会将后台变为红色。 在此示例中，如果取消的项目的完成日期较晚，则即使行中的其他单元格为灰色，该单元格也将显示为红色。 要更正此格式：

   * 编辑计划完成日期的格式，并删除延迟项目中红色背景的列规则。
   * 添加格式与行规则相同的列规则（当项目状态=“无效”时，背景为灰色）。
   * 在较晚的项目上为红色背景再次添加列规则。
   * 保存规则和视图时，红色背景不会应用于已取消的项目。


1. 单击 **完成**.
1. 单击 **保存并关闭**.\
   在报表中，如果满足指定的条件，用户将看到格式的更改。
