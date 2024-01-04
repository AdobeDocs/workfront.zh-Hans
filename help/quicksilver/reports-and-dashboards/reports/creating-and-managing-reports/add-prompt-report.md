---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 向报表添加提示
description: 过滤器和提示相似，因为它们都会限制您在报告中显示的信息量。
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1251'
ht-degree: 0%

---

# 向报表添加提示

## 提示和筛选器之间的区别

过滤器和提示相似，因为它们都会限制您在报告中显示的信息量。

当您希望每次运行报告时，报告中显示的信息都按相同的标准进行过滤时，可以构建过滤器。 过滤器只构建一次，并在报表中进行硬编码。 有关构建过滤器的更多信息，请参阅文章 [过滤器概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

提示是打开的过滤器，每次运行报告时可以通过不同的方式对其进行自定义和应用。

在向报表中添加提示时，可通过在每次运行报表时编辑提示条件来自定义过滤信息。 根据您选择的修饰符，报表每次都使用不同的过滤器运行，而不是在报表的过滤器中对修饰符硬编码一次。

提示对报告起到可自定义过滤器的作用，可在运行报告之前更新。 您可以创建通用报表，然后根据当天要查看的信息或与自己的一组标准相关的信息来缩小结果范围。 例如，如果您有小时报告，并且希望根据以下条件更改报告的信息：

* 记录小时数的日期
* 输入小时数的用户
* 输入的小时数

您将生成三个提示，其中条件为所需条件，并且每次运行报告时，报告都会根据为提示选择的信息而有所不同。

过滤器可以告知Adobe Workfront仅显示今年6月至8月之间输入的小时数。 但是，每次运行报表时，如果提示符，您可以使用不同的时间范围（例如，在一月和二月之间或十月和十二月之间）。

## 访问要求

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
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>编辑对筛选器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建报告，然后才能向其添加提示。

有关创建报告的说明，请参阅 [创建报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## 创建提示

1. 转到要添加提示的报告。
1. 展开 **报表操作**，然后单击 **编辑**.

1. 单击 **报表设置**.
1. 在 **报告提示** 区域，单击 **添加提示**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. （视情况而定）选择提示所基于的字段。 开始键入字段的名称，并在该字段出现在列表中时单击以将其选定。\
   运行该报表的用户可用的选项将因您选择的字段而异。\
   例如，如果您在任务报告中选择了一个日期字段，如实际完成日期，则“实际完成日期”是提示的名称。 在运行此报告时编辑此提示时，可以从一组修饰符中进行选择，以生成您的筛选语句。 此过程与构建过滤器相同。 有关修饰符的详细信息，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （视情况而定）单击 **自定义提示** 创建自定义提示。

   自定义提示是预定义提示，可在运行报表之前对筛选条件进行硬编码。 从这个意义上说，自定义提示比提示更接近于过滤器。

   但是，该提示与常规提示一样灵活，因为您可以从多个预定义语句中进行选择，而不是在报表中仅使用一个硬编码过滤器。

   为自定义提示指定以下信息：自定义提示的条件只能使用文本模式进行编辑。 这允许在单个字段中应用多个条件。

   * **字段名称：** 这是提示的名称，您在运行报告之前看到它。
   * **标签：** 在运行报告之前，您会看到该提示中的一个选项，这是该选项的名称。
   * **条件：** 输入定义提示的条件。

   使用与输入文本模式过滤器时相同的语法，并通过“&amp;”连接语句。 有关在文本模式下编辑过滤器的更多信息，请参阅 [使用文本模式编辑筛选器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   例如， **条件** 的自定义提示字段，适用于以下场景：

   * 项目状态为“想法”、“已请求”、“已计划”和“当前”的未来项目中的所有任务：

     ```
     project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
     ```

   * 已完成（过去）项目中项目状态为“已完成”或“终止”的所有任务：

     ```
     project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
     ```

   有关文本模式修饰符的详细信息，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >运行报告时，不能像更改标准提示那样更改自定义提示的条件。 您可以根据需要为自定义提示设置任意数量的预定义条件。

1. （可选）重复步骤4或步骤5，根据需要创建任意数量的提示。
1. 单击 **完成**，然后单击 **保存+关闭** 以保存报表。

## 在报表中应用提示

当您将提示添加到报告时，报告的默认选项卡始终是提示选项卡。

要运行带有提示的报告，请执行以下操作：

1. 转到带有提示的报告。

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. 为显示在“ ”上的一个或多个提示选择条件 **提示** 选项卡。\
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
>当您在Workfront之外共享提示的报告时，查看报告的用户必须登录到Workfront，才能使用提示运行报告。 如果查看报告的用户未登录，则报告的所有结果将显示而不应用提示。

以下是从Workfront共享提示报表时的限制：

* 在公开共享报告时，用户无法通过应用提示来运行报告，除非他们具有Workfront凭据并先登录以在Workfront中查看报告。

  有关共享报表的更多信息，请参阅文章 [在Adobe Workfront中共享报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* 当您计划发送提示报告时，电子邮件附件中的报告包含提示报告的数据。 当用户单击电子邮件中的链接以访问报告时，必须首先登录才能查看报告并自行运行提示。

  有关计划传送报表的信息，请参阅 [计划自动报表提交](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
