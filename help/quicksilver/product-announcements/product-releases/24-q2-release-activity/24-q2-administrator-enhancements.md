---
title: 2024年第二季度管理员增强功能
description: 2024年第二季度管理员增强功能
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '791'
ht-degree: 0%

---

# 2024年第二季度管理员增强功能

本页介绍了在2024年第二季度版本中对“预览”环境做出的所有管理员增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2024年第二季度发布周期中此时可用的所有更改列表，请参阅[ 2024年第二季度发布概述](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md)。

## 显示逻辑和跳过逻辑现在可在表单设计器预览模式下使用

>[!NOTE]
>
>预览版本： 2024年3月28日；适用于所有客户的生产： 24.4（2024年4月11日）

Beta版自定义表单设计器现在允许您在预览模式下测试显示逻辑和跳过逻辑。 以前，即使应用了逻辑，预览中也显示所有字段。

有关在表单设计器中预览自定义表单的详细信息，请参阅[使用表单设计器整理和预览表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。

## 公司和用户现在支持高级自定义表单字段

>[!NOTE]
>
>预览版本： 2024年3月14日；适用于所有客户的生产：24.4（2024年4月11日）

向公司或用户附加自定义表单时，现在可以使用高级自定义表单功能，例如外部查找字段和Workfront本机字段。 高级功能在“公司详细信息”和“用户详细信息”页面上可用，而在“编辑公司”和“编辑用户”对话框中不可用。 必须在新的表单设计器中创建自定义表单，才能利用这些字段类型。

有关自定义表单字段的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## JumpSeat集成现在可用于新包类型

>[!NOTE]
>
>预览版本： 2024年2月26日；用于快速发布的生产版本：使用24.3版本（2024年3月14日）；面向所有客户的生产版本：24.4（2024年4月11日）

现在，使用一种新包类型（即Select、Prime或Ultimate）的帐户可以使用现有的JumpSeat集成。 要启用集成，您必须仍然拥有有效的JumpSeat订阅。

有关JumpSeat集成的详细信息，请参阅[配置JumpSeat集成](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md)。

## 表单设计器测试版中提供了Workfront原生字段

>[!NOTE]
>
>预览版本： 2024年2月29日；用于快速发布的生产版本：使用24.3版本（2024年3月14日）；面向所有客户的生产版本：24.4（2024年4月11日）

Workfront本机字段现在可供您添加到自定义表单中。 利用此新字段类型，可按逻辑方式整理数据并将其呈现给用户，而无需在自定义字段中重新创建现有数据。

在自定义表单字段列表中选择本机字段以将该字段添加到表单设计器后，可以为表单对象选择任何本机字段。 例如，如果表单设计器顶部的“对象类型”列表显示“项目”，则您将能够选择项目的本机字段，但不能选择特定于任务的字段。

将自定义表单附加到对象时，会从对象数据填充字段。 例如，附加到项目的自定义表单上的描述字段将拉入项目描述。 （如果没有可用数据，则字段可能显示“不适用”。）

自定义表单中使用的本机字段在设计器的字段库中可供重复使用。此外，它们还可在设置>自定义Forms >字段区域中可见，以便您查看它们在哪些表单中使用。

此功能仅在表单设计器测试版中可用，在旧版表单生成器中不可用。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

[观看此功能的视频演示。](https://video.tv.adobe.com/v/3427702/){target=_blank}

## 属性映射现在可用于已迁移到Adobe IMS的组织

>[!NOTE]
>
>预览版本： 2024年2月22日；适用于所有客户的生产： 2024年2月22日

Workfront系统管理员现在可以为已迁移到Adobe IMS的组织设置用户属性映射。 这允许用户信息从组织的SSO（单点登录）提供商传递到Workfront，因此用户数据不必同时输入到Workfront和SSO提供商中。

以前，此功能仅适用于尚未载入Adobe IMS的组织。

有关配置属性映射的说明，请参阅&#x200B;**映射用户属性和自动配置新用户**&#x200B;一文中的[映射Adobe统一体验中的用户属性](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience)。

## 跳过逻辑和显示逻辑现在可在表单设计器测试版中使用

>[!NOTE]
>
>预览版本： 2024年2月8日；用于快速发布的生产版本：使用24.2版本（2024年2月15日）；适用于所有客户的生产版本：24.4（2024年4月11日）

现在，您可以在表单设计器测试版中编辑现有显示和跳过逻辑，并向自定义表单添加新逻辑。 易于使用的逻辑生成器可帮助您根据表单中的选择定义要显示或跳过的字段。

表单设计器画布中某个字段上的图标指示已在该字段上配置逻辑，或该字段用于在其他字段上配置的逻辑规则中。

有关详细信息，请参阅[使用表单设计器添加显示逻辑和跳过逻辑](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)。
