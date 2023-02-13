---
title: 在报表画布中配置条形图可视化
description: 在报表画布中配置条形图可视化
author: Nolan
feature: Reports and Dashboards
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 3%

---


# 在报表画布中配置条形图可视化

条形可视化图表通过使用水平条突出显示重要信息，可帮助您快速讲述有关数据的故事。

## 先决条件

在开始之前，您必须注册报表画布测试版。 有关更多信息，请参阅 [报表画布测试版：概述](/help/quicksilver/product-announcements/betas/reporting-canvas-beta/reporting-canvas-beta-overview.md).

## 配置条形图可视化

>[!NOTE]
>
>在您构建和编辑报表中的块时，所有更改都会自动保存。

1. 首先，使用 **条形图** 报表的可视化类型，如 [在报表画布中添加或编辑可视化块](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md).

1. 单击编辑可视化图表图标 ![](assets/edit-icon.png) 在可视化的右上角，执行以下任意操作。

   1. 在 **设置** 选项卡：

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">可视化类型</td>
         <td><p>切换到其他类型的可视化图表。 如果这样做，菜单上的后续选项可能会发生更改。</p></td>
        </tr>
        <tr>
         <td role="rowheader">垂直轴</td>
         <td><p>选择要沿垂直左边或条形可视化的Y轴描述的数据。 可视化图表会根据水平轴上的每个项目比较此轴上的项目。</p></td>
        </tr>
        <tr>
         <td role="rowheader">水平轴</td>
         <td><p>在左侧下拉菜单中，选择要沿水平轴或X轴描述的数据。 此轴上的项目根据其值显示为比较栏。</p><p>在右下拉菜单中，选择您希望可视化图表如何计算和显示沿水平轴的值：</p>
          <ul>
           <li><p><b>计数</b>:值的数量</p></li>
           <li><p><b>总和</b>:所有值的总和 </p></li>
           <li><p><b>平均</b>：所有值的平均值</p></li>
           <li><p><b>最小</b>：仅最低值</p></li>
           <li><p><b>最大值</b>：仅最高值</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+ 添加值</td>
         <td>添加要沿水平轴跟踪的另一个字段。</td>
        </tr>
       </tbody>
      </table>

   1. 在 **数据** 选项卡：

      | 数据源（下拉菜单） | 将可视化的数据源更改为报表画布上的其他表。 |
      |---|---|
      | 显示数据源 | 启用此选项可在报表画布上显示可视化的源表格，或禁用用于隐藏可视化的选项。 |

      {style=&quot;table-layout:auto&quot;}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. 单击可视化设置菜单外的任意位置以将其关闭。
