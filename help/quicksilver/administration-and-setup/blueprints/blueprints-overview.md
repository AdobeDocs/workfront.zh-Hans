---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprint概述
description: Blueprint是一组Workfront对象，用于处理Workfront中的常见用例。 您可以下载并安装Blueprint，然后根据特定用例配置对象。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 0%

---

# Blueprint概述

<!--Audited: 01/2024-->

Blueprint是一组Workfront对象，用于处理Workfront中的常见用例。 您可以下载并安装Blueprint，然后针对您的特定用例配置对象。

![Blueprint主页](assets/blueprints-main-page-catalog.png)

>[!INFO]
>
>示例：
>
>* **人力资源组织设置**
>
>   此Blueprint包含要扩展到人力资源部门的组织结构的配置。
>
>* **添加新的员工IT核对清单**
>
>   此Blueprint包含用于组织新员工加入活动的模板。 使用此模板，IT团队可以高效地运营，从而获得良好的新员工体验，并更快地提高生产效率。
>
>* **继承的实例基础知识|清单**
>
>    此蓝图包含一个项目模板（或清单），您可以用简短的问题、资源和链接列表查看这些模板，以清楚地了解您的Workfront实例是如何配置的。 当您最近继承了Workfront实例并需要有关从何处开始的指导时，请使用此项。
>
>要查看当前蓝图，请参阅[可用蓝图列表](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md)。


蓝图提供了基本构建块，以帮助您创建随您的需要而发展的工作管理系统。 系统管理员可以浏览Blueprint目录并安装随时可用的项目模板、功能板和组织结构。 其他用户可以浏览目录并请求安装Blueprint。 有关详细信息，请参阅[浏览Blueprints目录并请求安装Blueprints](../../administration-and-setup/blueprints/browse-catalog.md)。

每个Blueprint都面向一个部门和特定的成熟度级别，以帮助您更快地在系统中实施经验证的最佳做法。 下面详述的成熟度级别会在Blueprint目录卡和详细信息中指明。

* **[!UICONTROL 受管]:**&#x200B;受管项目模板可帮助支持采用新的业务流程，然后再将活动和交付项作为标准流程完全接受。 它们包含确保执行新流程中每个步骤的任务。

* **[!UICONTROL 集成]:**&#x200B;集成项目模板假定通过标准操作过程支持业务函数。 进程的参与者了解完成进程所需的步骤和任务。 支持此流程的项目模板包含的任务较少，只能跟踪里程碑以及报告所需的其他关键交付项。

## 查找正确的Blueprint

您可以按用例、成熟度级别、安装状态浏览Blueprint，并在目录右侧键入过滤器。 找到您感兴趣的Blueprint后，您可以在详细信息页面上查看详细信息。

### Blueprint 类型

Blueprint类型显示Blueprint中包含的内容。 类型列在目录的Blueprint卡片底部。 请注意，一个Blueprint可以有多个类型。

提供了以下类型的Blueprint：

* **项目模板**：包含与项目模板关联的标准对象（任务、问题、角色和团队），以及与这些对象相关的一些首选项。 有关详细信息，请参阅[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。
* **组织结构**：包括与组织结构（公司、组、角色和团队）关联的对象。 有关详细信息，请参阅[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。
* **功能板**：包含一个或多个用于特定用例（如实施服务）的功能板。
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

要查看当前蓝图，请参阅[可用蓝图列表](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md)。

### 查看详情

每个蓝图都包含一个“详细信息”页面。 在此页面中，您可以：

* 查看工作流内容摘要
* 阅读Blueprint的简短摘要
* 查看安装历史记录（单击&#x200B;**[!UICONTROL 查看详细信息]**&#x200B;以查看随Blueprint一起安装的对象的完整列表）
* 请参阅角色、团队、公司和组的描述
* 查看特定Blueprint的可视示例，如项目模板（您可以在浏览器中预览或下载完整图像）

![[!UICONTROL Blueprint详细信息]页面](assets/blueprint-details-page-2022.png)

## 安装Blueprint

Workfront管理员可以直接在任何环境（生产、预览或沙盒环境）中安装Blueprint。 要了解更多信息，请参阅[安装Blueprint](../../administration-and-setup/blueprints/blueprints-install.md)或[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。

安装后，您可能不确定接下来要采取什么最佳操作。 有关信息，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。

## 关于蓝图和模板的其他说明

Blueprints不会替换[!DNL Adobe Workfront]中的项目模板功能。 Blueprints可让您更快地创建新模板以在[!DNL Workfront]中组织更多工作。

您无法复制或编辑Blueprint。 但是，从蓝图安装解决方案后，您可以修改从蓝图创建的项目模板、职务角色或团队，方法与通常在[!DNL Workfront]界面中更新这些记录的方式相同。 此外，安装Blueprint时，该模板存储在[!UICONTROL 的]模板[!DNL Workfront]区域，而原始Blueprint停留在[!UICONTROL Blueprint]区域。 您无需在开始根据需要进行定制之前制作模板的副本。

蓝图不会删除或替换您环境中配置的任何内容。 如果您打算通过安装创建新模板的蓝图来替换现有模板，我们建议您停用以前的版本，以避免从模板构建项目的规划者混淆。
