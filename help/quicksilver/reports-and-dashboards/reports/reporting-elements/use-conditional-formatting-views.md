---
product-area: reporting
navigation-topic: reporting-elements
title: 在视图中使用条件格式
description: 在与Adobe Workfront中的其他用户共享报表时，请考虑自定义报表视图，以使某些信息更易于阅读或引人注目。
author: Nolan
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 2%

---

# 在视图中使用条件格式

<!--Audited: 01/2024-->

在与Adobe Workfront中的其他用户共享报表时，请考虑自定义报表视图，以使某些信息更易于阅读或引人注目。

通过向报表视图添加特殊或条件格式，您可以自定义报表的详细信息选项卡。

有关创建报告的详细信息，请参阅文章[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

通过有条件地设置报表视图中的列格式，您可以设置影响报表显示方式的规则。 当满足这些条件或规则时，将应用特殊格式。

例如，如果任务的完成百分比小于20%，您可以通过以粗体、红色文本和黄色背景颜色显示百分比数字来突出显示字段。

对于有条件的格式化视图，您可以：

* 更改列的标题。
* 将列的值更改为自定义文本或图像。
* 通过更改字体类型、颜色、对齐方式或背景颜色来设置字段显示的格式。

您在报告视图中所做的更改仅在报告的详细信息选项卡中生效。 这些更改不会影响报告的“摘要”、“矩阵”或“图表”选项卡。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>新增：</p> 
   <ul><li>报告视图的标准</li>
  <li> 列表视图的参与者或更高版本</li></ul>

<p>当前：</p>
   <ul>
    <li> 规划报告视图 </li>
    <li> 请求或更高版本以访问列表视图 </li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板、日历的访问权限以编辑报告中的视图</p> <p><b>注释</b></p> <p>如果您没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理对报告的权限以创建或编辑报告中的视图</p> <p>管理视图的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

## 先决条件

必须先创建报表，然后才能将条件格式添加到其视图。

有关创建报告的信息，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)。

## 创建条件格式化视图

{{step1-to-reports}}

1. 单击要在其中创建条件格式视图的报表的名称

   或

   单击&#x200B;**新建报告**，然后选择对象类型以生成新报告。

1. （视情况而定）如果您编辑现有报表，请单击&#x200B;**报表操作**，然后单击&#x200B;**编辑**。

1. 在&#x200B;**列（视图）**&#x200B;选项卡中，单击以选择现有列，或单击&#x200B;**添加列**&#x200B;以创建列。
1. 在Report Builder左上角的&#x200B;**在此列显示**&#x200B;字段中，选择要在新列中显示的字段。
1. 单击&#x200B;**高级选项**。

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
      <td>选择列中值的显示格式。 根据列字段的内容，允许您设置日期、数字或货币的显示方式。 并非所有列都显示此选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>在仪表板上显示此列</strong></td> 
      <td>如果希望报表放在仪表板上时显示列，请选择此字段。 当您在仪表板外查看报表时，列始终显示。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**添加此列的规则**。

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. 在&#x200B;**当：**&#x200B;部分中，为该列设置条件语句。

   例如：“当任务完成百分比等于（区分大小写）50时。”
1. 在&#x200B;**显示这样的字段：**&#x200B;部分中，指定当满足以上定义的条件时，此字段的外观。

   指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>文本颜色</strong></td> 
      <td> <p>选择显示文本的颜色。 有8种颜色可供选择。</p> <p><b>注释</b></p> <p> 如果该字段包含超链接，则文本颜色选择不会应用于该字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文本格式</strong></td> 
      <td>选择以粗体还是斜体显示文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文本对齐</strong></td> 
      <td>选择是将文本与列中的右对齐、居中对齐还是左对齐。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>背景</strong></td> 
      <td>选择文本背景的颜色。 有8种颜色可供选择。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>显示图标</strong></td> 
      <td>如果要显示图标而非此列的实际值，请从16个图标中选择一个。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>显示文本</strong></td> 
      <td> <p>选择此选项以显示此列的自定义标签，而不是其实际值。 指定要显示的文本，而不是提供的字段中的值。</p> <p><b>重要</b></p> <p>选择<strong>显示文本</strong>将禁用内联编辑此列中的文本的功能。<br>此外，无法更改“前置任务”列的值，因为它包含内置逻辑。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>应用于整行</strong></td> 
      <td>选择此选项可将设置应用到整行，而不是仅将设置应用到选定列。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**添加规则**。\
   您可以将其他规则添加到同一列，或将规则添加到其他列。

   规则的应用顺序与创建顺序相同。 它们会合并，但不会相互覆盖，不过同一单元格中的列规则优先于行规则。

   **示例1**

   您可以首先创建一个规则，声明当项目处于“正在生成”状态时，文本颜色为紫色和粗体。 然后，创建第二个规则，规定当任务的“名称”不为空时，文本颜色为红色和斜体，背景颜色为绿色。 在此示例中，会发生以下情况：

   * 项目状态为“正在生成”的任务以紫色和粗体文本显示。 如果任务名称不为空，则任务还具有绿色背景。
   * 其项目状态不是“正在生成”（且“任务名称”不为空）的任务将以绿色背景的红色和斜体文本显示。

   **示例2**

   在项目计划完成日期列中创建一个影响整行的规则，如果项目已取消（例如，项目状态为“废弃”），则变为背景灰色。 然后，创建一个列规则，当项目计划完成日期小于今天（即项目延迟）时，该规则将变为背景红色。 在此示例中，如果取消的项目具有延迟完成日期，则该单元格将显示为红色，即使行中的其他单元格为灰色。 要更正此格式，请执行以下操作：

   * 编辑计划完成日期的格式，并删除延迟项目中红色背景的列规则。
   * 添加与行规则格式相同的列规则（项目状态=无效时为灰色背景）。
   * 再次为延迟项目中的红色背景添加列规则。
   * 保存规则和视图时，红色背景不会应用于已取消的项目。

1. 单击&#x200B;**完成**。
1. 单击&#x200B;**保存+关闭**。\
   在报告中，如果满足指定的条件，用户会看到格式更改。
