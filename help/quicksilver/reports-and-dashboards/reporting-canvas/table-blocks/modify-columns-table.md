---
title: 在报表画布中配置表列
description: 在报表画布中配置表列
author: Nolan
feature: Reports and Dashboards
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 2%

---


# 在报表画布中配置表列

可以配置表格中的列以供显示。 您可以修改列的以下方面：

* 名称
* 排序
* 编辑权限
* 悬停文本
* 聚合
* 条件格式化

## 先决条件

在开始之前，您必须注册报表画布测试版。 有关更多信息，请参阅 [报表画布测试版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 修改表中的列

1. 转到现有报表，单击 **“更多”菜单** 图标 ![](assets/more-icon.png) 在报表标题中，选择 **编辑**.
1. 在报表的表标题上，单击 **编辑** 图标 ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >如果刚刚创建了表，但尚未添加任何字段，请改为单击表中心的“编辑”按钮。

1. （可选）添加、重新定位或删除表中的列。 有关编辑表格中字段的详细信息，请参阅 [在报表画布中添加或编辑表块](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | 添加新列 | 要向表中添加列，请单击并拖动 **字段** 面板，将其放置到要放置的表格上，或双击某个字段以将其添加为最右侧的列。 |
   |---|---|
   | 移动列 | 要重新排列表中列的顺序，请单击列名称，然后将其拖动到新位置。 |
   | 删除列 | 要从表中删除列，请单击要删除的列，然后单击列名称右侧的x。 |

   {style=&quot;table-layout:auto&quot;}

1. 要配置列，请在表的标题行中单击要修改的列的名称，然后在右侧面板中单击以下选项卡之一：

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">“数据”选项卡</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">聚合依据</td>
      <td><p> 要聚合（在标题中汇总）列中的信息，请从 <strong>聚合依据</strong> 下拉菜单。 可用选项取决于列中包含的数据类型。</p><p>如果在表中使用组，则聚合值将显示在列名称上方的组行中，而不是列名称旁边。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">字段格式</td>
      <td><p>（仅当列包含日期、%、货币或时间数据，而不是文本时可用。） 选择您希望对中的数据使用的格式 <b>字段格式</b> 下拉菜单。 例如，您可以在列中的数字后面显示百分比符号，或更改日期的显示方式。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">字段可编辑</td>
      <td><span>启用 <strong>字段可编辑</strong> 如果希望允许查看表的用户编辑列的名称，则。</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>排序</strong></td>
      <td><p>默认情况下，表会根据其最左侧列中的数据以升序排序。 要按所选列排序，请单击旁边的向下箭头 <strong>排序</strong>，然后单击复选框 <b>按此列排序</b>. 然后，您可以选择 <strong>排序</strong> 方向（升序或降序值）和 <strong>排序顺序</strong> （与表中其他排序列相比，此列的相对排序优先级）。</p><p>您可以重复此过程，以按多达5个不同的列对表进行排序。 确保每列均具有正确的 <strong>排序顺序</strong> 相对于您为排序而选择的任何新列。</p><p>注意：如果删除选定对表进行排序的列，并且还选择另一列进行排序，则该列将用于对表进行降序排序。 如果没有选择其他用于排序的列，则表将返回默认值：按其第一列排序。</p><p>指定列对表进行排序时，列名称旁会显示一个小框，其中的数字表示该列在对表进行排序时的相对优先级（表先按1、2等排序），并显示一个箭头以指示排序方向是升序还是降序。 </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">样式选项卡</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自定义列标签</strong> </td> 
      <td>输入列的新显示名称（限制为100个字符）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示悬停文本</td> 
      <td> <p>确定当某人将鼠标悬停在列名称上时，是否显示说明性文本。</p> <p>默认情况下，此选项处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">悬停文本</td> 
      <td>(仅在 <strong>显示悬停文本</strong> 启用。) 自定义当某人将鼠标悬停在列名称上时显示的解释性文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>条件格式化</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>添加 <img src="assets/add-rule.png">，编辑 <img src="assets/edit-icon.png">或删除 <img src="assets/delete.png"> 一个规则，当列中的单元格值符合您指定的条件时，该规则会设置这些单元格的格式。</p> <p>例如，您可以创建一个规则，当“项目状态”字段的值等于“Building”时，该规则会将该字段中的字体更改为粗体紫色。</p> <p>或者，您可以使用 <b>显示图标</b> 向列中每个状态为“当前”的项目添加绿色标记图标。</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>注意：如果您使用 <strong>显示图标</strong>，则其他格式选项将不可用。</p> <p>您可以选择 <strong>应用于整行</strong> 如果您希望格式影响符合规则条件的单元格的整行。 例如，您可以通过将黄色背景颜色应用于“到期日”列中的日期单元格以及发生这些日期的整行来突出显示特定日期之后到期的项目。</p> <p>提示：向规则添加格式选项时，生成的单元格格式将显示在 <strong>预览</strong> 在面板底部。</p> </li> 
        <li value="2">添加完规则后，单击 <strong>保存</strong>.</li> 
        <li value="3"> <p>（可选）单击 <b>+添加规则</b> 向同一列添加其他规则。</p> <p>表中的多个条件格式规则按以下顺序应用：</p> 
         <ul> 
          <li> <p>首先，将评估应用于整个行的规则，从每列的左到右，然后从上到下评估一列的规则。</p> <p>注意：行格式将覆盖该行中单元格的其他条件格式，即使这些格式不符合另一列规则的条件也是如此。</p> </li> 
          <li> <p>随后，将从上到下评估其他规则，因为它们列在列的右侧面板中。 您可以拖动 <img src="assets/drag-object-icon.png"> 面板中保存的规则以更改其顺序。</p> <p>注意：单元格会根据满足的第一个条件进行格式设置，即使单元格满足其他条件，也不会进一步进行格式设置。</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **回去** 箭头返回报表。
