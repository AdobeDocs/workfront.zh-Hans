---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器将自定义字段添加到自定义表单
description: 处理自定义表单时，您可以创建新的自定义字段并将其添加到自定义表单。 您还可以添加已添加到其他自定义表单的自定义字段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '2208'
ht-degree: 2%

---

# 使用旧版表单生成器将自定义字段添加到自定义表单

处理自定义表单时，您可以创建新的自定义字段并将其添加到自定义表单。

您还可以添加已添加到其他自定义表单的自定义字段。 有关说明，请参阅 [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

有关将资产小组件添加到自定义表单（与添加自定义字段类似的过程）的信息，请参阅 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>在包含许多自定义字段或在自定义字段中包含许多多选选项的自定义表单中，用户在添加或更改这些字段中的值时可能会遇到性能变慢的情况。 例如，包含100个自定义字段或具有超过200个选项的多选自定义字段的表单，在用户与其交互时速度可能会较慢。

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
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有哪些计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 将自定义字段添加到自定义表单

1. 开始创建或编辑自定义表单，如中所述 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 打开 **添加字段** 选项卡。

   ![](assets/add-a-field.jpg)

1. 替换为 **新建字段** ![](assets/new-field.jpg) 选中，请选择下面列出的字段类型之一：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">单行文本字段</td> 
      <td>允许用户在字段中键入单行文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">段落文本字段</td> 
      <td>允许用户在字段中键入多行文本。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">带格式的文本字段</td> 
      <td>允许用户在字段中键入多行文本，并使用粗体、斜体、下划线、项目符号、编号、超链接和块引号设置文本的格式。 可在主页、更新区域、列表和Workfront对象的详细信息区域中找到它。 15,000个字符的限制允许使用大量文本和格式。</p> <p>有关通过API访问此字段的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API中的富文本字段存储</a>.</p> <p><b>注意</b>：带格式的文本字段不可用于Workfront移动设备应用程序（将在未来版本中提供）。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下拉</td> 
      <td>提供下拉选项列表。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">键盘缓冲 </td> 
      <td>允许用户键入Workfront中存在的对象的名称。 用户开始键入内容时，将显示建议列表。
      此字段类型支持以下对象：
      <ul><li>用户</li>
      <li>组</li>
      <li>工作角色</li>
      <li>项目组合</li>
      <li>项目群</li>
      <li>项目</li>
      <li>团队</li>
      <li>模板</li>
      <li>公司</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">已计算</td> 
      <td>允许您定义表达式并在自定义表单上显示结果。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">将计算的数据添加到自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">日期</td> 
      <td>显示一个日历，用户可以在其中选择日期和时间。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">复选框</td> 
      <td>允许用户选择多个选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">单选按钮</td> 
      <td>要求用户仅选择一个选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明文本</td> 
      <td>允许您包含相关说明，并包含指向Workfront外部页面的链接。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">分节符</td> 
      <td>分区界限实际上不是字段。 您可以使用分区界限将自定义字段和小组件组织到分区中，并在必要时为每个分区配置不同的查看和编辑权限。 有关添加和配置分区界限的信息，请参见 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">向自定义表单添加分区界限</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **字段设置** 选项卡，配置可用于要添加的自定义字段类型的选项：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在自定义字段上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要</b>：避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是向Workfront中的各个区域（如报表、主页和API交互）添加自定义字段时，系统标识该字段的方式。</p> <p>首次配置自定义字段并键入标签时，将自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够自由地更改用户看到的标签，而不必更改系统看到的名称。</p> 
      <p><b>重要</b>：   
      <ul> 
      <li>虽然可以这样做，但我们建议您在或其他用户开始使用Workfront中的自定义表单后，不要更改此名称。 如果这样做，系统将不再识别现在可能在Workfront其他区域引用它的自定义字段。 <p>例如，如果您将自定义字段添加到报表后更改其名称，Workfront将无法在报表中识别该字段，并且除非您使用新名称将其重新添加到报表，否则将无法在该报表中正常发挥作用。</p> </li>
      <li> <p>我们建议您不要键入已用于内置Workfront字段的名称。</p> </li>
      <li><p>我们建议您在自定义字段名称中不要使用句点/点字符，以防止在Workfront的不同区域使用字段时出错。</p></li>
      </ul> <p>每个自定义字段名称在贵组织的Workfront实例中必须是唯一的。 这样，您就可以重新使用已为其他自定义表单创建的表单。 有关更多信息，请参阅 <a href="#Add" class="MCXref xref">将自定义字段添加到自定义表单</a> 本文章中。</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>选择将在自定义字段中捕获的数据类型。</p> <p><b>注释</b>:   
        <ul> 
         <li>保存表单后无法编辑此字段。 如果要在数学计算中使用字段，请确保选择“数字”或“货币”格式。<br></li> 
         <li>选择数字或货币时，系统会自动截断以0开头的数字。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示类型</td> 
      <td>（仅下拉列表、复选框和单选按钮）切换字段所需的选项选择类型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（仅限文本字段）选择字段的宽度。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示当日时间</td> 
      <td>（仅限日期字段）如果要显示一天中的时间以及字段中的日期，请选择此选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">参考对象类型</td> 
      <td> <p>（仅限预输入字段）选择要与字段关联的对象类型。</p> <p>单击“应用”或“保存+关闭”后，将无法更改该字段的对象类型。</p> <p><b>注释</b>:   
        <ul> 
         <li>如果您的Workfront管理员在Workfront用户界面中自定义了Portfolio、程序或项目的名称，则该对象的默认Workfront名称将显示在此下拉列表中，而不是自定义名称。 如果您需要此方面的帮助，请咨询您的Workfront管理员。<br></li> 
         <li>iOS和Android Workfront Mobile应用程序支持以下对象类型：用户、公司、组、工作角色、Portfolio、项目、项目和模板。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">添加筛选器</td> 
      <td> <p>（仅限预输入字段）为对象类型添加过滤器，以限制用户在使用字段时可以选择的对象。 </p> <p>例如，您可以限制一个字段，以便只有在满足以下条件时才能选择用户名：</p> 
       <ul> 
        <li>它们属于您指定的一个或多个组</li> 
        <li>它们与您指定的角色或职称相关联</li> 
        <li>他们与使用字段的人员属于同一组</li> 
       </ul> <p>必须使用“文本模式”语法为所选对象类型定义过滤器。 有关使用文本模式创建过滤器的信息，请参阅部分 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">在筛选器中编辑文本模式</a> 在文章中 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">文本模式概述</a>. </p> <p><b>注释</b>:   
        <ul> 
         <li>如果您正在编辑现有的自定义表单，则将过滤器添加到“预输入”字段不会删除用户已使用该字段添加的任何对象（在过滤器的范围外）。</li> 
         <li>此筛选器在移动设备上不可用。 如果您将过滤器用于“预输入”字段，则该字段将显示在用户的移动设备上而不受过滤器影响。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明文本</td> 
      <td>（仅限描述性文本字段）键入要显示的文本，以便在自定义表单上提供说明或链接。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">超链接</td> 
      <td>（仅限描述性文本字段）如果要将超链接应用于已键入的描述性文本，请在此处添加该超链接。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">创建一个必填字段</td> 
      <td>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在更新提要中跟踪字段变化</td> 
      <td><p>单击下拉列表，然后选择要自动跟踪字段值更改的对象类型。</p> 
      <p><b>注意</b>：此选项不适用于以下内容：</p> 
      <ul> 
      <li>与以下对象类型关联的自定义表单：费用、公司、小版本、记帐记录和组。</li> 
      <li>以下字段类型：计算、描述性文本和分区界限</li> 
      </ul>
      <p><b>重要</b>：在此处选择或取消选择对象类型会影响与所选对象类型关联且包含此字段的所有自定义表单。 例如，如果在此处取消选择某个对象类型并保存自定义表单，则不再在包含该字段的任何自定义表单中跟踪该对象类型的字段值更改。</p>
       <p>在此处为字段选择对象类型并保存自定义表单后，该字段显示在“设置”的“更新馈送”区域的“自定义字段”选项卡上。</p> 
       <p>反之，如果在“设置”的“更新馈送”区域中删除了此字段，则会在与对象类型关联且包含此字段的所有自定义表单上取消选择此设置的对象类型。</p> 
       <p>有关更多信息，请参阅部分 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">添加您希望Workfront跟踪的字段</a> 在文章中 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">配置系统更新</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加逻辑</td> 
      <td>根据用户在现有字段中所做的选择，指定应在表单上显示的字段。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">将显示逻辑和跳过逻辑添加到自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">选项 </td> 
      <td> <p>（仅限下拉列表、复选框或单选按钮；可选）</p> 
       <ol> 
        <li> <p>单击 <b>选项</b>，然后启用以下任一项：</p> 
           <ul> 
            <li><strong>显示值</strong>：显示字段中每个选择的值。 默认情况下，将显示每个选项的标签。</li> 
            <li><strong>按A-Z排序选项</strong>：按字母顺序对您在字段中添加的选项进行排序。</li> 
           </ul> 
        </li> 
        <li> <p>对于您为用户添加的每个选择，单击齿轮图标 <img src="assets/gear-icon-settings.png">，然后选择以下选项之一：</p> 
           <ul> 
            <li><strong>默认选择</strong>：在字段中选择默认选项。</li> 
            <li> <p><strong>隐藏选择</strong>：隐藏字段中的选项。 隐藏选项在报表中仍可访问。</p> </li> 
            <li> <p><strong>删除选项</strong>：从字段中移除选项。</p> <p><b>警告</b>：如果当前有对象使用此选项，请勿将其从字段中移除。 删除它将导致历史数据丢失。 相反，选择隐藏它的选项，这会阻止用户将来选择它。</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）要更改自定义表单中字段的显示类型，请单击 **显示类型** 下拉菜单，然后单击所需的类型。

   您可以在以下字段显示类型之间切换：

   * **选择类型字段**：复选框、下拉列表、单选按钮。
   * **文本类型字段**：单行文本字段、段落文本字段。 (不能将带有格式的文本字段切换为其他显示类型。 但是，您可以删除它并添加其他类型的字段。)

   例如，如果已创建复选框字段，则可以将其更改为下拉字段或单选按钮字段。 或者，如果您已创建单行文本字段，则可以将其更改为段落文本字段。

   >[!NOTE]
   >
   >当想要将字段的显示类型从复选框字段或多选下拉字段（允许选择多个选项的下拉列表）更改为单选字段类型时，请考虑以下事项：
   >
   >* 如果更改为单选按钮，Workfront会保留用户可能在字段中输入的任何多选值，直到用户更改并将数据保存到表单的任何部分为止。 此时，使用“多选类型”字段选择的任何值都将被选中的“单选按钮”值替换。
   >* 如果更改为单选下拉列表，Workfront会保留用户可能在字段中输入的任何多选值，直到用户更改并将值保存在字段中。 此时，使用多选类型字段选择的任何值都将被所选的下拉列表值替换。


1. （可选）重复步骤2-6以添加其他自定义字段。

   或

   添加已为贵组织创建的字段，如中所述 [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >您最多可以在单个自定义表单上添加500个字段和小部件。 但是，当表单中存在超过100个时，可能会发生性能下降，具体取决于表单的复杂性。 复杂表单的示例包括带有级联参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 单击 **应用**.
1. 如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [向自定义表单添加分区界限](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [将显示逻辑和跳过逻辑添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
