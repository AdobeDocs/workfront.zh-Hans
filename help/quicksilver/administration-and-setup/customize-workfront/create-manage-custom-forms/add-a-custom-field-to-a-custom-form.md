---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器将自定义字段添加到自定义表单
description: 处理自定义表单时，可以创建新的自定义字段并将其添加到自定义表单。 您还可以添加已添加到其他自定义表单的自定义字段。
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

处理自定义表单时，可以创建新的自定义字段并将其添加到自定义表单。

您还可以添加已添加到其他自定义表单的自定义字段。 有关说明，请参阅 [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

有关将资产小组件添加到自定义表单（与添加自定义字段类似的过程）的信息，请参阅 [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>在包含大量自定义字段或自定义字段中许多多选选项的自定义表单中，用户在添加或更改这些字段中的值时可能会遇到性能降低的情况。 例如，当用户与表单进行交互时，包含100个自定义字段或包含200个以上选项的多选自定义字段的表单速度可能会较慢。

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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请联系您的Workfront管理员。

## 将自定义字段添加到自定义表单

1. 开始创建或编辑自定义表单，如 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 打开 **添加字段** 选项卡。

   ![](assets/add-a-field.jpg)

1. 使用 **新建字段** ![](assets/new-field.jpg) 选中后，选择下面列出的字段类型之一：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">单行文本字段</td> 
      <td>允许用户在字段中键入一行文本。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">段落文本字段</td> 
      <td>允许用户在字段中键入多行文本。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">带格式的文本字段</td> 
      <td>允许用户在字段中键入多行文本，并使用粗体、斜体、下划线、项目符号、编号、超链接和块引号设置文本格式。 这可在“主页”(Home)、“更新”(Updates)区域、列表和Workfront对象的“详细信息”(Details)区域中找到。 字符数限制为15,000，允许大量文本和格式。</p> <p>有关通过API访问此字段的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">API中的富文本字段存储</a>.</p> <p><b>注意</b>:格式化的文本字段不适用于Workfront移动设备应用程序（在即将发行的版本中提供）。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">下拉</td> 
      <td>提供下拉选项列表。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">键盘缓冲 </td> 
      <td>允许用户键入Workfront中存在的对象的名称。 当用户开始键入内容时，会显示建议列表。
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
      <td>用于定义表达式并在自定义表单上显示结果。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">将计算数据添加到自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">日期</td> 
      <td>显示日历，用户可在其中选择日期和时间。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">复选框</td> 
      <td>允许用户选择多个选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">单选按钮</td> 
      <td>要求用户只选择一个选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明文本</td> 
      <td>允许您包含说明和指向Workfront以外页面的链接。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">分节符</td> 
      <td>分区实际上不是字段。 您可以使用节划分将自定义字段和小组件整理到各节中，并根据需要为每个节配置不同的查看和编辑权限。 有关添加和配置节点的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">向自定义表单中添加节分符</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **字段设置** 选项卡，配置可用于添加的自定义字段类型的选项：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在自定义字段上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>:避免在此标签中使用特殊字符。 无法在报表中正确显示它们。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是在您将自定义字段添加到Workfront中的各个区域（如报表、主页和API交互）时，系统如何标识该字段。</p> <p>首次配置自定义字段并键入标签时，“名称”字段会自动填充以进行匹配。 但“标签”和“名称”字段未同步，这可让您自由更改用户看到的标签，而无需更改系统看到的名称。</p> 
      <p><b>重要信息</b>:   
      <ul> 
      <li>尽管可以这样做，但我们建议您在您或其他用户开始使用Workfront中的自定义表单后，不要更改此名称。 如果您这样做，系统将不再识别自定义字段，该字段现在可能会在Workfront的其他区域中引用。 <p>例如，如果您将自定义字段添加到报表中，稍后更改其名称，则Workfront将无法在报表中识别该字段，除非您使用新名称将其重新添加到报表中，否则该字段将在报表中正常运行。</p> </li>
      <li> <p>我们建议您不要键入已用于内置Workfront字段的名称。</p> </li>
      <li><p>我们建议您不要在自定义字段名称中使用句点/圆点字符，以防止在Workfront的不同区域中使用字段时出错。</p></li>
      </ul> <p>在贵组织的Workfront实例中，每个自定义字段名称必须唯一。 这样，您就可以重复使用已为其他自定义表单创建的表单。 有关更多信息，请参阅 <a href="#Add" class="MCXref xref">将自定义字段添加到自定义表单</a> 在本文中。</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，他们可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式</td> 
      <td> <p>选择将在自定义字段中捕获的数据类型。</p> <p><b>注释</b>:   
        <ul> 
         <li>保存表单后，无法编辑此字段。 如果您打算在数学计算中使用字段，请确保选择数字或货币格式。<br></li> 
         <li>选择“数字”或“货币”时，系统会自动截断以0开头的数字。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示类型</td> 
      <td>（仅限下拉列表、复选框和单选按钮）切换所需字段的选项选择类型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（仅限文本字段）为字段选择宽度。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">显示当日时间</td> 
      <td>（仅限日期字段）如果要在字段中显示一天中的时间以及日期，请选择此选项。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">参考对象类型</td> 
      <td> <p>（仅限Typeahead字段）选择要与字段关联的对象类型。</p> <p>单击应用或保存并关闭后，便无法更改字段的对象类型。</p> <p><b>注释</b>:   
        <ul> 
         <li>如果您的Workfront管理员在Workfront用户界面中为Portfolio、程序或项目自定义了名称，则对象的默认Workfront名称会显示在此下拉列表中，而不是自定义名称。 如需有关此方面的帮助，请咨询Workfront管理员。<br></li> 
         <li>iOS和Android Workfront移动设备应用程序支持以下对象类型：用户、公司、组、职务角色、Portfolio、项目、项目和模板。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">添加筛选器</td> 
      <td> <p>（仅限Typeahead字段）为对象类型添加过滤器，以限制用户在使用字段时可以选择的对象。 </p> <p>例如，您可以限制字段，以便仅在用户名满足以下条件时才能选择其用户名：</p> 
       <ul> 
        <li>它们属于您指定的组或组</li> 
        <li>它们与您指定的角色或职务相关联</li> 
        <li>它们属于使用字段的人员所在的组</li> 
       </ul> <p>必须使用文本模式语法为所选对象类型定义过滤器。 有关使用文本模式创建过滤器的信息，请参阅部分 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md#editing2" class="MCXref xref">在过滤器中编辑文本模式</a> 在文章中 <a href="../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md" class="MCXref xref">文本模式概述</a>. </p> <p><b>注释</b>:   
        <ul> 
         <li>如果您正在编辑现有的自定义表单，则向Typeahead字段添加过滤器不会删除用户已使用该字段添加的任何对象（在过滤器的范围之外）。</li> 
         <li>此过滤器在移动设备上不可用。 如果您对Typeahead字段使用过滤器，则该字段将显示在未受该过滤器影响的用户移动设备上。</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明文本</td> 
      <td>（仅限描述性文本字段）键入要显示的文本以在自定义表单上提供说明或链接。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">超链接</td> 
      <td>（仅限描述性文本字段）如果要将超链接应用于您键入的描述性文本，请将其添加到此处。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">创建必填字段</td> 
      <td>如果希望必填字段以供用户完成自定义表单，请选择此选项。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">在更新提要中跟踪字段变化</td> 
      <td><p>单击下拉列表，然后选择要自动跟踪字段值更改的对象类型。</p> 
      <p><b>注意</b>:此选项不适用于以下情况：</p> 
      <ul> 
      <li>与以下对象类型关联的自定义表单：费用、公司、迭代、帐单记录和组。</li> 
      <li>以下字段类型：计算量度、描述性文本和分节时间</li> 
      </ul>
      <p><b>重要信息</b>:选择或取消选择此处的对象类型会影响与所选对象类型关联并包含此字段的所有自定义表单。 例如，如果在此处取消选择对象类型并保存自定义表单，则在包含该字段的任何自定义表单中，将不再跟踪该对象类型对字段值的更改。</p>
       <p>在此处为字段选择对象类型并保存自定义表单后，该字段会显示在“设置”的“更新馈送”区域的“自定义字段”选项卡中。</p> 
       <p>相反，如果在“设置”的“更新馈送”区域中删除了此字段，则在与对象类型关联并包含此字段的所有自定义表单上，都会取消选择此设置的对象类型。</p> 
       <p>有关更多信息，请参阅 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#adding-fields-to-the-update-feeds" class="MCXref xref">添加您希望Workfront跟踪的字段</a> 在文章中 <a href="../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md" class="MCXref xref">配置系统更新</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加逻辑</td> 
      <td>根据用户在现有字段中所做的选择，指定应在表单上显示哪些字段。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">向自定义表单添加显示逻辑和跳过逻辑</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">选项 </td> 
      <td> <p>(仅限下拉列表、复选框或单选按钮；可选)</p> 
       <ol> 
        <li> <p>单击 <b>选项</b>，然后启用以下任一项：</p> 
           <ul> 
            <li><strong>显示值</strong>:显示字段中每个选项的值。 默认情况下，每个选项的标签都会显示。</li> 
            <li><strong>排序选项A-Z</strong>:按字段中的字母顺序对您添加的选项进行排序。</li> 
           </ul> 
        </li> 
        <li> <p>对于您为用户添加的每个选项，单击齿轮图标 <img src="assets/gear-icon-settings.png">，然后选择以下选项之一：</p> 
           <ul> 
            <li><strong>默认选择</strong>:默认情况下，在字段中选择选项。</li> 
            <li> <p><strong>隐藏选择</strong>:在字段中隐藏选项。 隐藏的选项仍可在报表中访问。</p> </li> 
            <li> <p><strong>删除选择</strong>:从字段中删除选择。</p> <p><b>警告</b>:如果当前有使用此选项的对象，请勿将其从字段中删除。 删除它将导致历史数据丢失。 相反，请选择用于隐藏该内容的选项，这会阻止用户在将来选择该内容。</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. （视情况而定）要更改自定义表单上字段的显示类型，请单击 **显示类型** 下拉菜单，然后单击所需的类型。

   您可以在以下字段显示类型之间切换：

   * **选择类型字段**:复选框、下拉列表、单选按钮。
   * **文本类型字段**:单行文本字段、段落文本字段。 (无法将具有格式的文本字段切换到其他显示类型。 但是，您可以删除该字段并添加其他类型的字段。)

   例如，如果已创建复选框字段，则可将其更改为下拉字段或单选按钮字段。 或者，如果已创建单行文本字段，则可将其更改为段落文本字段。

   >[!NOTE]
   >
   >如果要将字段的显示类型从复选框字段或多选下拉字段（允许选择多个选项的下拉字段）更改为单选字段类型，请考虑以下事项：
   >
   >* 如果您更改为单选按钮，Workfront将保留用户可能在字段中输入的任何多选值，直到用户更改并在表单的任何部分中保存数据为止。 此时，使用多选类型字段选择的任何值都将被替换为选定的单选按钮值。
   >* 如果您更改为单选下拉列表，则Workfront将保留用户可能在字段中输入的任何多选值，直到用户更改并在字段中保存这些值为止。 此时，使用多选类型字段选择的任何值都将被替换为选定的下拉值。


1. （可选）重复步骤2-6以添加其他自定义字段。

   或

   添加已为贵组织创建的字段，如 [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md#add).

   >[!NOTE]
   >
   >您最多可以在一个自定义表单上添加500个字段和小组件。 但是，如果表单上存在超过100个，则性能可能会降低，具体取决于表单的复杂性。 复杂表单的示例包括具有级联参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 单击 **应用**.
1. 如果您希望以其他方式继续构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中放置自定义字段和小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [在自定义表单中添加或编辑资产小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [向自定义表单中添加节分符](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [在自定义表单中重复使用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
