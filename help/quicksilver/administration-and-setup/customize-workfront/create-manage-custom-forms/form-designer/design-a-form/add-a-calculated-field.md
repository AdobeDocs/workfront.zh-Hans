---
title: 使用表单设计器添加计算字段
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以添加计算自定义字段，在自定义表单附加到对象时，该字段使用现有数据生成新数据。
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---

# 使用表单设计器添加计算字段

您可以添加计算自定义字段，在自定义表单附加到对象时，该字段使用现有数据生成新数据。

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
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 在自定义表单中重用现有的计算自定义字段

您可以在属于不同对象的自定义表单上使用相同的计算自定义字段。 例如，您可以使用为任务自定义表单上的项目自定义表单创建的“利润”计算字段。

使用现有的已计算自定义字段时，计算不会转移到新表单中。 您必须在新自定义表单的同一字段中再次添加计算。

在新表单上，您还可以对同一字段进行不同的计算。 将计算自定义字段的名称保持相同可确保命名惯例的一致性和连贯性。

>[!IMPORTANT]
>
>更改计算表达式可能导致对象上的字段值过时。 要确保始终在这些字段中查看最新计算，请执行以下操作之一：
>
>* 在附加的自定义表单中保存了编辑数据的对象后，单击更多图标 ![](assets/more-icon.png) 在对象的主页上，然后重新计算自定义表达式。
>* 批量编辑对象时，选择重新计算自定义表达式选项。
>* 在自定义表单上编辑已计算的自定义字段时，选择更新以前的计算选项。

要重用现有的计算自定义字段，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 在左侧面板中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 单击 **新建自定义表单。**
1. 选择要将自定义表单附加到的对象类型，然后单击 **继续**.

1. 在屏幕的左上角，单击 **字段库**.

   ![](assets/field-library.png)

1. 使用搜索框或展开 **已计算** 区域以找到所需的计算字段，然后将字段拖动到要在自定义表单中显示的位置。

1. （可选）重复上一步以添加任何其他字段。

   >[!NOTE]
   >
   >您最多可以在单个自定义表单上添加500个字段和小部件。 但是，当表单中存在超过100个时，可能会发生性能下降，具体取决于表单的复杂性。
   >
   >
   >复杂表单的示例包括带有层叠参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

## 添加新计算字段

>[!IMPORTANT]
>
>在创建新的计算自定义字段之前，请确定要包含的现有字段，以便确保在Workfront中存在计算所需的数据。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 在左侧面板中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 单击 **新建自定义表单。**
1. 选择要将自定义表单附加到的对象类型，然后单击 **继续**.

1. 在屏幕左侧，查找 **已计算** 然后将其拖动到画布上的某个部分。

   ![](assets/drag-field-to-section.png)

1. 在屏幕右侧，配置可用于要添加的自定义字段类型的选项：

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
      <li><p>提醒我们这个公式是什么以及它如何运作的。 如果您打算在多个表单上使用此计算自定义字段，这会特别有用。</p> </li> 
      <li> <p>用户将鼠标悬停在该字段上时可以看到工具提示。 您可以在此处添加任何您希望他们在工具提示中看到的文本。</p> <p>如果您不希望他们在工具提示中查看公式（这可能会让他们感到困惑），您可以隐藏该公式。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>您希望存储和显示字段结果的格式。</p> <p>如果该字段将用于数学计算，请始终使用 <strong>数字</strong> 或 <strong>货币</strong> 格式。 选择“数字”或“货币”时，系统会自动截断以0开头的数字。</p> 
      <p><b>重要</b>：在选择格式之前，请考虑新字段的正确格式。 保存自定义表单后，无法编辑格式字段。 此外，选择错误的格式可能会影响报告和列表分组中的未来计算和汇总值。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **计算** 框中，开始生成计算：
   1. 单击 **最大化** 以打开计算编辑器并构建计算。</p>
计算通常以表达式开头，后跟括号，其中包含将自定义表单附加到对象时要引用的字段。

      每个字段都必须用大括号括起来。 当您开始键入字段名称时，系统会提供建议，您可以选择一个来将其插入到计算中。

+++ **展开以查看计算自定义字段中所需的语法**

      每个字段都必须使用下面解释的语法，每个字段名称两侧都应使用大括号。 当您开始键入字段名称时，系统会提供建议，您可以选择一个来将其插入到计算中。 如果在计算中输入的数据不正确，则会出现警告消息，提醒您。 除非编辑计算以包含有效字段和有效计算表达式，否则无法保存表单。

      >[!NOTE]
      >
      >目前，系统仅在您开始键入您希望在自定义表单将附加到的对象上引用的字段名称时提出建议。 不建议使用父对象中的字段。

      **用大括号括住字段名称**

      * 如果您希望计算引用内置字段，则该字段的名称必须用大括号括起来。

        例如： `{actualRevenue}`

        字段名称区分大小写，且必须准确显示在计算中Workfront系统中的显示方式。

        导航至 [Workfront API资源管理器](https://developer.adobe.com/workfront/api-explorer/) 标识可在计算中使用的字段名称。

      * 如果您希望计算引用自定义字段，则该字段的名称必须用大括号括起来，并且前面加上 `DE:` 括弧内。

        例如： `{DE:Profit}`

        系统将列出键入时可以选择的所有自定义字段 `DE:`.

         * 如果您希望计算引用一个字段，该字段将从 *父级* 对象将自定义表单附加到对象时，您必须在字段名称前面加上父对象的对象类型，并且必须用大括号括起来。

        例如，如果自定义表单配置为处理任务，并且您希望字段在表单附加到任务时计算父对象的实际收入，则需要指示 `Project` 作为字段的对象类型：

        `{project}.{actualRevenue}`

        或者，如果是自定义字段：

        `{project}.{DE:profit}`

        **使用句点分隔项目**

        在计算自定义字段中引用相关对象时，必须使用句点分隔对象名称和属性。

        例如，在任务类型自定义表单中，要在计算自定义字段中显示Portfolio所有者的名称，应键入以下内容：

        `{project}.{porfolio}.{owner}`

        这将确定以下内容：从自定义表单（任务）的对象中，您可以访问与任务（项目）相关的下一个对象。 从那里，您可以访问项目（项目组合）的下一个相关对象，然后引用为项目组合对象（所有者）定义的字段

        **用于引用自定义字段的名称语法**

        在计算的自定义字段中引用其他自定义字段时，需要输入该字段在Workfront用户界面中显示的名称。

        例如，要在标记为执行发起人的自定义字段中引用所选选项，应键入以下内容：

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >预输入字段的语法与其他类型的字段的语法略有不同，因为您需要添加 `:name` 在结尾处。
        >
        >例如，要在名为“执行发起人”的自定义预输入字段中引用所选选项，您需要键入：
        >
        >`{DE:Executive sponsor:name}`


        **多对象自定义表单中计算的自定义字段**

        在多对象自定义表单中，所选对象类型必须与表单的计算自定义字段中引用的至少一个字段兼容。 与对象不兼容的字段在表单上显示N/A。

        要确保计算字段显示所有对象类型的正确结果，您必须使用 `$$OBJCODE` 定义每种对象类型的计算。

        >[!INFO]
        >
        >**示例:**
        >
        >在配置为处理项目、任务和问题的自定义表单中，您可以使用以下公式来显示对象类型：
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >在项目上，该字段将显示“这是一个项目”；在任务上，该字段将显示“这是一个任务”；而在问题上，该字段将显示“这是一个问题”。


        >[!INFO]
        >
        >**示例：** 虽然项目中没有“分配至：姓名”字段，但有一个内置的“所有者”字段（该字段会自动填写项目创建者的姓名，除非有人手动更改此名称）。
        >
        >因此，在自定义的“负责人”字段中，您可以使用 `$$OBJCODE` 如下所示，在自定义表单附加到项目时引用“所有者”字段，在表单附加到任务时引用“分配给：名称”字段：
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        有关变量的更多信息，例如 `$$OBJCODE,` 请参阅 [通配符筛选器变量](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **已计算自定义字段的自动更新**

        出现以下情况时，会自动重新计算对象中已计算的自定义字段：

         * 对象上的某些内容发生了变化，例如每日时间线计算。
         * 有人编辑对象上计算自定义字段引用的另一个字段。
         * 计算表达式为空，并且字段包含一个值 — 这会将值设置为null。

           >[!NOTE]
           >
           ><div>在附加到对象的自定义表单中，计算自定义字段中的日期和时间语句通过协调世界时(UTC)进行计算和保存，而不是通过为组织的实例和用户配置文件设置的时区配置进行计算和保存。 自定义表单中的计算根据每个用户的各个时区生成。</div>

+++

   1. 在大文本框中单击，然后单击 **表达式** 和 **字段** 以将其添加到您的计算中。

      您也可以在大文本框中开始键入表达式或字段，然后在显示时将其选定。 每个项目都以“F”（表示字段）或“E”（表示表达式）显示。

      如果键入左圆括号，则会自动添加右圆括号。

+++ **展开以查看有用的提示**
      >[!TIP]
      >
      >您可以执行以下任一操作以获得有关计算的帮助：
      > 
      >* 将鼠标悬停在计算中的表达式上可查看说明、如何使用该表达式的示例以及文章中有关更多信息“了解详情”链接 [计算的数据表达式](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![](assets/hover-expression-help-text.jpg)
      >* 使用颜色编码标识已添加的组件。 表达式以蓝色显示，字段以绿色显示。
      >  ![](assets/colors-fields-expressions.jpg)
      >* 查找以粉红色突出显示的计算错误。 您可以将鼠标悬停在突出显示的错误上以显示其原因的简短描述。
      >  ![](assets/error-help.png)
      >* 在计算下面的区域中，预览现有Workfront对象的结果。
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![](assets/preview-calc.jpg)
      >* 使用左侧显示的行号在长计算中引用表达式。

+++
   1. 单击 **最小化** 在为计算的自定义字段创建计算后。

   1. （可选）使用以下任意选项进一步配置计算的自定义字段：

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">添加逻辑</td> 
      <td>可添加显示逻辑以确定是否根据用户在填写表单时在前面的多选字段（下拉列表、复选框或单选按钮）中所做的选择显示计算字段。 <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>仅当表单上计算的自定义字段前面至少有一个复选框、单选按钮或下拉字段时，此选项才可用。 </p> <p>跳过逻辑不可用于计算的自定义字段。</p> </td> 
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

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.
