---
title: 在报告画布中配置列可视化
description: 在报告画布中配置列可视化
author: Nolan
feature: Reports and Dashboards
exl-id: 5a0cdcd4-b44b-4a63-964e-1c570cd9ff77
hidefromtoc: true
hide: true
source-git-commit: a9c36ff874d3272e1d2de70578c420af29b9d44c
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 1%

---


# 在报告画布中配置列可视化

列可视化图表可以使用垂直列突出显示重要信息，从而帮助您快速讲述有关数据的故事。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 配置列可视化

>[!TIP]
>
>当您在报表中构建和编辑块时，会自动保存所有更改。

1. 首先，添加一个可视化图块，其中 **列** 报表可视化图表类型，如中所述 [在报表画布中添加或编辑可视化图表块](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

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
         <td role="rowheader">水平轴</td>
         <td><p>选择要沿列可视化图表的水平轴或X轴描述的数据。 可视化图表会根据垂直轴上的每个项比较此轴上的项。</p></td>
        </tr>
        <tr>
         <td role="rowheader">垂直轴</td>
         <td><p>在左侧下拉菜单中，选择要沿水平轴或Y轴描述的数据。 该可视化图表根据项目的值将此轴上的项目显示为比较列。</p><p>在右侧的下拉菜单中，选择您希望如何在显示中计算这些值：</p>
          <ul>
           <li><p><b>计数</b>：值的数量</p></li>
           <li><p><b>总和</b>：所有值的总计 </p></li>
           <li><p><b>Average</b>：所有值的平均值</p></li>
           <li><p><b>最小值</b>：仅最小值</p></li>
           <li><p><b>最大值</b>：仅最大值</p></li>
          </ul></td>
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
