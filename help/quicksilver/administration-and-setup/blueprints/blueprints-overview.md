---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprint概述
description: Blueprint是一组Workfront对象，用于处理Workfront中的常见用例。 您可以下载并安装Blueprint，然后根据特定用例配置对象。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: 0da724e975cfb1f0f7e36cffdc545c6223a14a76
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# Blueprint概述

<!--Audited: 01/2024-->

Blueprint是一组Workfront对象，用于处理Workfront中的常见用例。 您可以下载并安装Blueprint，然后根据特定用例配置对象。

![](assets/blueprints-main-page-catalog.png)

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
>   此Blueprint包含用于组织新员工入门培训活动的模板。 使用此模板可让IT团队高效运营，从而带来积极的新员工体验并更快地跟踪工作效率。
>
>* **继承的实例基础知识 | 清单**
>
>    此Blueprint包含一个项目模板（或清单），您可以查看该项目模板（或清单），其中包含一个简短的问题、资源和链接列表，以清楚地了解Workfront实例的配置方式。 当您最近继承了Workfront实例并且需要有关从何处开始的指导时，请使用此项。
>
>若要查看当前Blueprint，请参阅[可用Blueprint的列表](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md)。


Blueprint提供基本的构建块，帮助您创建随增长而增长的工作管理系统。 系统管理员可以浏览Blueprint目录并安装现成的项目模板、功能板和组织结构。 其他用户可以浏览目录并请求安装Blueprint。 有关详细信息，请参阅[浏览Blueprint目录并请求安装Blueprint](../../administration-and-setup/blueprints/browse-catalog.md)。

每个Blueprint都面向一个部门和特定的成熟度级别，以帮助您在系统中更快地实施经验证的最佳实践。 Blueprint目录卡和详细信息中指示了以下详细的成熟度级别。

* **[!UICONTROL 托管]：**&#x200B;托管项目模板可帮助支持在将活动和交付项完全接受为标准流程之前采用新的业务流程。 它们包含确保遵循新流程每个步骤的任务。

* **[!UICONTROL 集成]：**&#x200B;集成项目模板假定业务功能通过标准操作过程受支持。 进程的参与者了解完成进程所需的步骤和任务。 支持此流程的项目模板包含的任务较少，只能跟踪里程碑以及报告所需的其他关键交付项。

## 查找正确的Blueprint

您可以按用例、成熟度级别、安装状态浏览Blueprint，并在目录右侧键入过滤器。 找到您感兴趣的Blueprint后，您可以在详细信息页面上查看详细信息。

### Blueprint 类型

Blueprint类型显示Blueprint中包含的内容。 类型列在目录的Blueprint卡片底部。 请注意，一个Blueprint可以有多个类型。

提供了以下类型的Blueprint：

* **项目模板**：包含与项目模板关联的标准对象（任务、问题、角色和团队），以及与这些对象相关的一些首选项。 有关详细信息，请参阅[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。
* **组织结构**：包括与组织结构（公司、组、角色和团队）关联的对象。 有关详细信息，请参阅[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。
* **仪表板**：包含用于特定用例的一个或多个仪表板，例如实施服务。
<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

若要查看当前Blueprint，请参阅[可用Blueprint的列表](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md)。

### 查看详细信息

每个Blueprint都包含一个“详细信息”页面。 在此页中，您可以：

* 查看工作流内容的摘要
* 阅读Blueprint的简短摘要
* 查看安装历史记录（单击&#x200B;**[!UICONTROL 查看详细信息]**&#x200B;可查看随Blueprint一起安装的对象的完整列表）
* 请参阅角色、团队、公司和组描述
* 查看特定Blueprint的可视化示例，如项目模板（您可以在浏览器中预览或下载完整图像）

![[!UICONTROL Blueprint详细信息]页面](assets/blueprint-details-page-2022.png)

## 安装Blueprint

Workfront管理员可以直接在任何环境（生产、预览或沙盒环境）中安装Blueprint。 要了解更多信息，请参阅[安装Blueprint](../../administration-and-setup/blueprints/blueprints-install.md)或[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。

安装后，您可能不确定接下来要采取什么最佳操作。 有关信息，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。

## 关于Blueprint和模板的其他说明

Blueprint不会替换[!DNL Adobe Workfront]中的项目模板功能。 Blueprint是一种让您能够更快地创建新模板的方法，以在[!DNL Workfront]中组织更多工作。

无法复制或编辑Blueprint。 但是，一旦您从Blueprint安装了解决方案，就可以修改从Blueprint创建的项目模板、工作角色或团队，就像在[!DNL Workfront]界面中更新这些记录一样。 此外，安装Blueprint时，模板存储在[!DNL Workfront]的[!UICONTROL 模板]区域中，而原始Blueprint保留在[!UICONTROL Blueprint]区域中。 在开始根据需要定制模板之前，您不需要制作模板的副本。

Blueprint不会移除或替换环境中配置的任何内容。 如果您打算通过安装可创建新模板的Blueprint来替换现有模板，我们建议您停用以前的版本，以避免从模板构建项目的规划人员混淆。
