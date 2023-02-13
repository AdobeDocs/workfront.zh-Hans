---
product-area: user-management
navigation-topic: configure-your-user-profile
title: 创建自定义部分
description: 您在 [!DNL Workfront] 默认情况下，Web应用程序通常显示在左侧面板的部分中。 每个部分包含有关 [!DNL Workfront] 区域或对象。
author: Lisa
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---

# 创建自定义部分

## [!DNL Adobe Workfront] 章节

您在 [!DNL Workfront] 默认情况下，Web应用程序通常显示在左侧面板部分中。 每个部分包含有关 [!DNL Workfront] 区域或对象。\
有关的默认区域的详细信息 [!DNL Workfront]，请参阅文章 [关于默认 [!DNL Adobe Workfront] 布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

除了附带的 [!DNL Workfront] 默认情况下，您可以添加功能板，在功能板上显示与工作流相关的信息。 不能向所有区域和对象添加功能板。

下表列出了 [!DNL Workfront] 左侧面板中包含部分以及其中哪些部分可以自定义的区域和对象：

| **[!DNL Workfront]区域或对象** | **默认系统部分** | **自定义部分** |
|---|---|---|
| [!UICONTROL 项目] 面积 | ✓ | ✓ |
| [!UICONTROL 团队] | ✓ |   |
| [!UICONTROL 请求] 面积 | ✓ |   |
| [!UICONTROL 工时单] 面积 | ✓ |   |
| [!UICONTROL 项目组合] | ✓ | ✓ |
| [!UICONTROL 项目群] | ✓ | ✓ |
| [!UICONTROL 项目] | ✓ | ✓ |
| [!UICONTROL 任务] | ✓ |  ✓ |
| [!UICONTROL 问题] |  ✓ |  ✓ |
| [!UICONTROL 用户] |  ✓ |  ✓ |
| [!UICONTROL 文档] |  ✓ |  ✓ |

{style=&quot;table-layout:auto&quot;}

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>[!UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td>[!UICONTROL Reviewer]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td>查看对对象类型的访问权限</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 在 [!DNL Workfront] 对象或区域

在添加功能板之前，您必须使用要在功能板上显示的所有信息构建功能板。 您还可以构建外部页面。\
有关构建功能板的更多信息，请参阅文章 [创建功能板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
有关构建外部页面的更多信息，请参阅文章 [在功能板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

构建功能板或外部页面后，可以将其添加到左侧面板。

1. 转到 [!DNL Workfront] 可在左侧面板中添加自定义部分的区域或对象。\
   或
1. 转到可在其中添加 [!UICONTROL 仪表板] 中。\
   有关可向其添加自定义部分的区域和对象的更多信息，请参阅 [[!DNL Adobe Workfront] 章节](#adobe-workfront-sections).
1. 单击 **[!UICONTROL 添加功能板]** 中。
1. 在 **[!UICONTROL 快速链接名称]** 字段。 这仅对您可见。
1. 开始在 **[!UICONTROL 选择功能板]** 字段，然后选择功能板在列表中显示时显示的内容。
1. 单击 **[!UICONTROL 添加]**.
1. （可选）按照要显示部分的顺序拖放这些部分。

   顶部是页面的默认部分。

   当您访问所有具有相同类型的对象时，将显示您为单个对象创建的节，这些节仅供您使用。

## 在对象的左侧面板中显示功能板

有关在对象下添加功能板的更多信息，请参阅部分 [[!UICONTROL 添加功能板] 在Workfront对象或区域的左侧面板中](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) 在本文中。

将功能板添加到对象下的自定义部分时，该对象将充当功能板的过滤器。 例如，如果您在功能板上添加任务报表，然后将功能板添加到项目，则包含项目功能板的自定义部分仅显示您正在查看的项目中的任务。

如果对象的层次结构比对象高，则会为显示对象的对象筛选以下对象：

* 项目
* 任务
* 问题
* 批准流程
* 注释
* 文档

有关对象的层次结构和相互依赖关系的详细信息，请参阅部分 [对象的相互依赖和层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 在布局模板中自定义左侧面板

将功能板添加到 [!DNL Workfront] 实例中，则它们仅对您可见。

您可以在 [!DNL Workfront] 并与布局模板中的多个用户共享新布局。 只有系统或组管理员才能与布局模板中的其他用户共享它们。 有关使用布局模板自定义左侧面板的更多信息，请参阅 [使用布局模板自定义左侧面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
