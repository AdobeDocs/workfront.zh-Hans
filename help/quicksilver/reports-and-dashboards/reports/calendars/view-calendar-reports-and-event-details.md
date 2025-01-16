---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: 查看日历报告和事件详细信息
description: 您可以在Adobe Workfront中查看您创建或与您共享的日历报告和事件详细信息。
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 9ddbe09ab99b6b151fc2d052b4c53e004eb0fa44
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# 查看日历报告和事件详细信息

您可以在Adobe Workfront中查看您创建或与您共享的日历报告和事件详细信息。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新：参与者</p>
       <p>或</p>
       <p>当前：请求</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL View]或更高版本的[！UICONTROL Reports]、[！UICONTROL Dashboards]和[！UICONTROL Calendars]访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>[！UICONTROL视图]或日历报表的更高权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看日历报告

{{step1-to-calendars}}

根据您的访问级别，您可能会看到列出以下日历：

* 您的默认[!DNL Adobe Workfront]日历

  Workfront会根据分配给您或分配给您所分配团队、组或角色的项目、任务和问题为您创建日历。

* 您已创建的日历

  要了解有关创建日历的信息，请参阅[日历报告概述](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)。

* 其他用户与您共享的日历

  要了解如何共享日历，请参阅[[!UICONTROL 共享日历]报告](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)。

1. （视情况而定）单击&#x200B;**[!UICONTROL 查看]**下拉列表，然后选择要查看的日历持续时间。
   ![日历持续时间](assets/view-menu-calendar-report-350x189.png)
您可以从以下日历报表视图中进行选择：

   * **[!UICONTROL 月]**：显示日历的四周
   * **[!UICONTROL 周]**：显示日历的一周
   * **[!UICONTROL 甘特图]**：显示日历的连续视图

     ![[!UICONTROL 甘特图]日历报告](assets/gantt-calendar-report.png)

     通过向下或横向滚动，您可以在[!UICONTROL 甘特图]视图中查看更多事件。 在为视图填充数据时，将显示一个加载符号。

   >[!NOTE]
   >
   >在[!UICONTROL 月]和[!UICONTROL 周]视图中，当前或未来的事件（包括跨越多天的事件，只要它们包含今天或未来的某天即可）具有与项目或日历分组中的颜色对应的阴影。 过去的事件具有更浅的阴影以表示它们不再是最新，但您仍然可以选择和查看这些事件。

1. （可选）如果您在[!UICONTROL 月]或[!UICONTROL 周]查看中查看日历，则可以使用以下选项更改日历视图：

   * 要包含或排除周末，请执行以下操作：

      1. 在&#x200B;**[!UICONTROL 日历]**&#x200B;工具栏上，单击&#x200B;**[!UICONTROL 日历操作]**，然后从下拉列表中选择显示周末&#x200B;**[!UICONTROL 或隐藏周末]**。]****[!UICONTROL 

   * 要快速更改显示的日期，请执行以下操作：

      1. 在&#x200B;**[!UICONTROL 日历]**&#x200B;工具栏上，单击日期指示器的左箭头在日历中向后移动，或者单击右箭头向前移动。

         ![单击箭头以更改日期](assets/click-arrows-to-change-dates-calendar-report.png)\
         显示的日期会根据当前日历视图按间隔进行调整。 例如，如果您在[!UICONTROL 周]视图中查看日历，则根据您选择的箭头，日历显示一周前或一周后。

      1. （可选）要返回到当前日期，请单击&#x200B;[!UICONTROL **今天**]。


1. （可选）要以全屏方式查看日历，请单击&#x200B;**[!UICONTROL 日历]**工具栏右侧的全屏箭头。
   ![单击箭头以更改日期](assets/click-arrows-to-change-dates-calendar-report.png)\
   按Esc返回到日历的正常视图。

1. （可选）要隐藏链接到日历的项目或日历分组事件，请在项目列表中清除该项目或日历分组。
   ![隐藏事件](assets/hide-events-for-project-or-cal-grouping.png)
通过选择项目列表中的[!UICONTROL 项目]或日历分组，可以再次显示事件。

## 查看日历报告事件详细信息

您可以在日历中查看当前和过去事件的详细信息。

1. 转到要了解其详细信息的事件，然后单击该事件。
此时将打开事件的详细信息页面。
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. （可选）要查看有关对象的其他详细信息，请执行以下操作：

   1. 将鼠标悬停在项目、任务或问题名称上。

      将打开对象的详细信息页面。
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. （可选）要打开关联的项目、任务或问题，请单击对象的标题。
   1. （可选）要关闭所有打开的详细信息页面，请单击事件详细信息页面之外的任意位置。
