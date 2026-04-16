---
title: 将逻辑规则添加到自定义Forms和字段
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 利用逻辑规则，可进一步自定义表单上的字段。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 49f26e963647f5015955396489bfe537bbac0918
workflow-type: tm+mt
source-wordcount: '3544'
ht-degree: 0%

---

# 向自定义表单和字段添加逻辑规则

利用逻辑规则，可进一步自定义表单上的字段。

例如，您可以根据用户在填写自定义表单时所做的选择，显示或跳过该表单中的字段或章节。

>[!NOTE]
>
>逻辑仅适用于一个表单，且不能基于从其他表单中选择的内容。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td> <p>要应用高级显示、默认值、条件格式或可编辑性逻辑，请执行以下操作：工作流Prime或更高版本</p>
         <p>要应用所有其他逻辑类型：任何Workfront或工作流包</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr>  
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 逻辑指示器图标

自定义表单显示图标以指示何时将逻辑应用于字段。

在表单设计器标题中单击&#x200B;**显示逻辑**&#x200B;可显示或隐藏不同字段逻辑类型的图标。

| 图标 | 定义 |
| --- | --- |
| ![目标字段的显示逻辑](assets/display-logic-bottom-right.png) | 字段是应用显示逻辑的目标字段。 如果对表单进行了特定选择，则会显示此字段。 |
| ![显示引用字段的逻辑图标](assets/display-logic-bottom-left.png) | 该字段是显示逻辑的参考字段。 此字段上的特定选择或值将显示目标字段。 |
| ![跳过目标字段的逻辑](assets/skip-logic-bottom-right.png) | 该字段是应用跳过逻辑的目标字段。 此字段上的特定选择或值会跳过其他字段，并直接转到参考字段。 |
| 引用字段的![跳过逻辑图标](assets/skip-logic-bottom-left.png) | 该字段是跳过逻辑的参考字段。 如果为目标字段进行了特定选择，则表单会跳过此字段并隐藏其中的字段。 |
| ![目标字段的验证逻辑](assets/validation-logic-icon.png) | 字段是应用验证逻辑的目标字段。 参考字段上的特定选择或值确定验证是否失败。 对于验证逻辑，目标字段和参考字段可以相同。 |
| 引用字段的![验证逻辑](assets/validation-logic-reference-field.png) | 该字段是验证逻辑的参考字段。 此字段上的特定选择或值确定验证是否在目标字段上失败。 对于验证逻辑，目标字段和参考字段可以相同。 |
| ![目标字段的默认值逻辑](assets/default-value-logic-icon.png) | 字段是应用默认值逻辑的目标字段。 引用字段上的特定选择或值决定了默认值。 对于默认值逻辑，目标字段和引用字段可以相同。 |
| ![引用字段的默认值逻辑](assets/default-value-logic-reference-field.png) | 该字段是默认值逻辑的参考字段。 此字段上的特定选择或值决定了目标字段上的默认值。 对于默认值逻辑，目标字段和引用字段可以相同。 |
| ![正在格式化目标字段的逻辑](assets/formatting-logic-icon.png) | 字段是应用格式逻辑的目标字段。 引用字段上的特定选择或值决定了格式。 目标字段和引用字段对于格式逻辑可以相同。 |
| ![正在格式化引用字段的逻辑](assets/formatting-logic-reference-field.png) | 字段是格式逻辑的参考字段。 此字段上的特定选择或值决定了目标字段的格式。 目标字段和引用字段对于格式逻辑可以相同。 |
| 目标字段的![可编辑性逻辑](assets/editability-logic-icon.png) | 字段是应用可编辑性逻辑的目标字段。 当满足定义的条件时，该字段可以是可编辑的或只读的。 对于可编辑性逻辑，目标字段和参考字段可以相同。 |
| 引用字段的![可编辑性逻辑](assets/editability-logic-reference-field.png) | 该字段是可编辑性逻辑的参考字段。 当此字段满足定义的条件时，逻辑将应用于目标字段。 对于可编辑性逻辑，目标字段和参考字段可以相同。 |

[逻辑图标](assets/custom-form-logic-icon-samples.png)

对于仅显示和跳过逻辑，请选择一个字段以在字段设置中显示现有逻辑规则。

![逻辑规则](assets/form-designer-view-only-logic.png)

## 使用显示逻辑和跳过逻辑的注意事项

* 要在自定义字段、小组件或分区界限中添加显示逻辑，必须在表单上至少一个多选字段（单选按钮、下拉列表或复选框）之前放置。
有关自定义表单中的自定义字段和小部件的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
* 无法将跳过逻辑添加到构件或分区界限中。 您只能将其添加到多选字段（单选按钮、下拉列表或复选框）。
* 不能应用显示或跳过逻辑来显示或隐藏多选项字段的选择。 例如，不能根据其他字段的显示或跳过逻辑限制为下拉列表、复选框组或单选按钮字段显示的选项。
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

>[!NOTE]
>
>此过程描述显示逻辑的基本模式。 高级显示逻辑也可用。 有关详细信息，请参阅本文中的[将高级显示逻辑添加到自定义表单](#add-advanced-display-logic-to-a-custom-form)。

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。 必须在要显示的目标字段之前放置至少一个多选字段（单选按钮、下拉列表或复选框）。
1. 选择目标字段并单击&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**显示**&#x200B;选项卡。
1. 单击&#x200B;**添加显示规则**。

   ![显示逻辑生成器](assets/simple-display-logic1.png)

1. 执行以下步骤，在生成器中创建逻辑语句。

   1. 第一个选项是选择定义字段。 这是带有显示目标的选择值的字段。 必须为多选字段。
   1. 第二个选项是选择选择值。 只有已为该字段定义的值可用。
   1. 第三个选项是&#x200B;**已选择**&#x200B;或&#x200B;**未选择**。 选择&#x200B;**已选定**&#x200B;表示在选择该值时，将显示目标字段。 选择&#x200B;**未选择**&#x200B;表示在定义字段中选择任何其他值时，将显示目标字段。
   1. 要将&#x200B;**And**&#x200B;规则添加到逻辑语句中，请在刚刚创建的规则下单击&#x200B;**添加规则**。 按照相同的提示构建规则。 必须满足所有和规则才能显示目标字段。

      ![显示逻辑生成器](assets/simple-display-logic2.png)

   1. 要将&#x200B;**Or**&#x200B;规则添加到逻辑语句中，请单击逻辑生成器底部附近的&#x200B;**添加规则**。 然后，单击Or区域中的&#x200B;**添加规则**，并按照相同的提示生成规则。 满足一个Or规则时，将显示目标字段。

1. 完成生成逻辑语句后，单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

## 向自定义表单添加高级显示逻辑

自定义表单字段的高级显示逻辑允许您使用公式构建复杂的逻辑。 您可以将此逻辑应用于以下字段类型：单行文本、段落、带格式的文本、单选下拉列表、多选下拉列表、外部查找、多选外部查找、本机字段引用、预输入、计算、日期、复选框组和单选按钮。

>[!NOTE]
>
>此过程描述显示逻辑的高级模式。 还提供基本显示逻辑。 有关详细信息，请参阅本文中的[将显示逻辑添加到自定义表单](#add-display-logic-to-a-custom-form)。

### 示例

您可以使用高级显示逻辑根据用户角色控制自定义表单部分的可见性，并根据其他字段的状态控制字段的可见性。

表单上的默认部分不应用任何逻辑，因此所有用户始终可见。

如果满足以下条件，则仅当具有资源管理器工作角色的用户查看表单时，才会显示“需要资源”部分。

```IF($$USER.{roleID}="123abc", true)```

请注意，```123abc```表示资源管理器的角色ID。

为角色![显示的](assets/advanced-display-on-form1.png)表单节

具有不同角色ID的相同条件将应用于“项目财务KPI”部分，以定义只有财务顾问角色可以查看该部分。

如果使用以下条件，只有在项目完成后，“销售的KPI”字段才可见。 此逻辑将直接应用于字段，而不是表单分区。 无需指定哪个角色可以查看该字段，因为该角色已在字段所在的部分中定义。

```IF({status}="CPL", true)```

![字段在完整项目中可见](assets/advanced-display-on-form2.png)

### 定义高级显示逻辑

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。
1. 选择要应用逻辑的字段，然后单击&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**显示**&#x200B;选项卡。
1. 打开&#x200B;**高级模式**。

   对于不支持显示逻辑的简单模式的字段类型，此选项可能会自动启用。

   显示逻辑的![高级模式](assets/advanced-display-logic-blank-editor.png)

1. 在编辑器中构建显示条件。

   有关计算和表达式的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)和[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

   >[!NOTE]
   >
   >表单设计器预览模式不支持高级显示逻辑。

## 将跳过逻辑添加到自定义表单

跳过逻辑定义用户在多选字段中选择特定值时跳过的自定义表单字段。 跳过的字段在表单上隐藏。 该逻辑将应用于在其中进行了选择的定义字段，而不是跳过的字段。

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。 跳过逻辑的定义字段必须是多选字段（单选按钮、下拉列表或复选框）。
1. 选择定义字段，然后单击屏幕左下角的&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**跳过**&#x200B;选项卡。
1. 单击&#x200B;**添加跳过规则**。

   ![跳过逻辑生成器](assets/skip-logic1.png)

1. 执行以下步骤，在生成器中创建逻辑语句。

   1. 定义字段显示在生成器中。 这是您选择将跳过逻辑应用到的字段。
   1. 第一个选项是选择选择值。 只有已为该字段定义的值可用。
   1. 第二个选项是&#x200B;**已选择**&#x200B;或&#x200B;**未选择**。 选择&#x200B;**选定**&#x200B;意味着在选择该值时，将显示目标字段并跳过其中的字段。 选择&#x200B;**未选择**&#x200B;表示在定义字段中选择任何其他值时，将显示目标字段并跳过其中的字段。
   1. 第三个选项是目标字段，或跳至的位置。 选择字段名称或&#x200B;**表单**&#x200B;的结尾。 您可能需要先单击“空”一词，然后再选择一个选项。

      ![跳过逻辑生成器](assets/skip-logic2.png)

   1. 要将&#x200B;**Or**&#x200B;规则添加到逻辑语句中，请单击逻辑生成器底部附近的&#x200B;**添加规则**。 然后，根据相同的提示选择相应的选项来构建规则。 当满足一个&#x200B;**或**&#x200B;规则时，将显示目标字段。

1. 完成生成逻辑语句后，单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

## 向自定义表单添加默认值逻辑

默认值逻辑允许您使用公式为自定义表单字段配置默认值。 当满足定义的条件时，将显示默认值。 默认值可以是引用对象内其他字段的静态值或动态值。 尽管默认值可以引用其他字段，但它不会随着表单上的其他字段更改而更改。

您可以将高级默认值逻辑应用于以下字段类型：单行文本、段落、单选下拉列表、多选下拉列表、外部查找、多选外部查找。 本机字段引用、预输入、复选框组和单选按钮。

>[!TIP]
>
>当自定义表单附加到对象时，默认值仅应用于自定义字段一次。 如果默认值公式依赖于另一个字段的值，则在附加自定义表单时，另一个字段中的值必须已存在。

>[!NOTE]
>
>表单设计器中的标准默认值逻辑仍然存在。 如果这两种类型应用于同一字段，则高级逻辑优先。 有关标准默认值逻辑的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkbox-groups-and-drop-downs)中的[添加单选按钮、复选框组和下拉列表](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 示例

使用下面的公式，当项目状态为“计划”时，应用逻辑的多选下拉字段将从项目说明中提取其默认值。

```
IF({status} = 'PLN', ARRAY({description}, ','))
```

当自定义表单附加到项目并且项目状态为“计划”时，项目描述字段值将用作多选字段中的默认值。 由于它是一个多选字段，因此当值与描述匹配时，可以提取多个值。 如果描述值与任何多选值选项都不匹配，则多选字段将不具有默认值，用户可以从下拉列表中选择一个值。

### 定义默认值逻辑

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。
1. 选择要应用逻辑的字段，然后单击&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**默认值**&#x200B;选项卡。

   ![默认值逻辑生成器](assets/default-value-blank-editor.png)

1. 在编辑器中构建默认值条件。

   有关计算和表达式的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)和[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

   >[!NOTE]
   >
   >表单设计器预览模式不支持默认值逻辑。

## 向自定义表单添加验证逻辑

验证逻辑是使用公式构建的，您可以根据需要使逻辑简单或复杂。 验证可以基于其他字段的值或对象的状态，并且您可以在验证失败时提供错误消息。

如果用户填写自定义表单时，如果应用了逻辑的字段满足定义的验证条件，则该字段会高亮显示并显示错误消息。

您可以将验证逻辑应用于以下字段类型：单行文本、段落、单选下拉列表、多选下拉列表、外部查找、多选外部查找、预输入、日期、复选框组和单选按钮。

### 示例

如果满足以下条件，当用户输入触发消息的值时，“预算”字段会在字段下方显示消息。 例如，如果输入的值为负，则显示第一条消息。 如果用户在输入预算值之前尝试将项目状态更改为当前，则会显示第二条消息。

```
IF({DE:Budget Field} < 0,
     "Budget cannot be negative",
     IF({DE:Budget Field} == 0 && {status} == "CUR", "Budget must be specified before moving to Current status")
)
```

另一个简单示例是，电话号码字段必须包含特定的有效位数。

基于其他字段进行验证的另一个示例是会议室大小（小、中或大）字段和会议出席者人数的单独字段。 每个房间大小的人员数会写入验证公式中。 如果用户输入的与会者人数太多，则显示错误消息。

有关验证逻辑的其他示例，请参阅[自定义表单中的高级逻辑示例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/advanced-logic-examples.md)。

### 定义验证逻辑

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。
1. 选择要应用逻辑的字段，然后单击&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**验证**&#x200B;选项卡。

   ![验证逻辑生成器](assets/validation-logic-blank-editor.png)

1. 在编辑器中构建验证条件，包括不符合验证条件时显示的错误消息。

   有关计算和表达式的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)和[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

   >[!NOTE]
   >
   >表单设计器预览模式不支持验证逻辑。

## 向自定义表单添加格式逻辑

格式逻辑在满足定义的条件时突出显示字段值。 应用的格式将同时适用于多个字段。

可以将格式逻辑应用于以下字段类型：单行文本、段落、单选下拉列表、多选下拉列表、外部查找、多选外部查找、预输入、计算、日期、复选框组和单选按钮。

应用于自定义表单的格式与应用于列表和报表的格式不同。 有关报表格式的信息，请参阅[在视图中使用条件格式](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)。

### 示例

如果使用以下条件，当用户输入值1000或更多时，“预算”字段显示为红色。 当用户输入500或更多值时，该字段显示为黄色。

要添加格式的悬停定义，请使用自定义表单中的说明字段。 例如，“预算”字段上的消息可能显示“请输入合理范围内的预算。 值超过500是警告通知，而超过1000则被视为过高。”

```
IF(
     {DE:Budget Field} >=1000,
     FORMAT($$NEGATIVE),
     IF({DE:Budget Field} >= 500, FORMAT($$NOTICE))
)
```

### 定义格式逻辑

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。
1. 选择要应用逻辑的字段，然后单击&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**格式化**&#x200B;选项卡。

   ![正在格式化逻辑生成器](assets/formatting-logic-blank-editor.png)

1. 在编辑器中构建格式条件。

   每个字段最多可以添加5个格式规则。

   突出显示颜色选项的字段包括：

   * `$$POSITIVE (green)`
   * `$$INFORMATIVE (blue)`
   * `$$NEGATIVE (red)`
   * `$$NOTICE (orange)`

   文本格式选项包括：

   * `$$BOLD`
   * `$$ITALIC`
   * `$$UNDERLINE`

   每个函数只能使用一个颜色选项，并且最多只能使用三个其他文本格式选项。 如果未指定颜色选项，则应用系统的默认颜色。

   有关计算和表达式的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)和[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

   >[!NOTE]
   >
   >表单设计器预览模式不支持格式逻辑。

## 向自定义表单添加可编辑性逻辑

可编辑性逻辑确定自定义表单字段是否可以编辑或是否为只读。 此逻辑是使用公式构建的，当字段满足定义的条件时，可以将其设置为可编辑或只读。

您可以将可编辑性逻辑应用于以下字段类型：单行文本、段落、带格式的文本、单选下拉列表、多选下拉列表、外部查找、多选外部查找、预输入、日期、复选框组和单选按钮。

### 示例

使用以下公式，仅当另一个名为Radio的字段选择了Enabled选项时，应用了逻辑的字段才可编辑。

```
IF({DE:Radio} = "Enabled", true)
```

使用以下公式，“说明”字段仅在为空时可编辑。 输入值后，该值将变为只读。

```
IF(ISBLANK({DE:Description}), true)
```

使用以下公式，仅当具有资源管理器工作角色的用户查看表单时，才可编辑应用了逻辑的字段。

```
IF($$USER.{role}.{name}="Resource Manager", true)
```

### 定义可编辑性逻辑

{{step-1-to-setup}}

1. 单击&#x200B;**自定义Forms**。
1. 创建新的自定义表单或打开现有表单。 有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。
1. 根据需要向表单添加字段。
1. 选择要应用逻辑的字段，然后单击&#x200B;**添加逻辑**。
1. 选择逻辑生成器上的&#x200B;**可编辑性**&#x200B;选项卡。

   ![可编辑性逻辑生成器](assets/editability-blank-editor.png)

1. 在编辑器中构建可编辑性条件。

   有关计算和表达式的详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)和[计算数据表达式的概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md)。

1. 单击&#x200B;**应用**。

   应用逻辑，并将逻辑图标添加到表单设计器的目标字段和引用字段中。

   >[!NOTE]
   >
   >表单设计器预览模式不支持可编辑性逻辑。
