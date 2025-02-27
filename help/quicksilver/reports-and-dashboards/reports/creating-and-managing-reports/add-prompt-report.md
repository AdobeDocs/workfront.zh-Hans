---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 向报表添加提示
description: 过滤器和提示相似，因为它们都会限制您在报告中显示的信息量。
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 0%

---

# 向报表添加提示

<!-- Audited: 11/2024 -->

## 提示和筛选器之间的区别

过滤器和提示相似，因为它们都会限制您在报告中显示的信息量。

当您希望每次运行报告时，报告中显示的信息都按相同的标准进行过滤时，可以构建过滤器。 过滤器只构建一次，并在报表中进行硬编码。 有关生成筛选器的更多信息，请参阅文章[筛选器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)。

提示是打开的过滤器，每次运行报告时可以通过不同的方式对其进行自定义和应用。

在向报表中添加提示时，可通过在每次运行报表时编辑提示条件来自定义过滤信息。 根据您选择的修饰符，报表每次都使用不同的过滤器运行，而不是在报表的过滤器中对修饰符硬编码一次。

提示对报告起到可自定义过滤器的作用，可在运行报告之前更新。 您可以创建通用报表，然后根据当天要查看的信息或与自己的一组标准相关的信息来缩小结果范围。 例如，如果您有小时报告，并且希望根据以下条件更改报告的信息：

* 记录小时数的日期
* 输入小时数的用户
* 输入的小时数

您将生成三个提示，其中条件为所需条件，并且每次运行报告时，报告都会根据为提示选择的信息而有所不同。

过滤器可以告知Adobe Workfront仅显示今年6月至8月之间输入的小时数。 但是，每次运行报表时，如果提示符，您可以使用不同的时间范围（例如，在一月和二月之间或十月和十二月之间）。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
    <td> 
      <p>新增：</p>
         <ul>
         <li><p>标准</p></li>
         </ul>
      <p>当前：</p>
         <ul>
         <li><p>计划</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限*</td> 
   <td> <p>管理报表的权限</p></td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

必须先创建报告，然后才能向其添加提示。

有关创建报告的说明，请参阅[创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## 创建提示

1. 转到要添加提示的报告。
1. 展开&#x200B;**报表操作**，然后单击&#x200B;**编辑**。

1. 单击&#x200B;**报表设置**&#x200B;按钮。
1. 单击&#x200B;**报告提示**&#x200B;选项卡，然后单击&#x200B;**添加提示**。\
   ![报告提示选项卡](assets/create-report-prompt-tab.png)

1. （视情况而定）选择提示所基于的字段。 开始键入字段的名称，然后单击以在字段出现在列表中时将其选定。\
   运行该报表的用户可用的选项将因您选择的字段而异。\
   例如，如果您在任务报告中选择了一个日期字段，如实际完成日期，则“实际完成日期”是提示的名称。 在运行此报告时编辑此提示时，可以从一组修饰符中进行选择，以生成您的筛选语句。 此过程与构建过滤器相同。 有关修饰符的详细信息，请参阅[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

1. （视情况而定）单击&#x200B;**自定义提示**&#x200B;以创建自定义提示。

   自定义提示是预定义提示，可在运行报表之前对筛选条件进行硬编码。 从这个意义上说，自定义提示比提示更接近于过滤器。

   但是，该提示与常规提示一样灵活，因为您可以从多个预定义语句中进行选择，而不是在报表中仅使用一个硬编码过滤器。

   为自定义提示指定以下信息：自定义提示的条件只能使用文本模式进行编辑。 这允许在单个字段中应用多个条件。

   * **字段名：**&#x200B;这是提示的名称，您在运行报告之前看到它。
   * **下拉项目标签：**&#x200B;这是您在运行报告之前看到的提示中其中一个选项的名称。
   * **条件：**&#x200B;输入定义提示的条件。
   * **默认值：**&#x200B;您可以选择一个项目作为此提示的默认选项。

   使用与输入文本模式过滤器时相同的语法，并通过“&amp;”连接语句。 有关在文本模式下编辑筛选器的详细信息，请参阅[使用文本模式编辑筛选器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md)。

   例如，以下方案的自定义提示的&#x200B;**Condition**&#x200B;字段可能如下所示：

   * 项目状态为“想法”、“已请求”、“已计划”和“当前”的未来项目中的所有任务：

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * 已完成（过去）项目中项目状态为“已完成”或“终止”的所有任务：

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   有关文本模式修饰符的详细信息，请参阅[筛选器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md)。

   >[!NOTE]
   >
   >运行报告时，不能像更改标准提示那样更改自定义提示的条件。 您可以根据需要为自定义提示设置任意数量的预定义条件。

1. （可选）重复步骤4或步骤5，根据需要创建任意数量的提示。
1. 单击&#x200B;**完成**，然后单击&#x200B;**保存+关闭**&#x200B;以保存报告。

## 在报表中应用提示

当您将提示添加到报告时，报告的默认选项卡始终是提示选项卡。

要运行带有提示的报告，请执行以下操作：

1. 转到带有提示的报告。

   ![运行报告提示](assets/run-report-prompts.png)

1. 为&#x200B;**提示**&#x200B;选项卡上显示的一个或多个提示选择条件。\
   （可选）您可以将提示保留为空，而不按提示条件筛选报告。

1. 单击&#x200B;**运行报告**。\
   （视情况而定）如果填充了提示，则报表将按您为提示选择的条件进行筛选。\
   （视情况而定）如果将提示保留为空，则报告不会按提示条件进行过滤。 报告显示为未过滤。

   >[!NOTE]
   >
   >除了提示之外，还包含过滤器的报表会根据过滤器中定义的条件和组合的提示来过滤结果。

## 共享提示报表的限制

>[!CAUTION]
>
>当您共享提示的报告时，已登录和未登录用户使用公共共享链接查看报告时，使用其提示无法运行报告。 在这种情况下，显示报告结果时不会应用任何提示，显示的信息将改为基于用户的访问级别和权限或报告的“以用户身份运行”访问级别和权限（如果已设置）。

以下是从Workfront共享提示报表时的限制：

* 公开共享报告时，用户无法运行带有应用提示的报告，除非他们：拥有Workfront凭据，先登录，然后直接在Workfront中导航到报告（不通过公共共享链接）。

  有关共享报表的更多信息，请参阅文章[在Adobe Workfront中共享报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)。

* 当您计划发送提示报告时，电子邮件附件中的报告会包含未提示的报告数据。 当用户单击电子邮件中的链接以访问报告时，必须首先登录才能查看报告并自行运行提示。

  有关计划传送报表的信息，请参阅[计划自动报表传送](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md)。

* 在运行带有基于日期的提示的报告时，将根据浏览器的时区设置过滤报告结果。 这可能导致在出现提示、表示日期处于月份开始或结束的报表中显示的日期范围略有差异。 如果浏览器的时区设置与特定位置绑定，则该位置本地时间的变化（例如遵循夏令时）也将计入为提示报表显示的日期中。 这可能会导致位于相同时区但位置设置不同的用户之间存在轻微的日期范围差异。
