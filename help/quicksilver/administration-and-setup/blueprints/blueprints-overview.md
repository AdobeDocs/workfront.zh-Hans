---
user-type: administrator
content-type: overview
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Blueprint概述
description: Blueprint提供基本的构建基块，帮助您创建一个随您一起扩展的工作管理系统。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4c487598-2066-4507-8dfe-1a54d38f5eea
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Blueprint概述

Blueprint提供基本的构建基块，帮助您创建一个随您一起扩展的工作管理系统。 系统管理员可以浏览Blueprint目录并安装现成的项目模板。 其他用户可以浏览目录并请求安装Blueprint。 有关更多信息，请参阅 [浏览蓝图目录并请求安装蓝图](../../administration-and-setup/blueprints/browse-catalog.md).

每个蓝图都针对一个部门和特定的成熟度级别，以帮助您更快地在系统中实施经验证的最佳实践。 下面详述的成熟度级别在Blueprint目录卡和详细信息中指示。

**[!UICONTROL 受管]:** 受管项目模板有助于支持在活动和交付件被完全接受为标准程序之前采用新的业务流程。 它们包含任务，以确保新流程的每个步骤都得到遵循。

**[!UICONTROL 集成]:** 综合项目模板假定业务职能通过标准操作程序得到支持。 该流程的参与者了解完成该流程所需的步骤和任务。 支持此流程的项目模板包含的任务较少，只跟踪里程碑和用于报告目的所必需的其他关键交付项。

## 找到正确的蓝图

您可以按用例、成熟度级别、安装状态浏览Blueprint，并键入目录右侧的过滤器。 找到您感兴趣的蓝图后，即可查看详细信息页面上的详细信息。

### Blueprint 类型

Blueprint类型显示Blueprint中包含的内容。 类型列在目录的Blueprint卡的底部。 请注意，Blueprint可以具有多种类型。

提供了以下类型的蓝图：

* 项目模板：包括与项目模板（任务、问题、角色和团队）关联的标准对象，以及与这些对象相关的某些首选项。 有关更多信息，请参阅 [配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* 组织结构：包括与组织结构（公司、组、角色和团队）关联的对象。 有关更多信息，请参阅 [配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
* 功能板：包括特定用例（如实施服务）的一个或多个功能板。

<!--
* Request queues: Includes one or more projects configured as request queues.
* Custom forms: Includes custom forms attached to another object type, such as a project or portfolio.
* Setup features: Includes one or more elements that are configured in the Setup area of Workfront, such as layout templates.
-->

要查看当前蓝图，请参阅 [可用蓝图列表](/help/quicksilver/administration-and-setup/blueprints/list-of-available-blueprints.md).

### 查看  详细信息

每个Blueprint都包含一个详细信息页面。 在此页面中，您可以：

* 查看工作流内容的摘要
* 阅读Blueprint的简短摘要
* 查看安装历史记录(单击 **[!UICONTROL 请参阅详细信息]** 查看随Blueprint一起安装的对象的完整列表)
* 请参阅角色、团队、公司和群组描述
* 查看特定Blueprint的可视化示例，如项目模板（您可以在浏览器中预览完整图像或下载完整图像）

![[!UICONTROL Blueprint详细信息] 页面](assets/blueprint-details-page-2022.png)

## 安装Blueprint

系统管理员可以直接在生产环境或沙盒环境中安装。 要了解更多信息，请参阅 [安装Blueprint](../../administration-and-setup/blueprints/blueprints-install.md) 或 [配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).

安装后，您可能不确定要采取的最佳后续操作。 有关信息，请参阅 [安装Blueprint后要执行的操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

## 关于蓝图和模板的其他说明

Blueprint不会替换 [!DNL Adobe Workfront]. Blueprint是您更快地创建新模板的一种方式，可以在 [!DNL Workfront].

您无法复制或编辑Blueprint。 但是，从Blueprint安装解决方案后，您可以像在 [!DNL Workfront] 界面。 此外，当您安装Blueprint时，该模板会存储在 [!UICONTROL 模板] 面积 [!DNL Workfront] 原始蓝图就在 [!UICONTROL 蓝图] 的上界。 在开始根据需要定制模板之前，您无需制作模板副本。

Blueprint不会删除或替换环境中配置的任何内容。 如果您打算通过安装用于创建新模板的蓝图来替换现有模板，我们建议您停用以前的版本，以避免使用模板构建项目的规划人员造成混淆。
