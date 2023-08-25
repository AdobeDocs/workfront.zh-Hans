---
title: 在报告画布中配置表列
description: 在报告画布中配置表列
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 2%

---


# 在报告画布中配置表列

表中的列可以配置为显示。 您可以修改列的以下方面：

* 名称
* 排序
* 编辑权限
* 悬停文本
* 聚合
* 条件格式化

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 修改表中的列

1. 转到现有报表，单击 **更多菜单** 图标 ![](assets/more-icon.png) 在报表标题中，然后选择 **编辑**.
1. 在报表的表标题上，单击 **编辑** 图标 ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >如果您刚刚创建了表并且尚未添加任何字段，请改为单击表中心的“编辑”按钮。

1. （可选）在表中添加、重新定位或删除列。 有关编辑表格中的字段的详细信息，请参阅 [在报告画布中添加或编辑表块](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | 添加新列 | 要向表中添加列，请单击并拖动表中的字段。 **字段** 页面右侧的面板放入要放置它的表中，或者双击某个字段以将其添加为最右侧的列。 |
   |---|---|
   | 移动列 | 要重新排列表中各列的顺序，请单击列名称并将其拖动到新位置。 |
   | 删除列 | 要从表中删除列，请单击要删除的列，然后单击列名右侧的x。 |

   {style="table-layout:auto"}

1. 要配置列，请在表的标题行中单击要修改的列的名称，然后单击右面板上的以下选项卡之一：

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">“数据”选项卡</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">聚合依据</td>
      <td><p> 要聚合（在标题中汇总）列中的信息，请从中选择所需的聚合类型 <strong>聚合依据</strong> 下拉菜单。 可用的选项取决于列中包含的数据类型。</p><p>如果在表中使用组，则聚合值将显示在列名上方的组行中，而不是列名旁边。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">字段格式</td>
      <td><p>（仅当列包含日期、百分比、货币或时间数据而非文本时可用。） 选择您想要的数据格式 <b>字段格式</b> 下拉菜单。 例如，您可以在列中的数字后面显示百分比符号，或更改日期的显示方式。</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">字段可编辑</td>
      <td><span>启用 <strong>字段可编辑</strong> 如果您希望允许查看表的用户编辑列的名称。</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>排序</strong></td>
      <td><p>默认情况下，表格会根据其最左列中的数据按升序排序。 要改为按选定列进行排序，请单击旁边的向下箭头 <strong>排序</strong>，然后单击复选框 <b>按此列排序</b>. 然后，您可以选择 <strong>排序</strong> 方向（升序或降序值）和 <strong>排序顺序</strong> （此列与表中其他排序列相比的相对排序优先级）。</p><p>您可以重复此过程，最多按5个不同的列对表进行排序。 确保每列具有正确的内容 <strong>排序顺序</strong> 相对于您选择进行排序的任何新列。</p><p>注：如果删除了选择对表进行排序的列，同时选择了另一列进行排序，则使用该列对表进行降序排序。 如果没有选择其他列进行排序，则表将返回到默认值：按第一列排序。</p><p>当指定列对表进行排序时，在列名旁边会显示一个小框，该框中的数字表示该列在对表进行排序时的相对优先级（表首先按1、2等进行排序），箭头表示排序方向是升序还是降序。 </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">“样式”选项卡</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自定义列标签</strong> </td> 
      <td>输入列的新显示名称（限制为100个字符）。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示悬停文本</td> 
      <td> <p>确定当有人将鼠标悬停在列名称上时是否显示说明性文本。</p> <p>此选项默认处于禁用状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">悬停文本</td> 
      <td>(仅在 <strong>显示悬停文本</strong> 已启用。) 自定义当有人将鼠标悬停在列名称上时显示的说明文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>条件格式化</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>添加 <img src="assets/add-rule.png">，编辑 <img src="assets/edit-icon.png">，或删除 <img src="assets/delete.png"> 当列中的单元格的值符合您指定的条件时，设置这些单元格的格式的规则。</p> <p>例如，您可以创建一个规则，当“项目状态”字段的值等于“正在生成”时，该规则会将该字段中的字体更改为紫色粗体。</p> <p>或者，您可以使用 <b>显示图标</b> 为列中每个具有“当前”状态的项目添加绿色标记图标。</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>注意：如果您使用 <strong>显示图标</strong>中，其他格式选项不可用。</p> <p>您可以选择 <strong>应用于整行</strong> 如果希望格式设置影响满足规则条件的单元格的整行。 例如，您可以通过不仅对“到期时间”列中的日期单元格应用黄色背景色，而且对其包含的整个行应用黄色背景色，来突出显示特定日期后到期的项目。</p> <p>提示：向规则添加格式选项时，生成的单元格格式将显示在 <strong>预览</strong> 位于面板底部。</p> </li> 
        <li value="2">添加完规则后，单击 <strong>保存</strong>.</li> 
        <li value="3"> <p>（可选）单击 <b>+添加规则</b> 将其他规则添加到同一列。</p> <p>表格中的多个条件格式规则按以下顺序应用：</p> 
         <ul> 
          <li> <p>首先评估适用于整个行的规则，针对每列从左到右评估，然后在列中从上到下评估。</p> <p>注意：行格式将覆盖该行中单元格的其他条件格式，即使它们在其他方面满足另一列规则的条件也是如此。</p> </li> 
          <li> <p>随后将从上到下评估其他规则，因为这些规则在列的右侧面板中列出。 您可以拖动 <img src="assets/drag-object-icon.png"> 已保存该面板中的规则以更改其顺序。</p> <p>注意：单元格将根据它们满足的第一个条件进行格式化，即使它们满足其他条件，也不会进一步进行格式化。</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **返回** 屏幕左上角的箭头，可返回至您的报表。
