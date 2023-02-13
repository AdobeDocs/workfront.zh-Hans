---
title: 自定义表单增强功能
description: 在22.2版本中，为管理自定义表单做出了以下重要改进。
author: Luke
exl-id: 81568eab-8a65-4767-b8ab-fb9353a90bb6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# 自定义表单增强功能

在22.2版本中，为管理自定义表单做出了以下重要改进。

## 添加资产小组件

您可以在自定义表单中嵌入图像。 这样，您就可以以更加交互和直观的方式与自定义表单用户通信。 即将推出其他小组件类型。

![](assets/image-in-custom-form.png)

将包含小组件的自定义表单附加到对象后，使用该对象的用户可以在以下区域看到该对象：

* 对象的“详细信息”区域(例如，对于项目，“项目详细信息”区域&#x200B;)

   ![](assets/see-image-details-page.png)

* 对象的“编辑”框(如果具有新的Adobe Workfront体验外观)（例如，“编辑项目”和“编辑任务”框）&#x200B;

   ![](assets/image-see-in-edit.png)

目前，用户在以下区域中看不到小组件&#x200B;:

* 列表和报表
* 主页和摘要
* 对象的“编辑”框(如果它没有新的Adobe Workfront体验外观)（例如，“编辑费用”框）
* &#x200B;Workfront移动应用程序

有关将小组件添加到自定义表单的更多信息，请参阅 [在自定义表单中添加或编辑图像或其他资产小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## 将自定义表单与多个对象类型关联

您可以将多个对象类型与任何新的自定义表单相关联：

![](assets/new-custom-form-object-types.png)

或任何现有的自定义表单：

![](assets/add-object-type-existing-form.png)

这允许您创建单个自定义表单，以用于项目、任务、问题以及自定义表单支持的任何其他类型的对象。

在转换问题或任务时，这特别有用，因为您可以将自定义表单及其数据传递到已转换的对象。 您不再需要为各种对象类型创建和维护同一自定义表单的确切副本，请手动将自定义表单添加到项目中。

>[!INFO]
>
>**示例:**
>
>某人提交了内部IT请求（问题），并提供了附加的自定义表单中所需内容的详细信息。
>
>您可以将问题转换为项目，以供将处理该问题的用户使用。
>
>由于包含提交者详细信息的自定义表单与问题和项目对象类型都相关联，因此自定义表单和所有这些详细信息将在转换期间传递到项目。

>[!NOTE]
>
>进行转换时，自定义表单必须已与您要转换为的对象类型关联。

有关将资产小组件添加到自定义表单的说明，请参阅 [在自定义表单中添加或编辑图像或其他资产小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

创建或编辑多对象自定义表单时，请考虑以下事项：

* [节中断的权限选项](#permission-options-for-section-breaks)
* [计算的自定义字段兼容性](#calculated-custom-field-compatibility)
* [请注意从自定义表单中删除对象类型](#caution-about-deleting-an-object-type-from-a-custom-form)

### 节中断的权限选项

可用于“问题”、“任务”、“项目”和“用户”对象类型的节中断权限选项集比所有其他对象类型的权限选项集具有更多权限选项：有限编辑。

![](assets/section-break-permissions-limited-edit.png)

可用于所有其他对象类型(Portfolio、文档、程序、费用、公司、小版本、帐单记录和组)的节中断权限集不包括“有限编辑”：

![](assets/section-break-permissions-no-limited-edit.png)

在与这两个组中的对象类型关联的自定义表单中，系统使用一组适用于所有对象类型的通用节中断权限。 特别是，此常用集不使用“有限编辑”权限选项，而是用“有限编辑”权限选项的“编辑”权限选项替换。 “编辑”选项与所有对象类型兼容。

如果关联的对象类型使用的权限选项不同于自定义表单上已有的其他对象类型，则会显示一条消息，允许您切换到表单的通用权限选项集。 此更改将应用于所有字段，即使这些字段不在分段下也是如此。

有关更多信息，请参阅 [向自定义表单中添加节分符](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

### 计算的自定义字段兼容性

在多对象自定义表单中，如果计算字段引用了可用于表单所有关联对象类型（如{name}、{description}和{entryDate}，它们可用于多个对象类型）的字段，则无论您将其附加到哪个对象，数据都会正确计算。

例如，如果您有一个针对项目和问题的多对象表单，并且您添加了一个包含{name}表达式的计算字段，则在将表单添加到项目时，该字段会显示项目名称，以及将表单添加到任务的任务名称。

但是，如果表单中的计算字段引用的字段与表单的所有对象类型不兼容，则会有消息提醒您进行调整。

>[!INFO]
>
>**示例：** 在与任务对象类型关联的自定义表单中，您可以创建一个计算的自定义字段，该字段引用了“已分配给”的内置字段：名称，以便在表单附加到任务时显示主要负责人的名称：
>
>
```
>Assigned To: Name{assignedTo}.{name}
>```
>
>稍后，您将Project对象类型添加到自定义表单中。 出现警告消息，告知您Project对象类型与计算的自定义字段不兼容。 这是因为“分配给”字段不适用于项目。

发生此情况时，您可以执行以下操作之一：

* 从自定义表单中删除两个不兼容的项目之一 — 对象类型或引用的字段。
* 保留两个项目并使用通配符过滤器变量 `$$OBJCODE` 作为IF表达式中的一个条件，以创建“主管”字段的两个不同版本。 这样，无论表单附加到哪种类型的对象，字段都可以成功运行。

   使用上面的示例，但没有内置的“分配给”：项目的“名称”字段中有一个内置的“所有者”字段（除非有人手动更改此字段，否则该字段会自动填写创建项目的人员的姓名）。 因此，在您的自定义“主管”字段中，您可以使用 `$$OBJCODE` 如下所示，在将自定义表单附加到项目时引用“所有者”字段，并且指定给：表单附加到任务时的“名称”字段：

   ```
   IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})
   ```

>[!NOTE]
>
>  如果在字段名称前添加对象类型，则该对象类型会引用该对象的父对象，因此您不能使用 `{project}.{name}` ，但您可以将其与任务结合使用。

有关向自定义表单添加计算自定义字段的说明，请参阅 [将计算数据添加到自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

有关变量(如 `$$OBJCODE`，请参阅 [通配符过滤器变量](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

### 请注意从自定义表单中删除对象类型

您可以随时删除自定义表单上的对象类型，但应谨慎执行此操作。 如果用户已将自定义表单附加到要删除的类型对象，并将数据添加到该对象，则当您在表单上删除该对象类型时，该数据将被永久删除。

此外，没有通知系统可提醒使用自定义表单的用户该表单已被删除。

有关更多信息，请参阅 [从系统中删除自定义字段或小组件](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
