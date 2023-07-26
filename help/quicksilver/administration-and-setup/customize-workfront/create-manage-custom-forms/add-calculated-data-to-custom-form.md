---
title: 使用旧版表单生成器将计算的数据添加到自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 在自定义表单中，您可以构建生成计算的计算自定义字段。 为此，您需要创建一个使用数据表达式和现有字段名称的语句，这些字段可以是自定义字段、计算自定义数据字段和内置Workfront字段。 此语句计算您输入的数据，并在新的计算自定义字段中显示结果。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 9174c4ef-3beb-4d47-9c5c-363f52105a2c
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2573'
ht-degree: 0%

---

# 使用旧版表单生成器将计算的数据添加到自定义表单

在自定义表单中，您可以添加计算自定义字段，该字段在自定义表单附加到对象时使用现有数据生成新数据。

计算自定义字段可以包含：

* 对单个内置字段的简单引用。

  >[!INFO]
  >
  > **示例：** 要计算项目和任务产生的收入，您可以创建一个包含内置字段实际收入的计算自定义字段。 当有人将自定义表单附加到项目或任务时，项目或任务的收入显示在字段中。

* 引用一个或多个字段的表达式。 这些可以是自定义字段、其他计算的自定义字段和内置字段。

  >[!INFO]
  >
  >**示例：** 要计算项目和任务生成的利润，您可以创建一个名为“利润”的计算自定义字段，该字段包含一个从收入中减去成本的数学表达式。
  >
  >为此，您可以使用数学表达式SUB（减）以及内置的Workfront字段Actual Cost和Actual Revenue。
  >
  >在以下步骤中，您可以看到如何执行此示例。

有关为贵组织创建自定义表单以及了解可与其关联的字段类型的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td>计划</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 将计算字段添加到自定义表单 {#add-a-calculated-field-to-a-custom-form}

您可以使用内置的Workfront字段和已创建的自定义字段。

>[!IMPORTANT]
>
>在创建新的计算自定义字段之前，请确定要包含的现有字段，以便确保在Workfront中存在计算所需的数据。

1. 开始创建或编辑自定义表单，如中所述 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. 在 **添加字段** 选项卡，单击 **已计算**.

   在右侧的显示区域中，将显示字段 *12345*. 这只是个指示器，提醒您在创建或编辑自定义表单时该字段是已计算的自定义字段。 当表单附加到对象并且用户填写时，他们会在字段中看到计算结果，而不是 *12345* 指示器。

1. 为计算字段指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td>为字段键入标签。 这是用户使用自定义表单时将看到的内容。 字段 <b>名称</b>，将自动填充，Workfront将在报表中引用它。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">说明</td> 
      <td> 默认情况下，您为该字段创建的公式存储在此处。 您可以添加文本以提供有关字段及其公式的附加信息。 这可以通过两种方式派上用场： 
       <ul> 
        <li> <p>提醒我们这个公式是什么以及它如何运作的。 如果您打算在多个表单上使用此计算自定义字段，这会特别有用。</p> </li> 
        <li> <p>用户将鼠标悬停在该字段上时可以看到工具提示。 您可以在此处添加任何您希望他们在工具提示中看到的文本。</p> <p>如果您不希望他们在工具提示中查看公式（这可能会让他们感到困惑），您可以隐藏该公式。 有关说明，请参阅一节中的表行“在说明中显示公式” <a href="#build-the-calculation-for-your-calculated-custom-field" class="MCXref xref">为计算的自定义字段构建计算</a> 本文章中。</p> </li> 
       </ul> <p>有关在新表单上使用相同的计算自定义字段的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md#using-an-existing-calculated-custom-field-on-a-new-form" class="MCXref xref">在自定义表单中重用现有的计算自定义字段</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>您希望存储并显示字段结果的格式。</p> <p>如果该字段将用于数学计算，请始终使用 <strong>数字</strong> 或 <strong>货币</strong> 格式。 选择“数字”或“货币”时，系统会自动截断以0开头的数字。</p> 
      <p><b>重要</b>：在选择格式之前，请考虑新字段的正确格式。 保存自定义表单后，无法编辑格式字段。 此外，选择错误的格式可能会影响报告和列表分组中的未来计算和汇总值。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 继续到 [为计算的自定义字段构建计算](#build-the-calculation-for-your-calculated-custom-field) 本文章中。

## 为计算的自定义字段构建计算 {#build-the-calculation-for-your-calculated-custom-field}

1. 开始创建计算自定义字段，如一节中所述 [将计算字段添加到自定义表单](#add-a-calculated-field-to-a-custom-form) 本文章中。

1. 单击 **最大化** 以打开 **计算编辑器** 并构建您的计算。

   >[!INFO]
   >
   >**示例：** 使用本文简介中的示例，您可以在自定义表单中为项目和任务创建名为Profit的计算自定义字段。 此字段可以包含显示实际收入与实际成本之间差异的计算：
   >
   >`SUB({actualRevenue},{actualCost})`
   >
   >在此示例中， `SUB` 是表达式，引用的字段为 `actualRevenue` 和 `actualCost`.

   计算通常以表达式开头，后跟括号，其中包含将自定义表单附加到对象时要引用的字段。 有关可用表达式的信息，请参见 [计算的数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

   每个字段都必须用大括号括起来，如一节中所述 [已计算的自定义字段中所需的语法](#syntax-required-in-calculated-custom-fields) 本文章中。 当您开始键入字段名称时，系统会提供建议，您可以选择一个来将其插入到计算中。

   您可以在计算中引用任何类型的自定义字段，但以下两种类型除外：具有格式设置的文本字段和描述性文本。 有关自定义字段类型的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)

1. 在大文本框中单击，然后单击 **表达式** 和 **字段** 以将其添加到您的计算中。

   您也可以在大文本框中开始键入表达式或字段，然后在显示时将其选定。 每个项目都以“F”（表示字段）或“E”（表示表达式）显示。

   如果键入左圆括号，则会自动添加右圆括号。

   >[!TIP]
   >
   >您可以执行以下任一操作以获得有关计算的帮助：
   > 
   >* 将鼠标悬停在计算中的表达式上可查看说明、如何使用该表达式的示例以及文章中有关更多信息“了解详情”链接 [计算的数据表达式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
   >  ![](assets/hover-expression-help-text.jpg)
   >* 使用颜色编码标识已添加的组件。 表达式以蓝色显示，字段以绿色显示。
   >  ![](assets/colors-fields-expressions.jpg)
   >* 查找以粉红色突出显示的计算错误。 您可以将鼠标悬停在突出显示的错误上以显示其原因的简短描述。
   >  ![](assets/error-help.png)
   >* 在计算下面的区域中，预览现有Workfront对象的结果。
   ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
   >  ![](assets/preview-calc.jpg)
   >* 使用左侧显示的行号在长计算中引用表达式。

1. 单击 **最小化** 在为计算的自定义字段创建计算后。

   >[!NOTE]
   >
   >在右侧的显示区域中，将显示字段 *12345。* 这只是个指示器，提醒您在创建或编辑自定义表单时该字段是已计算的自定义字段。 当表单附加到对象并且用户填写时，他们会在字段中看到计算结果，而不是 *12345* 指示器。

1. （可选）使用以下任意选项进一步配置计算的自定义字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">添加逻辑</td> 
      <td>可添加显示逻辑以确定是否根据用户在填写表单时在前面的多选字段（下拉列表、复选框或单选按钮）中所做的选择显示计算字段。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">向自定义表单添加显示逻辑和跳过逻辑</a>. <p>仅当表单上计算的自定义字段前面至少有一个复选框、单选按钮或下拉字段时，此选项才可用。 </p> <p>跳过逻辑不可用于计算的自定义字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新以前的计算</td> 
      <td>编辑现有的计算自定义字段时，可选择此选项，以在保存自定义表单时触发计算中的更新。 在保存自定义表单时，此操作只发生一次。 执行此操作后，选项会返回到其禁用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在说明中显示公式</td> 
      <td>如果您希望填写自定义表单的用户在将鼠标悬停在该字段上时能够查看该字段的公式，请保持启用此选项。 有关详细信息，请参阅有关 <a href="#instructions" class="MCXref xref">说明</a> 在此表格前面部分。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **完成** 完成对计算自定义字段的所有更改后。

   或者，单击 **应用** ，以应用您到目前为止对表单所做的更改，以便继续将自定义字段添加到表单。

   或者，单击 **保存+关闭** 在自定义表单上完成所有更改后。
1. 要验证计算的自定义字段是否正常工作，请将自定义表单附加到对象，然后查看计算自定义字段中的结果。

   有关附加自定义表单的说明，请参阅 [向对象添加自定义表单](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   如果要继续以其他方式构建自定义表单，可以继续阅读以下文章之一：

   * [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 已计算的自定义字段中所需的语法

每个字段都必须使用下面解释的语法，每个字段名称两侧都应使用大括号。 当您开始键入字段名称时，系统会提供建议，您可以选择一个来将其插入到计算中。 如果在计算中输入的数据不正确，则会出现警告消息，提醒您。 除非编辑计算以包含有效字段和有效计算表达式，否则无法保存表单。

>[!NOTE]
>
>目前，系统仅在您开始键入您希望在自定义表单将附加到的对象上引用的字段名称时才提出建议，而不是在对象的父级上提出建议。

### 用大括号括住字段名称

* 如果您希望计算引用内置字段，则该字段的名称必须用大括号括起来。

例如： `{actualRevenue}`

字段名称区分大小写，且必须准确显示在计算中Workfront系统中的显示方式。

* 如果您希望计算引用自定义字段，则该字段的名称必须用大括号括起来，并且前面加上 `DE:` 括弧内。

例如： `{DE:Profit}`

系统将列出键入时可以选择的所有自定义字段 `DE:`.

* 如果您希望计算引用一个字段，该字段将从 *父级* 对象将自定义表单附加到对象时，您必须在字段名称前面加上父对象的对象类型，并且必须用大括号括起来。

  例如，如果自定义表单配置为处理任务，并且您希望字段在表单附加到任务时计算父对象的实际收入，则需要指示 `Project` 作为字段的对象类型：

  `{project}.{actualRevenue}`

  或者，如果是自定义字段：

  `{project}.{DE:profit}`

  如果由于针对多个对象类型配置了的自定义，因此您不确定父对象的对象类型是什么，则可以使用通配符筛选器变量 `$$OBJCODE` 允许计算适用于每种可能的类型。 有关更多信息，请参阅 [多对象自定义表单中计算的自定义字段](#calculated-custom-fields-in-multi-object-custom-forms) 本文章中。

### 使用句点分隔项目

在计算自定义字段中引用相关对象时，必须使用句点分隔对象名称和属性。

例如，在任务类型自定义表单中，要在计算自定义字段中显示Portfolio所有者的名称，应键入以下内容：

`{project}.{porfolio}.{owner}`

这将确定以下内容：从自定义表单（任务）的对象中，您可以访问与任务（项目）相关的下一个对象。 从那里，您可以访问与项目相关的下一个对象（项目组合），然后访问与项目组合（所有者）相关的下一个对象。

### 用于引用自定义字段的名称语法

在计算的自定义字段中引用其他自定义字段时，您需要输入该字段的名称，该名称会显示在Workfront用户界面中。

例如，要在标记为执行发起人的自定义字段中引用所选选项，应键入以下内容：

`{DE:Executive sponsor}`

>[!NOTE]
>
>预输入字段的语法与其他类型的字段的语法略有不同，因为您需要添加 `:name` 在结尾处。
>
>例如，要在名为“执行发起人”的自定义预输入字段中引用所选选项，您需要键入：
>
>`{DE:Executive sponsor:name}`


## 多对象自定义表单中计算的自定义字段 {#calculated-custom-fields-in-multi-object-custom-forms}

在多对象自定义表单中，所选对象类型必须与表单的计算自定义字段中引用的所有字段兼容。 如果存在不兼容的情况，则会显示一条消息，提醒您进行调整。

>[!INFO]
>
>**示例:**
>
>在配置为与Task对象类型一起使用的自定义表单中，您将创建一个名为“负责”的计算自定义字段。 您可以将其配置为引用内置字段，以便在将表单附加到任务时，显示负责的主要被分配人的姓名：
>
>`{assignedTo}.{name}`
>
>稍后，将Project对象类型添加到自定义表单。 出现一条警告消息，指明Project对象类型与计算的自定义字段不兼容。

发生这种情况时，您可以执行以下操作之一：

* 从自定义表单中删除两个不兼容的项目之一 — 对象类型或引用的计算自定义字段。
* 保留这两个项目并使用通配符筛选器变量 `$$OBJCODE` 作为IF表达式中的条件，以创建两个不同版本的In Charge字段。 这允许字段成功运行，无论表单附加到哪种类型的对象。

>[!INFO]
>
>**示例：** 虽然项目中没有“分配至：姓名”字段，但有一个内置的“所有者”字段（该字段会自动填写项目创建者的姓名，除非有人手动更改此名称）。
>
>因此，在自定义的“负责人”字段中，您可以使用 `$$OBJCODE` 如下所示，在自定义表单附加到项目时引用“所有者”字段，在表单附加到任务时引用“分配给：名称”字段：
>
>`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

有关变量的更多信息，例如 `$$OBJCODE,` 请参阅 [通配符筛选器变量](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## 已计算自定义字段的自动更新

出现以下情况时，会自动重新计算对象中已计算的自定义字段：

* 对象上的某些内容发生了变化，例如每日时间线计算。
* 有人编辑对象上计算自定义字段引用的另一个字段。
* 计算表达式为空，并且字段包含一个值 — 这会将值设置为null。

  >[!NOTE]
  >
  ><div>在附加到对象的自定义表单中，计算自定义字段中的日期和时间语句通过协调世界时(UTC)进行计算和保存，而不是通过为组织的实例和用户配置文件设置的时区配置进行计算和保存。 自定义表单中的计算根据每个用户的各个时区生成。</div>
