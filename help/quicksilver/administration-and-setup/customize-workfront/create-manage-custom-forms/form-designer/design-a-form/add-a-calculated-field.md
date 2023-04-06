---
title: 使用表单设计器添加计算字段
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以添加一个计算量度的自定义字段，当自定义表单附加到对象时，该字段会使用现有数据来生成新数据。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---


# 使用表单设计器添加计算字段

您可以添加一个计算量度的自定义字段，当自定义表单附加到对象时，该字段会使用现有数据来生成新数据。

计算的自定义字段可以包含：

* 对单个内置字段的简单引用。

   >[!INFO]
   >
   > **示例：** 要计算由项目和任务生成的收入，您可以创建一个包含内置字段“实际收入”的计算自定义字段。 当某人将自定义表单附加到项目或任务时，该项目或任务的收入将显示在字段中。

* 引用一个或多个字段的表达式。 这些字段可以是自定义字段、其他计算的自定义字段和内置字段。

   >[!INFO]
   >
   >**示例：** 要计算项目和任务产生的利润，您可以创建一个名为“利润”的计算自定义字段，其中包含从收入中减去成本的数学表达式。
   >
   >为此，您可以将数学表达式SUB（减）与内置的Workfront字段“实际成本”和“实际收入”一起使用。
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
   <td>任意</td> 
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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的Workfront管理员。

## 在自定义表单中重复使用现有的计算自定义字段

您可以对属于不同对象的自定义表单使用相同的计算量度自定义字段。 例如，您可以在任务自定义表单上使用为项目自定义表单创建的“利润”计算字段。

使用现有的计算自定义字段时，计算不会转移到新表单。 您必须在同一字段的新自定义表单上再次添加计算。

您还可以对新表单上的同一字段进行不同的计算。 为计算的自定义字段保留相同的名称可确保命名约定的一致性和一致性。

>[!IMPORTANT]
>
>更改计算表达式可能会导致对象上的字段值过期。 要确保始终查看这些字段中的最新计算，请执行以下操作之一：
>
>* 在保存您以附加的自定义表单编辑数据的对象后，单击更多图标 ![](assets/more-icon.png) 在对象的主页上，重新计算自定义表达式。
>* 批量编辑对象时，选择“重新计算自定义表达式”选项。
>* 在自定义表单上编辑计算自定义字段时，选择更新以前的计算选项。


要重复使用现有计算的自定义字段，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 单击 **新的自定义表单。**
1. 选择要将自定义表单附加到的对象类型，然后单击 **继续**.

1. 在屏幕的左上角，单击 **字段库**.

   ![](assets/field-library.png)

1. 使用搜索框或展开 **已计算** 部分找到所需的计算字段，然后将其拖动到您希望在自定义表单中显示的位置。

1. （可选）重复上一步以添加任何其他字段。

   >[!NOTE]
   >
   >您最多可以在一个自定义表单上添加500个字段和小组件。 但是，如果表单上存在超过100个，则性能可能会降低，具体取决于表单的复杂性。
   >
   >
   >复杂表单的示例包括具有级联参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 要保存更改，请单击 **应用** 然后转到其他部分以继续构建表单。

   或

   单击 **保存并关闭**.

## 添加新的计算字段

>[!IMPORTANT]
>
>在创建新的计算自定义字段之前，请确定要包含的现有字段，以确保计算所需的数据存在于Workfront中。

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** 中。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 单击 **新的自定义表单。**
1. 选择要将自定义表单附加到的对象类型，然后单击 **继续**.

1. 在屏幕左侧，找到 **已计算** 并将其拖动到画布上的某个部分。

   ![](assets/drag-field-to-section.png)

1. 在屏幕右侧，配置可用于您添加的自定义字段类型的选项：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td>键入字段的标签。 这是用户在使用自定义表单时将看到的内容。 字段 <b>名称</b>,Workfront会在报表中引用自动填充的。</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">说明</td> 
      <td> 默认情况下，您为字段创建的公式会存储在此处。 您可以添加文本，以提供有关字段及其公式的其他信息。 这在以下两种方面非常有用： 
       <ul> 
      <li><p>提醒我们这个公式是什么，它是如何运作的。 如果您计划在多个表单上使用此计算量度的自定义字段，此功能会特别有用。</p> </li> 
      <li> <p>当用户将鼠标悬停在字段上时，可以看到工具提示。 您可以在此处添加希望在工具提示中看到的任何文本。</p> <p>如果您不希望他们在工具提示中看到公式（可能会令他们感到困惑），可以将其隐藏。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>您希望存储和显示字段结果的格式。</p> <p>如果在数学计算中将使用字段，请始终使用 <strong>数值</strong> 或 <strong>货币</strong> 格式。 选择“数字”或“货币”时，系统会自动截断以0开头的数字。</p> 
      <p><b>重要信息</b>:在选择格式之前，请考虑新字段的正确格式。 保存自定义表单后，无法编辑格式字段。 而选择错误的格式可能会影响报表和列表分组中未来的计算和聚合值。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **计算** 框中，开始构建计算：
   1. 单击 **最大化** 打开计算编辑器并生成计算。</p>
计算通常以表达式开头，后跟括号，其中包含在自定义表单附加到对象时要引用的字段。

      每个字段都必须用大括号括起来。 当您开始键入字段名称时，系统会提供建议，您可以选择一个字段以将其插入到计算中。

+++ **展开以查看计算自定义字段中所需的语法**

      每个字段必须使用下面介绍的语法，并在每个字段名称周围带有大括号。 当您开始键入字段名称时，系统会提供建议，您可以选择一个字段以将其插入到计算中。 如果您在计算中输入的数据不正确，将出现警告消息，提醒您。 除非编辑计算以包含有效字段和有效的计算表达式，否则无法保存表单。

      >[!NOTE]
      >
      >目前，系统仅在您开始键入要在自定义表单将附加到的对象中引用的字段名称时，才会提出建议。 不建议使用父对象中的字段。

      **用大括号括住字段名称**

      * 如果希望计算引用内置字段，则字段的名称必须用大括号括起来。

         例如： `{actualRevenue}`

         字段名称区分大小写，且必须准确显示在Workfront系统中的显示方式，才能在计算中显示。

         导航到 [Workfront API Explorer](https://developer.adobe.com/workfront/api-explorer/) 以标识可用于计算的字段名称。

      * 如果希望计算引用自定义字段，则字段名称必须用大括号括起来，并在前面加上 `DE:` 括号内。

         例如： `{DE:Profit}`

         系统会列出您在键入时可以从中选择的所有自定义字段 `DE:`.

         * 如果希望计算引用将从 *父项* 对象在自定义表单附加到对象后，必须在字段名称前面加上父对象的对象类型，也以花括号括起来。

         例如，如果自定义表单配置为处理任务，并且您希望字段在表单附加到任务时计算父对象的实际收入，则需要指示 `Project` 作为字段的对象类型：

         `{project}.{actualRevenue}`

         或者，如果是自定义字段：

         `{project}.{DE:profit}`

         **使用句点分隔项目**

         在计算的自定义字段中引用相关对象时，必须使用句点来分隔对象名称和属性。

         例如，在任务类型自定义表单中，要在计算的自定义字段中显示Portfolio所有者的名称，您应键入以下内容：

         `{project}.{porfolio}.{owner}`

         这将确定以下内容：从自定义表单（任务）的对象中，可以访问与任务（项目）相关的下一个对象。 从此处，您可以访问项目（组合）的下一个相关对象，然后引用为组合对象（所有者）定义的字段

         **用于引用自定义字段的名称语法**

         在计算的自定义字段中引用其他自定义字段时，您需要输入该字段在Workfront用户界面中显示的名称。

         例如，要在标有执行赞助商的自定义字段中引用所选选项，您应键入以下内容：

         `{DE:Executive sponsor}`

         >[!NOTE]
         >
         >typeahead字段的语法与其他类型字段的语法略有不同，因为您需要添加 `:name` 最后。
         >
         >例如，要引用名为“执行赞助商”的自定义类型前导字段中的选定选项，您需要键入：
         >
         >`{DE:Executive sponsor:name}`


         **多对象自定义表单中的计算自定义字段**

         在多对象自定义表单中，所选对象类型必须至少与表单计算自定义字段中引用的一个字段兼容。 与对象不兼容的字段将在表单上显示N/A。

         要确保计算字段显示所有对象类型的正确结果，您必须使用 `$$OBJCODE` 定义每个对象类型的计算。

         >[!INFO]
         >
         >**示例:**
         >
         >在配置为处理项目、任务和问题的自定义表单中，您可以使用以下公式来显示对象类型：
         >
         >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
         >
         >在项目中，字段将显示“这是项目”，在任务中将显示“这是任务”，在问题中，字段将显示“这是问题”。


         >[!INFO]
         >
         >**示例：** 尽管没有分配给：项目中的“名称”字段中有一个内置的“所有者”字段（除非有人手动更改此字段，否则将自动填写创建项目的人员的姓名）。
         >
         >因此，在您的自定义“主管”字段中，您可以使用 `$$OBJCODE` 如下所示，在将自定义表单附加到项目时引用“所有者”字段，并且指定给：表单附加到任务时的“名称”字段：
         >
         >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

         有关变量(如 `$$OBJCODE,` 请参阅 [通配符过滤器变量](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

         **自动更新计算的自定义字段**

         发生以下情况时，对象上的计算自定义字段会自动重新计算：

         * 对象上的某些内容会发生更改，例如每日时间轴计算。
         * 某人编辑了对象上计算自定义字段引用的其他字段。
         * 计算表达式为空，且字段包含值 — 这会将值设置为null。

            >[!NOTE]
            >
            ><div>在附加到对象的自定义表单中，计算的自定义字段中的日期和时间语句由协调通用时间(UTC)计算和保存，而不是由为组织实例和用户配置文件设置的时区配置来计算和保存。 自定义表单中的计算会根据每个用户的各个时区生成。</div>

+++
   1. 单击大文本框，然后单击 **表达式** 和 **字段** ，以将其添加到计算中。

      您还可以在大型文本框中开始键入表达式或字段，然后在显示时将其选中。 每个项目都显示“F”作为字段，“E”作为表达式。

      如果键入左圆括号，则会自动添加右圆括号。

+++ **展开以查看有用的提示**
      >[!TIP]
      >
      >您可以执行以下任一操作来获取有关计算的帮助：
      > 
      >* 将鼠标悬停在计算中的表达式上可查看描述、显示如何使用该表达式的示例，以及指向文章中更多信息的“了解更多”链接 [计算数据表达式](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
         >  ![](assets/hover-expression-help-text.jpg)
      >* 使用颜色编码标识已添加的组件。 表达式以蓝色显示，字段以绿色显示。
         >  ![](assets/colors-fields-expressions.jpg)
      >* 查找计算错误，并在您转到时以粉红色突出显示。 您可以将鼠标悬停在突出显示的错误上，以显示其原因的简要描述。
         >  ![](assets/error-help.png)
      >* 在计算下方的区域中，预览现有Workfront对象的结果。
         ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

         >  ![](assets/preview-calc.jpg)
      >* 使用左侧显示的行号在长计算中引用表达式。


+++
   1. 单击 **最小化** 完成计算的自定义字段的计算时。

   1. （可选）使用以下任意选项进一步配置计算的自定义字段：

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">添加逻辑</td> 
      <td>您可以添加显示逻辑，以根据用户在填写表单时在前多个选择字段（下拉列表、复选框或单选按钮）中至少做出的一项选择来确定是否显示计算字段。 <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>仅当表单上计算的自定义字段之前至少有一个复选框、单选按钮或下拉字段时，才可使用此选项。 </p> <p>跳过逻辑对于计算的自定义字段不可用。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新以前的计算</td> 
      <td>编辑现有的计算自定义字段时，您可以选择此选项以在保存自定义表单时触发计算中的更新。 仅在保存自定义表单时发生一次。 在执行此操作后，选项会返回到其禁用状态。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">在说明中显示公式</td> 
      <td>如果希望填写自定义表单的用户在将鼠标悬停在字段上时查看字段的公式，请启用此选项。 有关更多信息，请参阅 <a href="#instructions" class="MCXref xref">说明</a> 在此表格的前面。</td> 
     </tr> 
    </tbody> 
   </table>

1. 要保存更改，请单击 **应用** 然后转到其他部分以继续构建表单。

   或

   单击 **保存并关闭**.


