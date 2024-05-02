---
title: 在报表画布中配置条形图可视化
description: 在报表画布中配置条形图可视化
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# 在报表画布中配置条形图可视化

条形图可视化图表可以使用水平条形图突出显示重要信息，从而帮助您快速讲述有关数据的故事。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 配置条形图可视化

>[!NOTE]
>
>当您在报表中构建和编辑块时，会自动保存所有更改。

1. 首先，添加一个可视化图块，其中 **条形图** 报表可视化图表类型，如中所述 [在报表画布中添加或编辑可视化图表块](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. 单击编辑可视化图标 ![](assets/edit-icon.png) 然后执行以下任一操作。

   1. 在 **设置** 选项卡：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">可视化类型</td>
         <td><p>切换到其他可视化类型。 如果这样做，菜单上的后续选项可能会更改。</p></td>
        </tr>
        <tr>
         <td role="rowheader">垂直轴</td>
         <td><p>选择要沿条形图可视化图表的垂直左边缘或Y轴描述的数据。 可视化图表会根据水平轴上的每个项比较此轴上的项。</p></td>
        </tr>
        <tr>
         <td role="rowheader">水平轴</td>
         <td><p>在左侧下拉菜单中，选择要沿水平轴或X轴描述的数据。 此轴上的项目根据其值显示为比较条。</p><p>在右侧下拉菜单中，选择您希望可视化图表如何计算和显示沿水平轴的值：</p>
          <ul>
           <li><p><b>计数</b>：值的数量</p></li>
           <li><p><b>总和</b>：所有值的总计 </p></li>
           <li><p><b>Average</b>：所有值的平均值</p></li>
           <li><p><b>最小值</b>：仅最小值</p></li>
           <li><p><b>最大值</b>：仅最大值</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+添加值</td>
         <td>添加另一个要沿水平轴跟踪的字段。</td>
        </tr>
       </tbody>
      </table>

   1. 在 **数据** 选项卡：

      | 数据源（下拉菜单） | 将可视化图表的数据源更改为报表画布上的另一个表。 |
      |---|---|
      | 显示数据源 | 启用此选项以在报表画布上显示可视化图表的源表，或禁用隐藏该表的选项。 |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. 单击可视化设置菜单之外的任意位置将其关闭。
