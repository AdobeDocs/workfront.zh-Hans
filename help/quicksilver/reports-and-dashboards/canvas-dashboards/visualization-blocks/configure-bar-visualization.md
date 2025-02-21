---
title: 在报表画布中配置条形图可视化
description: 在报表画布中配置条形图可视化
hidefromtoc: true
hide: true
exl-id: 7dc4f156-d262-482f-aa82-c905f0d1b20f
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 2%

---

# 在报表画布中配置条形图可视化

条形图可视化图表可以使用水平条形图突出显示重要信息，从而帮助您快速讲述有关数据的故事。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关详细信息，请参阅[报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)。

## 配置条形图可视化

>[!NOTE]
>
>当您在报表中构建和编辑块时，会自动保存所有更改。

1. 首先，向报表添加一个可视化块，该可视化块具有&#x200B;**条形图**&#x200B;可视化类型，如[在报表画布](../../../reports-and-dashboards/reporting-canvas/visualization-blocks/add-or-edit-report-visualization.md)中添加或编辑可视化块中所述。

1. 单击可视化右上角的“编辑可视化”图标![编辑图标](assets/edit-icon.png)，然后执行以下任一操作。

   1. 在&#x200B;**设置**&#x200B;选项卡上：

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
           <li><p><b>总和</b>：所有值的总数 </p></li>
           <li><p><b>平均值</b>：所有值的平均值</p></li>
           <li><p><b>最小值</b>：仅最小值</p></li>
           <li><p><b>最大值</b>：仅限最大值</p></li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">+添加值</td>
         <td>添加另一个要沿水平轴跟踪的字段。</td>
        </tr>
       </tbody>
      </table>

   1. 在&#x200B;**数据**&#x200B;选项卡上：

      | 数据源（下拉菜单） | 将可视化图表的数据源更改为报表画布上的另一个表。 |
      |---|---|
      | 显示数据Source | 启用此选项以在报表画布上显示可视化图表的源表，或禁用隐藏该表的选项。 |

      {style="table-layout:auto"}

      <!--   
      NOLAN-FLAG: convert table to html. 
      -->

1. 单击可视化设置菜单之外的任意位置将其关闭。
