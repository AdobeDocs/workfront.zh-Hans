---
title: 在报告画布中添加或编辑Web内容块
description: 利用Web内容块，可直接在报表中显示来自外部网站的信息。
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# 在报告画布中添加或编辑Web内容块

利用Web内容块，可直接在报表中显示来自外部网站的信息。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 添加或编辑Web内容块

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击&#x200B;**报表**.
1. 单击 **新报告**.

   或

   转到现有报表，单击 **更多** 图标 ![](assets/more-icon-27x15.png) 在报表标题中，然后单击 **编辑**.

1. 在屏幕右侧的下方 **添加块**，可以：

   拖动 **Web内容** 图标直接放到画布上所需的位置。

   或

   双击 **Web内容** 图标，在画布顶部添加块。

   >[!TIP]
   >
   >可以通过拖动块拐角手柄来更改块放置后的大小。

1. 单击 **无标题Web内容** 在块标题中，然后键入块的标题。
1. 单击 **编辑** 图标 ![](assets/edit-icon.png) 在块标题中。

   ![](assets/web-content-block-header-350x76.png)

1. 在 **设置** 在打开的面板中，输入要显示的页面的完整URL(包括“https://”) **URL** 字段。

   >[!NOTE]
   >
   >目前，只能显示选定域中的站点。 当前可以使用的域包括：
   >   
   >   * workfront.com
   >   * google.com
   >   * sharepoint.com
   >   * attask-ondemand.om
   >   * powerbi.com
   >   * domo.com
   >   * looker.com

   如果输入的URL无法被嵌入，则会在它下面显示警告。 这些警告包括：

   | 警告名称 | 原因 |
   |---|---|
   | 无效 URL | 输入的URL未返回有效的站点。 |
   | 提供程序站点限制 | 不允许您尝试嵌入的网站。 |

   {style="table-layout:auto"}

1. （可选）单击 **传递参数** 切换可打开可用传递参数的列表。

   >[!WARNING]
   >
   >传递参数当前已禁用。

1. 单击 **嵌入URL** 以保存所做的选择并返回到报表。
