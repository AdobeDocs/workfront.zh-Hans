---
title: 自定义Forms概述
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以构建自定义表单，以便用户将其附加到Adobe Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: b04ed2e8-c60e-4978-8a9d-b9e087987ef4
source-git-commit: 8e6caabfaa347f0595657078e2d08ce70c0cb697
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 9%

---

# 自定义表单概述

<!--Audited: 12/2023-->

{{highlighted-preview}}

{{form-designer-default}}

您可以构建自定义表单，以便用户将其附加到Adobe Workfront对象。 处理对象的用户可以填写自定义表单以提供有关对象的信息。

例如，您可以附加一个名为“营销内容研究”的自定义表单来附加至项目，以便项目用户能够请求该项目的营销内容：

![](assets/see-image-details-page.png)

## 如何创建自定义表单

表单设计器具有画布样式的工作区，允许您同时查看字段、画布和字段设置。 它还允许您在设计表单时拖放部分中的字段。 您可以调整屏幕右侧的大小，为字段选项提供更多空间。

<span class="preview">使用&#x200B;**布局**&#x200B;按钮（此图像中未显示）可以从两列或三列工作区中进行选择。 按钮指示当前选择的布局。 三列式布局在最右侧的列中显示字段设置。 在双列布局中，字段设置显示在最左列的字段库旁边。</span>

有关详细信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

![示例表单设计器](assets/form-designer-example.png)

## 自定义字段和小部件

Workfront为每种对象类型提供了许多内置字段。

在自定义表单中，您可以创建其他字段来提示用户输入其工作流特有的信息。 这些自定义字段是自定义表单的构建块。

您可以在Workfront中将以下类型的自定义字段添加到自定义表单：

* 单行文本
* 段落文本
* 带格式文本
* 下拉
* 多选下拉框
* 外部查找
* 原生字段
* 键盘缓冲
* 已计算
* 日期字段
* 复选框组
* 单选按钮
* 说明文本
* 分节符
* Adobe XD
* 图像
* PDF
* 视频

>[!NOTE]
>
>要跟踪更新馈送中的字段更改，请转到“设置”>“界面”>“更新馈送”。 有关详细信息，请参阅[配置系统更新](/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md)。

## 用户可以附加自定义表单的对象

构建自定义表单时，您可以将其配置为使用多个对象类型。

用户可以将自定义表单附加到以下对象类型：

* 项目（包括业务案例）
* 任务
* 问题（包括请求队列）
* 公司
* 文档
* 用户
* 项目群
* 项目组合
* 费用
* 组
* 迭代
* 账单记录

有关将自定义表单附加到对象的详细信息，请参阅[将自定义表单添加到对象](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

有关转换对象时自定义表单发生什么情况的信息，请参阅[转换对象时传输自定义表单数据](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/transfer-custom-form-data-larger-item.md)。

