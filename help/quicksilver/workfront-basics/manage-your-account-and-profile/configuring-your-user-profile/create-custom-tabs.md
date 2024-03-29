---
product-area: user-management
navigation-topic: configure-your-user-profile
title: 创建自定义分区
description: 您在中看到的信息 [!DNL Workfront] 默认情况下，Web应用程序通常显示在左侧面板的部分中。 每个部分包含有关 [!DNL Workfront] 区域或对象。
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 2%

---

# 创建自定义分区

## [!DNL Adobe Workfront] 区域

您在中看到的信息 [!DNL Workfront] 默认情况下，Web应用程序通常显示在左侧面板部分中。 每个部分包含有关 [!DNL Workfront] 区域或对象。\
有关缺省区域的详细信息 [!DNL Workfront]，请参阅文章 [关于默认值 [!DNL Adobe Workfront] 布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

除了随附的部分 [!DNL Workfront] 默认情况下，您可以添加一个仪表板，以显示与工作流相关的信息。 不能将仪表板添加到所有区域和对象。

下表列出了所有 [!DNL Workfront] 左侧面板中包含部分以及可以自定义的区域和对象：

| **[!DNL Workfront]区域或对象** | **默认系统部分** | **自定义分区** |
|---|---|---|
| [!UICONTROL 项目] 区域 | ✓ “ ”标签 | ✓ |
| [!UICONTROL 团队] | ✓ |   |
| [!UICONTROL 请求] 区域 | ✓ |   |
| [!UICONTROL 时间表] 区域 | ✓ |   |
| [!UICONTROL 项目组合] | ✓ | ✓ |
| [!UICONTROL 项目群] | ✓ | ✓ |
| [!UICONTROL 项目] | ✓ | ✓ |
| [!UICONTROL 任务] | ✓ |  ✓ |
| [!UICONTROL 问题] |  ✓ |  ✓ |
| [!UICONTROL 用户] |  ✓ |  ✓ |
| [!UICONTROL 文档] |  ✓ |  ✓ |

{style="table-layout:auto"}

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td>[！UICONTROL Reviewer]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td>查看对对象类型的访问权限</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您的计划或许可证类型，请联系贵机构的 [!DNL Workfront] 管理员。

## 在的左侧面板中添加仪表板 [!DNL Workfront] 对象或区域

在添加功能板之前，必须构建包含所有要在其上显示信息的功能板。 您还可以构建外部页面。\
有关构建功能板的更多信息，请参阅文章 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
有关构建外部页面的更多信息，请参阅文章 [在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

构建功能板或外部页面后，可将其添加到左侧面板。

1. 转到 [!DNL Workfront] 可在左侧面板中添加自定义分区的区域或对象。\
   或
1. 转到可在其中添加 [!UICONTROL 仪表板] （在左侧面板中）。\
   有关可添加自定义分区的区域和对象的更多信息，请参阅 [[!DNL Adobe Workfront] 区域](#adobe-workfront-sections).
1. 单击 **[!UICONTROL 添加仪表板]** （在左侧面板中）。
1. 在中键入仪表板的名称 **[!UICONTROL 快速链接名称]** 字段。 仅对您可见。
1. 在中开始键入现有仪表板或外部页面的名称 **[!UICONTROL 选择仪表板]** 字段，然后选择在列表中显示的信息板。
1. 单击 **[!UICONTROL 添加]**.
1. （可选）按希望显示的顺序拖放各个部分。

   顶部部分是页面的默认部分。

   为单个对象创建的部分在访问相同类型的所有对象时显示，并且仅供您使用。

## 在对象的左侧面板中显示仪表板

有关在对象下添加功能板的更多信息，请参阅部分 [[!UICONTROL 添加仪表板] 在Workfront对象或区域的左侧面板中](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) 本文章中。

当您将仪表板添加到对象下的自定义节时，该对象将充当仪表板的筛选器。 例如，如果在功能板上添加任务报告，并将功能板添加到项目中，则包含项目上功能板的自定义部分仅显示您正在查看的项目中的任务。

如果显示对象的层次高于显示对象的层次，则会针对该对象筛选以下对象：

* 项目
* 任务
* 问题
* 批准流程
* 注释
* 文档

有关对象的层次和相互依赖关系的详细信息，请参阅一节 [对象的相互依赖性和层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 自定义布局模板中的左侧面板

在将功能板添加到时 [!DNL Workfront] 例如，它们仅对您可见。

您可以自定义以下位置的部分： [!DNL Workfront] 和在一个布局模板中与多个用户共享新布局。 只有系统或组管理员才能与布局模板中的其他用户共享它们。 有关使用版面模板自定义左侧面板的更多信息，请参阅 [使用布局模板自定义左侧面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
