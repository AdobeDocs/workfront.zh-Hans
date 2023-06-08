---
product-area: reporting
navigation-topic: other-blocks
title: 在报告画布中添加或编辑Web内容块
description: Web内容块允许您直接在报表中显示来自外部网站的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: ca70952bf0acd71f748b042852d434b560727a83
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 1%

---


# 在报告画布中添加或编辑Web内容块

Web内容块允许您直接在报表中显示来自外部网站的信息。

## 先决条件

在开始之前，您必须注册报表画布测试版。 有关更多信息，请参阅 [报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## 添加或编辑Web内容块

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击&#x200B;**报告**.
1. 单击 **新建报告**.

   或

   转到现有报表，单击 **更多** 图标 ![](assets/more-icon-27x15.png) 在报表标题中，然后单击 **编辑**.

1. 在屏幕右侧的下方 **添加块**，可以：

   拖动 **Web内容** 图标直接放到画布上所需的位置。

   或

   双击 **Web内容** 图标，在画布顶部添加块。

   >[!TIP]
   >
   >通过拖动块角控制滑块，可以在放置块后更改块的大小。

1. 单击 **无标题Web内容** 在块标题中，然后键入块的标题。
1. 单击 **编辑** 图标 ![](assets/edit-icon.png) 块标头中的。

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


   如果输入的URL无法被嵌入，则会在其下方显示警告。 这些警告包括：

   | 警告名称 | 原因 |
   |---|---|
   | 无效 URL | 输入的URL未返回有效的站点。 |
   | 提供程序站点限制 | 不允许您尝试嵌入的网站。 |

   {style="table-layout:auto"}

1. （可选）单击 **传递参数** 切换可打开可用传递参数的列表。

   >[!WARNING]
   >
   >传递参数当前被禁用。

1. 单击 **嵌入URL** 以保存所做选择并返回到报表。
