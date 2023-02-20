---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 跨时区工作
description: 了解如何 [!DNL Adobe Workfront] 使用时区计算以下内容 — 编辑我。
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# 跨时区工作

了解如何 [!DNL Adobe Workfront] 使用时区计算以下内容：

* 对象的时间字段
* 其他时间 [!DNL Workfront] 区域，如自动化的Workfront电子邮件

## 时区 [!DNL Workfront]

您在 [!DNL Workfront] 基于贵组织的时区配置 [!DNL Workfront] 实例和。 如果这两个时区不同，您可能会在中使用的不同区域和功能中看到时间差异 [!DNL Workfront].

>[!NOTE]
>
><div class="preview">在附加到对象的自定义表单中，计算的自定义字段中的日期和时间语句由协调通用时间(UTC)计算和保存，而不是由为组织实例和用户配置文件设置的时区配置来计算和保存。 根据每个用户的各个时区生成并显示自定义表单中的计算。</div>




* [贵组织的 [!DNL Workfront] 实例](#your-organization-s-workfront-instance)
* [您的用户配置文件](#your-user-profile)

### 贵组织的 [!DNL Workfront] 实例 {#your-organization-s-workfront-instance}

贵组织的时区 [!DNL Workfront] 通常为主办公室的位置设置实例。 这可确定以下内容：

* 在由生成的电子邮件中显示的时间 [!DNL Workfront]
* 新添加用户的时区(在 [!DNL Workfront] 管理员根据其工作位置为其配置不同的时区)

   有关这两个示例的更多信息，请参阅 [配置系统的基本信息](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* 项目的已覆盖开单费率的开始或结束。 有关更多信息，请参阅 [在项目层改写职务职责开单费率](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### 您的用户配置文件 {#your-user-profile}

应为用户配置文件中的时区配置您工作的位置。 这可确定以下内容：

* 传出中显示的时间 [!DNL Workfront] 电子邮件
* 处理对象的时间，如开始和结束时间

   如果多个时区的用户被分配给一个对象， [!DNL Workfront] 使用在每个用户配置文件中配置的时区，转换涉及的每个人的对象时间。

   **示例：** 在您工作的东部标准时间(EST)区域中，您将任务设置为在下午4:00开始，并将其分配给在太平洋标准时间(PST)区域工作的用户。 对于这些用户，开始时间显示为下午1:00。 如果它在下午4点显示，他们会在3小时后开始工作。

   如果对象创建者没有注意到被分配人的时区之间的差异，并在设置对象时间时进行必要的调整，或者被分配人没有注意到这种差异，则在每个人协作对象时，很难获得正确的时间。

   **示例：** 您可以将一天的任务配置为在东部标准时间上午9:00开始，但会忘记某些任务用户在PST区域工作。 对他们来说，开始时间是早上6点。 由于他们直到9:00（您的时间中午）才开始处理该任务，因此该任务开始并延迟了3个小时完成。

有关在用户配置文件中配置时区的信息，请参阅 [配置我的设置](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

有关如何 [!DNL Workfront] 管理员(或 [!UICONTROL 编辑] 用户访问权限)可以在用户配置文件中配置时区，请参阅 [编辑用户的配置文件](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## 如何让用户更轻松地跨时区工作

您可以通过多种方式帮助用户更轻松地跨多个时区工作：

* [使用计划](#use-schedules)
* [在自定义表单中使用计算时间字段](#use-calculated-time-fields-in-a-custom-form)
* [在自定义表单中使用文本字段而不是日期字段](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### 使用计划 {#use-schedules}

[!DNL Workfront] 管理员可为组织内的每个时区分别创建单独的计划，以确保无论在何处，都能为每个人适当地安排工作时间。 管理员创建计划后，即可将其与某些项目和用户关联：

* **[!UICONTROL 项目]**:项目创建者可以为单个项目选择计划。 这会根据为受分配者时区设置的工作时间来确定项目中任务的计划。
* **[!UICONTROL 用户]**:A [!DNL Workfront] 管理员(或 [!UICONTROL 编辑] 用户访问权限)可以在用户配置文件中为单个用户选择计划。

   此计划可能与项目计划不同。 例如，当某人在项目中创建了一个任务，但尚未为其分配任何人时，该任务将使用项目计划。 将用户分配到该任务后，该任务将使用该用户的计划。

   如果为任务分配了多个用户，则系统会使用以下任务之一，如系统范围的项目首选项中所配置：

   * 任务主要所有者的计划时区
   * 项目计划的时区。

   这可能会导致任务日期发生更改。

   **示例：** EST用户将被分配到一项为期一天的任务，该任务计划在上午9:00（太平洋标准时间）（即中午12:00）开始。 由于EST用户在一天中只剩下2个工作小时，因此任务完成日期会延长约6小时，直到下一个工作日。

   有关 [!UICONTROL 项目首选项] 面积 [!UICONTROL 设置]，请参阅 [配置系统范围的项目首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   有关将计划分配给项目或用户的说明，请参阅 [创建计划](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   有关计划中配置的时区如何影响 [!UICONTROL 计划小时数] 在 [!DNL Workload Balancer]，请参阅 [在 [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### 在自定义表单中使用计算时间字段 {#use-calculated-time-fields-in-a-custom-form}

您可以在自定义表单中使用一系列计算的自定义字段来显示组织中用户的当前时间，如在多个城市中显示时间的机场时钟行。 您可以为用户工作的每个时区创建一个字段，每个时区都计算其时区的时间。

有关更多信息，请参阅 [将计算数据添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)，以及部分 [日期和时间计算的自定义字段](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) 在文章中 [计算数据表达式](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### 在自定义表单中使用文本字段而不是日期字段 {#use-text-fields-instead-of-date-fields-in-a-custom-form}

如果你不想 [!DNL Workfront] 要为不同时区的用户转换在对象中配置的时间，您可以在自定义表单中使用文本字段（该字段附加到对象，而不是日期字段）。 这样，该时间就会显示您为项目中每个人键入的时间。

如果您这样做，我们建议您提醒表单的用户计算其时区与您时区的时差，以便他们确定工作的开始时间和结束时间。 您可以在为自定义表单键入的说明中，或在该字段的工具提示中包含此内容。 有关更多信息，请参阅 [将自定义字段添加到自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
