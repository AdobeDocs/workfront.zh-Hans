---
title: 使用表单设计器添加显示逻辑和跳过逻辑
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以根据用户在填写自定义表单时所做的选择，决定应显示或跳过自定义表单的哪些部分。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 21b2a8180512f71383a7d5201d62fd9ab166d8ef
workflow-type: tm+mt
source-wordcount: '1366'
ht-degree: 0%

---

# 使用表单设计器添加显示逻辑和跳过逻辑

<span class="preview">本页上的信息介绍了尚未公开发布的功能。 它只能在“预览”环境中用于所有客户，或者在“生产”环境中用于启用快速版本的客户。</span>

<span class="preview">有关快速版本的信息，请参阅 [为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">有关当前版本的信息，请参阅 [2024年第二季度发行版概述](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

您可以根据用户在填写自定义表单时所做的选择，决定应显示或跳过自定义表单的哪些部分。

>[!NOTE]
>
>逻辑仅适用于一个表单，且不能基于从其他表单中选择的内容。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront计划 </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置</td> 
   <td>对自定义表单的管理访问权限 </td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 显示和跳过逻辑图标

自定义表单显示图标以指示将哪个逻辑应用于某些字段。 表单设计器中字段上的图标指示逻辑应用于该字段。

| 图标 | 表单设计器中的字段上的位置 | 定义 |
|--- |--- |--- |
| ![目标字段的显示逻辑](assets/display-logic-bottom-left.png) | 左下 | 该字段是用于显示逻辑的目标字段。 如果对表单进行了特定选择，则会显示此字段。 |
| ![定义显示逻辑图标](assets/display-logic-bottom-right.png) | 右下 | 字段定义显示逻辑。 此字段上的特定选择或值将显示目标字段。 |
| ![目标字段的跳过逻辑](assets/skip-logic-bottom-left.png) | 左下 | 该字段是跳过逻辑的目标字段。 如果对表单进行了特定选择，则表单会跳过此字段并隐藏其中的字段。 |
| ![定义跳过逻辑图标](assets/skip-logic-bottom-right.png) | 右下 | 字段定义跳过逻辑。 此字段上的特定选择或值会跳过其他字段并直接转到目标字段。 |

![逻辑图标](assets/logic-icons-3.png)

选择一个应用了逻辑的字段，以在字段设置中显示现有逻辑规则。

![逻辑规则](assets/form-designer-view-only-logic.png)

## 使用显示逻辑和跳过逻辑的注意事项

* 要在自定义字段、小组件或分区界限中添加显示逻辑，必须在表单上至少一个多选字段（单选按钮、下拉列表或复选框）之前放置。
有关自定义表单中的自定义字段和小部件的信息，请参阅 [使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* 无法将跳过逻辑添加到构件或分区界限中。 您只能将其添加到多选字段（单选按钮、下拉列表或复选框）。
* 如果自定义字段的以下情况全部属实，则您可以将显示逻辑和跳过逻辑添加到自定义字段中：

   * 它是一个多选字段（单选按钮、下拉列表或复选框）
   * 它前面有一个多选字段
   * 后跟另一个自定义字段

* 复制具有显示逻辑或跳过逻辑的表单时，该逻辑将复制到新的自定义表单中。
* 批量编辑对象时，所有自定义字段都会显示在“编辑对象”框中，包括跳过或隐藏的字段。
* 为自定义表单创建显示逻辑规则时，请牢记以下几点：

   * 默认情况下，显示逻辑语句中未包含的自定义字段会显示在自定义表单中。
   * 您可以创建多字段显示逻辑语句。
   * 如果分区界限下的所有字段都应用了显示逻辑，并且它们都因该逻辑而隐藏，则整个分区将在自定义表单上隐藏。

## 向自定义表单添加显示逻辑

显示逻辑定义当用户在多选字段中选择特定值时，要在表单上显示的自定义字段。 该逻辑将添加到目标字段，该字段仅在选择值时显示。

{{step-1-to-setup}}

1. 单击 **自定义Forms**.
1. 创建新的自定义表单或打开现有表单。 请参阅 [使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 以了解详细信息。
1. 根据需要向表单添加字段。 必须在要显示的目标字段之前放置至少一个多选字段（单选按钮、下拉列表或复选框）。
1. 选择目标字段并单击 **添加逻辑** 在屏幕的左下角。
1. 选择 **显示逻辑** 选项卡。
1. 单击 **添加显示规则** 在逻辑生成器中。

   ![显示逻辑生成器](assets/custom-form-logic-builder-display-blank.png)

1. 按照以下生成器中的步骤创建逻辑语句。

   1. 第一个选项是选择定义字段。 这是带有显示目标的选择值的字段。 必须为多选字段。
   1. 第二个选项是选择选择值。 只有已为该字段定义的值可用。
   1. 第三个选项是 **已选择** 或 **未选择**. 选择 **已选择** 表示选择了值时，将显示目标字段。 选择 **未选择** 表示在定义字段中选择任何其他值时，将显示目标字段。
   1. 添加 **和** 规则到逻辑语句，请单击 **添加规则** 直接位于您刚刚创建的规则下。 按照相同的提示构建规则。 必须满足所有和规则才能显示目标字段。

      ![显示逻辑生成器](assets/custom-form-logic-builder-display1.png)

   1. 添加 **或** 规则到逻辑语句，请单击 **添加规则** 在逻辑生成器的底部附近。 然后，单击 **添加规则** 在Or区域内，按照相同的提示构建规则。 满足一个Or规则时，将显示目标字段。

1. 单击 **保存** 完成逻辑语句的生成操作后，发送电子邮件给用户。

   显示逻辑图标将添加到表单设计器的目标字段和定义字段中。

>[!NOTE]
>
><span class="preview">仅当在“预览”环境中的表单设计器中预览表单时，显示逻辑才可用。</span>

## 将跳过逻辑添加到自定义表单

跳过逻辑定义用户在多选字段中选择特定值时跳过的自定义表单字段。 跳过的字段在表单上隐藏。 该逻辑将应用于在其中进行了选择的定义字段，而不是跳过的字段。

{{step-1-to-setup}}

1. 单击 **自定义Forms**.
1. 创建新的自定义表单或打开现有表单。 请参阅 [使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) 以了解详细信息。
1. 根据需要向表单添加字段。 跳过逻辑的定义字段必须是多选字段（单选按钮、下拉列表或复选框）。
1. 选择定义字段并单击 **添加逻辑** 在屏幕的左下角。
1. 选择 **跳过逻辑** 选项卡。
1. 单击 **添加跳过规则** 在逻辑生成器中。

   ![跳过逻辑生成器](assets/custom-form-logic-builder-skip-blank.png)

1. 按照以下生成器中的步骤创建逻辑语句。

   1. 定义字段显示在生成器中。 这是您选择将跳过逻辑应用到的字段。
   1. 第一个选项是选择选择值。 只有已为该字段定义的值可用。
   1. 第二个选项是 **已选择** 或 **未选择**. 选择 **已选择** 表示选择值时，将显示目标字段并跳过两者之间的字段。 选择 **未选择** 表示在定义字段中选择任何其他值时，将显示目标字段并跳过其中的字段。
   1. 第三个选项是目标字段，或跳至的位置。 选择字段名称或 **表单结尾**. 您可能需要先单击“空”一词，然后再选择一个选项。

      ![跳过逻辑生成器](assets/custom-form-logic-builder-skip1.png)

   1. 添加 **或** 规则到逻辑语句，请单击 **添加规则** 在逻辑生成器的底部附近。 然后，根据相同的提示选择相应的选项来构建规则。 当一个 **或** 满足规则时，将显示目标字段。

1. 单击 **保存** 完成逻辑语句的生成操作后，发送电子邮件给用户。

   跳过逻辑图标会添加到表单设计器的目标字段和定义字段中。

>[!NOTE]
>
><span class="preview">只有在“预览”环境中的表单设计器中预览表单时，跳过逻辑才可用。</span>

