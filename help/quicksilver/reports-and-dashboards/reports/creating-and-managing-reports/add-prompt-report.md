---
product-area: reporting
navigation-topic: create-and-manage-reports
title: 向报表添加提示
description: 过滤器和提示在某种意义上是相似的，因为它们都会限制您在报表中显示的信息量。
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# 向报表添加提示

## 提示和过滤器之间的区别

过滤器和提示在某种意义上是相似的，因为它们都会限制您在报表中显示的信息量。

当您希望每次运行报表时报表中显示的信息都按照相同的条件进行过滤时，可以构建过滤器。 过滤器只构建一次，并在报表中进行硬编码。 有关构建过滤器的更多信息，请参阅文章 [过滤器Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

提示是打开的过滤器，每次运行报表时，这些过滤器的自定义和应用方式都会有所不同。

在向报表中添加提示时，您可以通过在每次运行报表时编辑提示条件来自定义过滤信息。 报表每次都会使用不同的过滤器运行，具体取决于您选择的修饰符，而不是在报表的过滤器中对修饰符进行一次硬编码。

提示对报表起可自定义的过滤器作用，您可以在运行报表之前立即更新该过滤器。 您可以创建通用报表，然后根据当天要查看的信息或与您个人的标准集相关的信息来缩小结果范围。 例如，如果您有一个小时报表，并且想要根据以下条件更改报表的信息：

* 记录小时数的日期
* 输入小时的用户
* 输入的小时数

您将生成三个提示，其中条件是所需的条件，并且每次运行报表时，报表的外观都会有所不同，根据您为提示选择的信息。

过滤器可以告知Adobe Workfront仅显示今年6月至8月之间输入的小时数。 但是，在出现提示时，您每次运行报表时（例如，在1月到2月或10月到12月之间）都可以使用不同的时间范围。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>编辑对过滤器、视图、分组的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

必须先创建报表，然后才能向其添加提示。

有关创建报告的说明，请参阅 [创建报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## 创建提示

1. 转到要添加提示的报表。
1. 展开 **报表操作**，然后单击 **编辑**.

1. 单击 **报表设置**.
1. 在 **报表提示** 区域，单击 **添加提示**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. （视情况而定）选择您希望提示所基于的字段。 开始键入字段名称，然后单击以在列表中显示该字段时将其选中。\
   运行报表的用户可用的选项将因您选择的字段而异。\
   例如，如果在任务报表中选择日期字段（如实际完成日期），则“实际完成日期”是提示的名称。 在运行此报表时编辑此提示时，您可以从一组修饰符中进行选择，以构建过滤语句。 此过程与构建过滤器相同。 有关修饰符的详细信息，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. （视情况而定）单击 **自定义提示** 创建自定义提示。

   自定义提示是一个预定义的提示，在运行报表之前，您可在该提示中对筛选条件进行硬编码。 从这个意义上讲，自定义提示比提示更接近过滤器。

   但是，提示与常规提示一样灵活，因为您可以从多个预定义语句中进行选择，而不是在报表中只有一个硬编码过滤器。

   为自定义提示指定以下信息：自定义提示的条件只能使用文本模式进行编辑。 这允许在单个字段中应用多个条件。

   * **字段名称：** 这是运行报表之前看到的提示的名称。
   * **标签：** 这是运行报表之前您在提示中看到的其中一个选项的名称。
   * **条件：** 输入用于定义提示的条件。

   使用输入文本模式过滤器时所使用的语法，并通过“&amp;”连接语句。 有关在文本模式下编辑过滤器的更多信息，请参阅 [使用文本模式编辑过滤器](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   例如， **条件** 以下方案的自定义提示字段可能如下所示：

   * 项目状态为“构思”、“已请求”、“已计划”和“当前”的未来项目上的所有任务：

      ```
      project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
      ```

   * 项目状态为“已完成”或“已终止”的已完成（过去）项目中的所有任务：

      ```
      project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
      ```
   有关文本模式修饰符的详细信息，请参阅 [过滤器和条件修饰符](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >运行报表时，您无法更改自定义提示的条件，如使用标准提示。 自定义提示的预定义条件可以根据需要而定。

1. （可选）重复步骤4或步骤5以根据需要创建任意数量的提示。
1. 单击 **完成**，然后单击 **保存并关闭** 以保存报表。

## 对报表应用提示

在报表中添加提示时，报表的默认选项卡始终为提示选项卡。

要运行带有提示的报表，请执行以下操作：

1. 转到显示提示的报表。

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. 为 **提示** 选项卡。\
   （可选）您可以将提示留空，而不按提示条件过滤报表。

1. 单击&#x200B;**运行报告**。\
   （视情况而定）如果填充了提示，则报表会按照您为提示选择的条件进行过滤。\
   （视情况而定）如果将提示留空，则报表不会按提示条件进行过滤。 报表会像未过滤一样显示。

   >[!NOTE]
   >
   >除了提示之外，还包含过滤器的报表会根据过滤器中定义的条件和组合的提示过滤结果。

## 共享提示报表的限制

>[!CAUTION]
>
>在Workfront外共享提示报表时，查看报表的用户必须登录Workfront才能使用提示运行报表。 如果查看报表的用户未登录，则将显示报表的所有结果，而不应用提示。

以下是共享Workfront中提示的报表时的限制：

* 当您公开共享报表时，用户无法通过应用提示来运行报表，除非他们具有Workfront凭据并首先登录以在Workfront中查看报表。

   有关共享报表的更多信息，请参阅文章 [在Adobe Workfront中共享报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* 计划提示的报表以提交时，电子邮件附件中的报表包含提示的报表数据。 当用户单击电子邮件中的链接以访问报表时，必须先登录才能查看报表并自行运行提示。

   有关计划提交报表的信息，请参阅 [计划自动报表提交](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
