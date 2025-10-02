---
product-area: user-management
navigation-topic: configure-your-user-profile
title: 创建自定义分区
description: 默认情况下，您在 [!DNL Workfront] Web应用程序中看到的信息通常显示在左侧面板的部分中。 每个部分包含有关 [!DNL Workfront] 区域或对象的不同信息。
author: Becky
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: ccaf637601c53e5d92dd3357fb07e84b5fd69166
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 1%

---

# 创建自定义分区

## [!DNL Adobe Workfront]节

默认情况下，您在[!DNL Workfront] Web应用程序中看到的信息通常显示在左侧面板部分中。 每个部分包含有关[!DNL Workfront]区域或对象的不同信息。\
有关[!DNL Workfront]的默认区域的详细信息，请参阅文章[关于默认 [!DNL Adobe Workfront] 布局](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)。

除了默认附带[!DNL Workfront]的部分之外，您还可以添加一个仪表板，在其中显示与您的工作流相关的信息。 不能将仪表板添加到所有区域和对象。

下表列出了左侧面板中包含节的所有[!DNL Workfront]区域和对象，以及可以自定义的区域和对象：

| **[!DNL Workfront]区域或对象** | **默认系统节** | **自定义分区** |
|---|---|---|
| [!UICONTROL 项目]区域 | ✓ | ✓ |
| [!UICONTROL 团队] | ✓ |   |
| [!UICONTROL 请求]区域 | ✓ |   |
| [!UICONTROL 时间表]区域 | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL 计划] | ✓ | ✓ |
| [!UICONTROL 项目] | ✓ | ✓ |
| [!UICONTROL 任务] | ✓ |  ✓ |
| [!UICONTROL 问题] |  ✓ |  ✓ |
| [!UICONTROL 用户] |  ✓ |  ✓ |
| [!UICONTROL 文档] |  ✓ |  ✓ |
| [!UICONTROL 资源]区域 | ✓ | ✓ |

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
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL Review]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td>[！UICONTROL Reviewer]或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>查看对对象类型的访问权限</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划或许可证类型，请与[!DNL Workfront]管理员联系。

## 在[!DNL Workfront]对象或区域的左侧面板中添加仪表板

在添加功能板之前，必须构建包含所有要在其上显示信息的功能板。 您还可以构建外部页面。\
有关构建仪表板的更多信息，请参阅文章[创建仪表板](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)。\
有关构建外部页面的更多信息，请参阅文章[在仪表板中嵌入外部网页](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)。

构建功能板或外部页面后，可将其添加到左侧面板。

1. 转到[!DNL Workfront]区域或对象之一，您可以在左侧面板中添加自定义分区。\
   或
1. 转到可在左侧面板中添加[!UICONTROL 仪表板]的对象。\
   有关可添加自定义分区的区域和对象的详细信息，请参阅[[!DNL Adobe Workfront] 分区](#adobe-workfront-sections)。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 添加仪表板]**。
1. 在&#x200B;**[!UICONTROL 快速链接名称]**&#x200B;字段中键入仪表板的名称。 仅对您可见。
1. 在&#x200B;**[!UICONTROL 选择仪表板]**&#x200B;字段中开始键入现有仪表板或外部页面的名称，然后在该仪表板显示在列表中时选择该仪表板。
1. 单击&#x200B;**[!UICONTROL 添加]**。
1. （可选）按希望显示的顺序拖放各个部分。

   顶部是页面的默认部分。

   当您访问相同类型的所有对象时，将为单个对象创建的部分显示，并且仅供您使用。

## 在对象的左侧面板中显示仪表板

有关在对象下添加仪表板的更多信息，请参阅本文中Workfront对象或区域的左侧面板中的[[!UICONTROL 添加仪表板]部分。](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area)

将仪表板添加到对象下的自定义节时，该对象将充当仪表板的筛选器。 例如，如果在功能板上添加任务报告，并将功能板添加到项目中，则包含项目上功能板的自定义部分仅显示您正在查看的项目上的任务。

如果以下对象在层次中高于显示对象，则会针对显示对象的对象过滤这些对象：

* 项目
* 任务
* 问题
* 审批流程
* 注释
* 文档

有关对象的层次结构和相互依赖关系的详细信息，请参阅[了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)一文中的[相互依赖关系和对象层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分。

## 自定义布局模板中的左侧面板

当您向[!DNL Workfront]实例添加仪表板时，它们仅对您可见。

您可以自定义[!DNL Workfront]中的分区，并在布局模板中与多个用户共享新布局。 只有系统或组管理员可以将其与布局模板中的其他用户共享。 有关使用布局模板自定义左侧面板的详细信息，请参阅[使用布局模板自定义左侧面板](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)。
