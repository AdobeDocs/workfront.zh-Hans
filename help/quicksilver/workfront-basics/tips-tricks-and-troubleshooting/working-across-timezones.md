---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 跨时区工作
description: 了解 [!DNL Adobe Workfront] 如何使用时区计算对象的时间字段和其他区域（如电子邮件）中的时间可能很有帮助。
feature: Get Started with Workfront
author: Becky
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# 跨时区工作

<!-- Audited: 2/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

了解[!DNL Adobe Workfront]如何使用时区计算以下内容会很有用：

* 对象的时间字段
* 其他[!DNL Workfront]区域(如自动发送的Workfront电子邮件)中的时间

>[!WARNING]
>
>如果您在我们提供的列表中找不到确切的时区，请查找最接近您的时区并为您的实例更新该时区。
>
>此外，请考虑一下，类似的时区可能与您的时区不完全相同。
>
>例如，某些国家或地区可能会遵守夏令时，但您的国家可能不会。 如果需要，您可能需要根据这些更改调整系统的时区。


## [!DNL Workfront]中的时区

您在[!DNL Workfront]中看到的时间基于您组织的[!DNL Workfront]实例和用户配置文件的时区配置。 如果这两个时区不同，您可能会在[!DNL Workfront]中使用的不同区域和功能中看到时间差异。

>[!NOTE]
>
>在附加到对象的自定义表单中，计算自定义字段中的日期和时间语句通过协调世界时(UTC)进行计算和保存，而不是通过为组织的实例和用户配置文件设置的时区配置进行计算和保存。 自定义表单中的计算会根据每个用户的各个时区生成和显示。

* [您组织的 [!DNL Workfront] 实例](#your-organization-s-workfront-instance)
* [您的用户配置文件](#your-user-profile)

### 您组织的[!DNL Workfront]实例 {#your-organization-s-workfront-instance}

您组织的[!DNL Workfront]实例的时区通常设置为主办公室的位置。 这会确定以下内容：

* [!DNL Workfront]生成的电子邮件中显示的时间
* 新添加用户的时区（在[!DNL Workfront]管理员根据用户的工作位置为其配置不同时区之前）

  有关这两个示例的详细信息，请参阅[配置系统的基本信息](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)。

* 项目的已覆盖记帐费率的开始或结束。 有关详细信息，请参阅[覆盖项目级别的工作角色记帐费率](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md)。

### 您的用户配置文件 {#your-user-profile}

用户配置文件中的“时区”字段控制发送电子邮件中显示的时间。

时区也会影响PTO日历报表中显示的内容。

有关在用户配置文件中配置时区的信息，请参阅[配置我的设置](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)。

有关[!DNL Workfront]管理员（或具有[!UICONTROL 编辑]用户访问权限的用户）如何在用户配置文件中配置时区的信息，请参阅[编辑用户配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

### 您的浏览器的时区

您应该为工作所在的位置配置浏览器中的时区。 这会确定以下内容：

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* 处理对象的时间，如开始和结束时间。

  如果将处于多个时区的用户分配给某个对象，则[!DNL Workfront]会使用每个用户的浏览器中配置的时区，转换每个相关人员的对象时间。

  **示例**
在您工作的东部标准时间(EST)区域中，您将任务设置为在下午4:00开始，并将其分配给在太平洋标准时间(PST)区域工作的用户。 对于这些用户，开始时间显示为下午1:00。 如果它显示为下午4:00，则他们会延迟三个小时开始处理它。

  如果对象创建者不知道被分配人时区之间的差异，并且在设置对象时间时没有做出必要的调整，或者被分配人不知道该差异，则当每个人协作处理对象时，可能很难获得正确的时间点。

  **示例**

  将一天任务配置为从东部时间上午9:00开始，忘记任务上的一些用户在PST区域中工作。 对于他们，开始时间为上午6:00。 由于他们直到时间9:00（您所在时间的正午）才会开始处理该任务，因此任务会延迟三个小时开始和结束。

不同浏览器的时区配置不同。 有关更多信息，请参阅每个浏览器的文档或帮助信息。

## 如何让用户更轻松地跨时区工作

您可以通过多种方式帮助用户在多个时区中更轻松地工作：

* [使用计划](#use-schedules)
* [在自定义表单中使用计算的时间字段](#use-calculated-time-fields-in-a-custom-form)
* [在自定义表单中使用文本字段而不是日期字段](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 使用计划 {#use-schedules}

[!DNL Workfront]管理员可以为组织内的每个时区创建单独的时间表，以确保为每个人（无论他们身在何处）正确安排工作。 管理员创建计划后，便可将它们与特定项目和用户关联：

* **[!UICONTROL 项目]**：项目创建者可以为单个项目选择计划。 这将根据为被分配人时区设置的工作时间确定项目中任务的计划。
* **[!UICONTROL 用户]**： [!DNL Workfront]管理员（或对用户具有[!UICONTROL 编辑]访问权限的人）可以在用户配置文件中为单个用户选择计划。

  此计划可能与项目计划不同。 例如，当有人在项目中创建任务，但尚未为其分配任何人员时，该任务将使用项目计划。 当用户被分配给任务时，任务使用该用户的计划。

  如果为任务分配了多个用户，则系统将使用下列选项之一，如系统范围或组范围项目首选项中所配置：

   * 任务的主要所有者计划的时区
   * 项目计划的时区。

  如果将一个用户分配给任务，则系统将使用下列选项之一，如系统范围或组范围项目首选项中所配置：

   * 任务被分派人的计划时区
   * 项目计划的时区。

  这可能会导致任务日期发生更改。

>[!BEGINSHADEBOX]

**示例：**
EST用户被分派到计划于PST上午9:00（正午）（EST中午）开始的一天任务。 由于EST用户在一天中只剩下2个工作小时，因此任务完成日期会延长约6小时，直至下一个工作日。


>[!ENDSHADEBOX]

有关[!UICONTROL 安装程序]的[!UICONTROL 项目首选项]区域的信息，请参阅[配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

有关将计划分配给项目或用户的说明，请参阅[创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)。

有关计划中配置的时区如何影响[!UICONTROL 工作负载均衡器]中[!UICONTROL 已计划小时数]分配的信息，请参阅[在[!UICONTROL 工作负载均衡器]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)中管理用户分配。


### 在自定义表单中使用计算的时间字段 {#use-calculated-time-fields-in-a-custom-form}

您可以在自定义表单中使用一系列计算出的自定义字段来显示组织中用户的当前时间，如显示多个城市中的时间的一行机场时钟。 您可以为用户工作的每个时区创建一个字段，每个字段都会计算其时区的时间。

有关详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)，以及文章[计算数据表达式概述](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date)中的[日期和时间计算自定义字段](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)部分。

### 在自定义表单中使用文本字段而不是日期字段 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

如果不希望[!DNL Workfront]转换您为处于不同时区的用户在对象中配置的时间，则可以在附加到对象的自定义表单中使用文本字段，而不是日期字段。 这样，时间就显示了您为项目中的每个人键入的时间。

为此，我们建议您提醒表单用户计算其时区与您的时区之间的差值，以便他们能够确定何时开始和结束工作。 您可以将此字典包含在为自定义表单键入的说明或该字段的工具提示中。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
