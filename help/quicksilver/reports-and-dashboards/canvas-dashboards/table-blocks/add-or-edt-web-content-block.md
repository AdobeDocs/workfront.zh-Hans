---
title: 在报告画布中添加或编辑Web内容块
description: 利用Web内容块，可直接在报表中显示来自外部网站的信息。
hidefromtoc: true
hide: true
exl-id: 29f0c2e1-1644-4989-81b1-c6db6bfec905
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# 在报告画布中添加或编辑Web内容块

利用Web内容块，可直接在报表中显示来自外部网站的信息。

## 先决条件

在开始之前，您必须注册报告画布测试版。 有关详细信息，请参阅[报告画布测试版：概述](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md)。

## 添加或编辑Web内容块

1. 单击Adobe Workfront右上角的&#x200B;**主菜单**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**报表**。
1. 单击&#x200B;**新建报告**。

   或

   转到现有报表，单击报表标题中的&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon-27x15.png)，然后单击&#x200B;**编辑**。

1. 在屏幕右侧的&#x200B;**添加块**&#x200B;下：

   将&#x200B;**Web内容**&#x200B;图标直接拖到画布上所需的位置。

   或

   双击&#x200B;**Web内容**&#x200B;图标以在画布顶部添加块。

   >[!TIP]
   >
   >可以通过拖动块拐角手柄来更改块放置后的大小。

1. 在块标题中单击&#x200B;**无标题的Web内容**，然后键入块的标题。
1. 单击块标题中的&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。

   ![编辑块标题中的图标](assets/web-content-block-header-350x76.png)

1. 在打开的&#x200B;**设置**&#x200B;面板中，输入要在&#x200B;**URL**&#x200B;字段中显示的页面的完整URL(包括“https://”)。

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

1. （可选）单击&#x200B;**传递参数**&#x200B;切换可打开可用传递参数列表。

   >[!WARNING]
   >
   >传递参数当前已禁用。

1. 单击&#x200B;**嵌入URL**&#x200B;以保存您的选择并返回报表。
