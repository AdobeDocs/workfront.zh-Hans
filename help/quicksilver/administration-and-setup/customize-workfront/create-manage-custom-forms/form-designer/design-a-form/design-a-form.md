---
title: 使用窗体设计器设计窗体
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器设计自定义表单。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: b56cf20e054b2658ade8aef6c179128e001603c2
workflow-type: tm+mt
source-wordcount: '3803'
ht-degree: 4%

---


# 使用窗体设计器设计窗体

{{highlighted-preview-article-level}}

您可以使用表单设计器设计自定义表单。 您可以将自定义表单附加到不同的Workfront对象，以捕获有关这些对象的数据。

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
   <td>
   <p>当前计划：标准</p>
   <p>或</p>
   <p>传统计划：计划</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;要了解您拥有哪些计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 开始设计自定义表单

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **自定义Forms** （在左侧面板中）。

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. 单击 **新建自定义表单。**
1. 选择要将自定义表单附加到的对象类型，然后单击 **继续**.

   ![](assets/choose-object-type.jpg)

1. 在 **标题为必填项** 区域，键入自定义表单标题。
1. （可选）如果要向表单中添加更多对象类型，以便将其附加到更多对象，请单击 **添加** 图标 ![](assets/add-objects-icon.png) 之后 **对象类型**，然后在显示的菜单中选择所需的类型。 您可以重复此操作，以添加所需数量的对象类型。

   也可以单击对象类型上的X将其从表单中删除。

   >[!CAUTION]
   >
   >删除自定义表单也会删除与表单关联的对象上的所有自定义数据。 无法恢复已删除的数据。 请考虑改为停用自定义表单 — 在停用不再使用的自定义表单时，将保留所有关联的历史数据。
   >
   >有关更多信息，请参阅 [删除自定义表单上的对象类型](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).


1. 接下来，您可以开始向自定义表单添加字段。 请参阅以下部分：
   * [重用已用于其他自定义表单中的现有字段或构件](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [添加文本字段](#add-text-fields)
   * [添加计算字段](#add-calculated-fields)
   * [添加单选按钮、复选框组和下拉列表](#add-radio-buttons-checkboxes-and-dropdowns)
   * [添加预输入和日期字段](#add-typeahead-and-date-fields)
   * [添加图像、PDF和视频](#add-images-pdfs-and-videos)
   * [添加Adobe XD文件](#add-adobe-xd-files)

## 向自定义表单中添加新字段或现有字段

在设计自定义表单时，您可以使用新的或现有的字段。

## 重用已用于其他自定义表单中的现有字段或构件

1. 在屏幕的左上角，单击 **字段库**.

1. 将您希望在自定义表单中显示的字段或构件拖动到此处。
1. （可选）重复上一步以添加任何其他字段或构件。

   >[!NOTE]
   >
   >您最多可以在单个自定义表单上添加500个字段和小部件。 但是，当表单中存在超过100个时，可能会发生性能下降，具体取决于表单的复杂性。
   >
   >
   >复杂表单的示例包括带有级联参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

### 添加文本字段

您可以将多个不同的文本字段添加到自定义表单。

+++ **展开以查看可用文本字段的说明**

* **单行文本字段**：允许用户在字段中键入单行文本。
* **段落文本字段**：允许用户在字段中键入多行文本。
* **带格式的文本字段**：允许用户在字段中键入多行文本，并使用粗体、斜体、下划线、项目符号、编号、超链接和块引号设置文本的格式。 15,000个字符的限制允许使用大量文本和格式。

   有关通过API访问此字段的信息，请参阅API中的富文本字段存储。

   >[!NOTE]
   >
   >带格式的文本字段不适用于Workfront移动设备应用程序（在即将发布的版本中提供）。

* **描述性文本**：用于包含相关说明和指向Workfront外部页面的链接。

+++

要添加文本字段，请执行以下操作：

1. 在屏幕左侧，找到以下文本字段之一，并将其拖动到画布上的某个部分：

   * 单行文本：
   * 段落文本
   * 带格式的文本字段
   * 描述性文本

   ![](assets/drag-field-to-section.png)

1. 在屏幕右侧，配置可用于要添加的自定义字段类型的选项：

   <table>
    <tr>
    <td>输入到</td>
    <td>描述</td>
    <td>可用于 </td>
    </tr>
    <tr>
    <td>大小</td>
    <td><p>更改表单上文本字段的大小。<p>
   </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落文本</li>
    <li>带格式文本</li>
    <li>描述性文本 — 即将推出</li>
    </ul></td>
    </tr>
    <tr>
    <td>标签</td>
    <td><p>键入要在小部件上方显示的描述性标签。 您可以随时更改标签。<p>
    <p>重要信息：请避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p></td>
    <td><ul>
    <li>单行文本</li>
    <li>段落文本</li>
    <li>带格式文本</li>
    </ul></td>
    </tr>
    <tr>
     <td>名称</td>
    <td><p>（必需）此名称是系统标识字段的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够自由地更改用户看到的标签，而不必更改系统看到的名称。</p>
    <p><b>重要</b>：   
      <ul> 
      <li>虽然可以这样做，但我们建议您在或其他用户开始使用Workfront中的自定义表单后，不要更改此名称。 如果这样做，系统将不再识别现在可能在Workfront其他区域引用它的自定义字段。 <p>例如，如果您将自定义字段添加到报表后更改其名称，Workfront将无法在报表中识别该字段，并且除非您使用新名称将其重新添加到报表，否则将无法在该报表中正常发挥作用。</p> </li>
      <li> <p>我们建议您不要键入已用于内置Workfront字段的名称。</p> </li>
      <li><p>我们建议您在自定义字段名称中不要使用句点/点字符，以防止在Workfront的不同区域使用字段时出错。</p></li>
    </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落文本</li>
    <li>带格式文本</li>
    <li>描述性文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>说明</td>
    <td>键入有关小部件的任何其他信息。 当用户填写自定义表单时，可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落文本</li>
    <li>带格式文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>格式</td>
    <td><p>选择将在自定义字段中捕获的数据类型。</p> <p><b>注释</b>:   
    <ul> 
    <li>保存表单后无法编辑此字段。 如果要在数学计算中使用字段，请确保选择“数字”或“货币”格式。<br></li> 
    <li>选择数字或货币时，系统会自动截断以0开头的数字。</li> 
     </ul></p></td> </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>显示类型</td>
    <td>在单行文本字段和段落文本字段之间切换。</td>
    <td><ul>
    <li>单行文本</li>
    <li>段落文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>超链接</td>
    <td> 如果要将超链接应用于键入的描述性文本，请在此处添加该超链接。 描述性文本在附加表单的对象上显示为链接。</td>
    <td><ul><li>描述性文本</li></ul></td>
    </tr>
   </table>

1. （可选）重复上一步以添加任何其他字段或构件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

### 添加计算字段

在自定义表单中，您可以添加计算自定义字段，在将自定义表单附加到对象时，该字段使用现有数据生成新数据。

要添加计算字段，请参阅 [使用表单设计器添加计算字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

### 添加单选按钮、复选框和下拉列表

您可以将单选按钮、复选框和下拉列表添加到自定义表单。

+++ **展开以查看可用字段的说明**

* **单选按钮**：要求用户仅选择一个选项。
* **复选框组**：允许用户选择多个选项。
* **下拉列表**：提供下拉列表选项列表。

+++

要添加单选按钮和复选框，请执行以下操作：

1. 在屏幕左侧，找到以下字段之一，并将其拖动到画布上的某个部分。

   * 单选按钮
   * 复选框组
   * 下拉

   ![](assets/drag-field-to-section.png)

1. 在屏幕右侧，配置可用于要添加的自定义字段类型的选项：

   <table style="table-layout:auto"> 
    <tbody> 
    <tr>
    <td>输入到</td>
    <td>描述</td>
    <td>可用于 </td>
    </tr>
    <tr> 
     <td role="rowheader">标签</td> 
     <td> <p>（必需）键入要在自定义字段上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要</b>：避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
     <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
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
     <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">说明</td> 
    <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">格式</td> 
    <td> <p>选择将在自定义字段中捕获的数据类型。</p> <p><b>注释</b>:   
     <ul> 
    <li>保存表单后无法编辑此字段。 如果要在数学计算中使用字段，请确保选择“数字”或“货币”格式。<br></li> 
    <li>选择数字或货币时，系统会自动截断以0开头的数字。</li> 
     </ul></p></td> 
     <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">显示类型</td> 
    <td>在字段的单选按钮、复选框组或下拉列表之间切换。</td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
    </tr> 
     <tr> 
    <td role="rowheader">创建一个必填字段</td> 
    <td>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。 </td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
     </tr> 
    <tr> 
    <td role="rowheader">选项 </td> 
    <td> 
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
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>下拉</li>
    </ul></td>
     </tr> 
    </tbody> 
    </table>

1. （可选）重复上一步以添加任何其他字段或构件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

### 添加预输入和日期字段

您可以将预输入和日期字段添加到自定义表单。

+++ **展开以查看可用字段的说明**

* **预输入**：允许用户键入Workfront中存在的对象的名称。 用户开始键入内容时，将显示建议列表。 此字段类型支持以下对象：
   * 用户
   * 组
   * 工作角色
   * 项目组合
   * 项目群
   * 项目
   * 团队
   * 模板
   * 公司
* **日期字段**：显示一个日历，用户可在其中选择日期和时间。

+++

要添加预输入日期字段，请执行以下操作：

1. 在屏幕左侧，找到以下字段之一，并将其拖动到画布上的某个部分。

   * 键盘缓冲
   * 日期字段

   ![](assets/drag-field-to-section.png)

1. 在屏幕右侧，配置可用于要添加的自定义字段类型的选项：

   <table style="table-layout:auto"> 
    <tbody> 
     <tr>
    <td>字段设置</td>
    <td>描述</td>
    <td>可用于 </td>
    </tr>
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在自定义字段上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要</b>：避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
       <td><ul>
    <li>键盘缓冲</li>
    <li>日期字段</li>
    </ul></td>
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
         <td><ul>
    <li>键盘缓冲</li>
    <li>日期字段</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>键盘缓冲</li>
    <li>日期字段</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">显示当日时间</td> 
      <td>如果要在字段中显示一天中的时间和日期，请选择此选项。</td> 
         <td><ul>
    <li>日期字段</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">参考对象类型</td> 
      <td> <p>选择要与字段关联的对象类型。</p> <p>单击“应用”或“保存+关闭”后，将无法更改该字段的对象类型。</p> <p><b>注释</b>:   
        <ul> 
         <li>如果您的Workfront管理员在Workfront用户界面中自定义了Portfolio、程序或项目的名称，则该对象的默认Workfront名称将显示在此下拉列表中，而不是自定义名称。 如果您需要此方面的帮助，请咨询您的Workfront管理员。<br></li> 
         <li>iOS和Android Workfront Mobile应用程序支持以下对象类型：用户、公司、组、工作角色、Portfolio、项目、项目和模板。</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>键盘缓冲</li>
    </ul></td>
     </tr>
     <tr> 
      <td role="rowheader">创建一个必填字段</td> 
      <td>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。 </td> 
       <td><ul>
    <li>键盘缓冲</li>
    <li>日期字段</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. （可选）重复上一步以添加任何其他字段或构件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

### 添加图像、PDF和视频

您可以将图像、PDF和视频添加到自定义表单。 使用已附加自定义表单的对象的用户只能在以下区域查看图像、PDF或视频：

* 对象的详细信息区域（例如，对于项目，为项目详细信息区域）
* 对象的“编辑”框(如果它具有新的Adobe Workfront Experience外观)（例如，“编辑项目”框和“编辑任务”框）

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ **展开以查看可用字段的说明**

* **图像**：允许用户添加_____像文件。
* **PDF**：允许用户添加PDF
* **视频**：允许用户添加____视频文件。

+++

要添加图像、PDF或视频，请执行以下操作：

1. 在屏幕左侧，找到以下字段之一，并将其拖动到画布上的某个部分。

   * 图像
   * PDF
   * 视频

   ![](assets/drag-field-to-section.png)

1. 键入或编辑小部件的以下任意属性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在小部件上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要</b>：避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统标识构件的方式。</p> <p>首次配置构件并键入标签时，会自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够自由地更改用户看到的标签，而不必更改系统看到的名称。</p> <p><b>重要</b>：虽然可以这样做，但我们建议您在或其他用户开始使用小部件中的自定义表单后，不要更改此名称。 如果这样做，系统将不再识别现在可能在Workfront的其他区域引用它的小组件。 </p> <p>每个构件名称在贵组织的Workfront实例中必须是唯一的。 这样，您就可以重新使用已为其他自定义表单创建的表单。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴存储在Internet上的构件的URL。</p> 
      <p>如果要添加视频小组件，当前可以通过在URL框中添加以下内容来实现此目的：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo链接</p> </li> 
      <li> <p>Google Drive视频链接</p> </li> 
      <li> <p>带有MP4和MOV扩展的视频链接</p> </li> 
      <li> <p>视频链接已上传到Workfront实例中的文档区域。 有关说明，请参阅 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">从“文档”区域向自定义表单添加视频构件</a> 本文章中。</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关小部件的任何其他信息。 当用户填写自定义表单时，可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>根据需要更改构件的显示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复上一步以添加任何其他字段或构件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

#### **从“文档”区域向自定义表单添加视频构件**{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以这种方式将视频添加到自定义表单时，当用户访问对象上的表单时，只有为自定义表单设置的权限才应用于视频，而不是在文档区域为视频设置的权限。

1. 转到文档区域中的视频并为其生成验证，如中所述 [为网站或其他Web内容创建交互式验证](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 打开证明。
1. 右键单击视频上的任意位置，然后选择 **复制视频地址**.
1. 在添加视频小部件的自定义表单中，将复制的地址粘贴到 **URL** 盒子。
1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

### 添加Adobe XD文件

您可以将Adobe XD原型直接添加到自定义表单。 使用附加了自定义表单的对象的用户只能在以下区域查看Adobe XD文件：

* 对象的详细信息区域（例如，对于项目，为项目详细信息区域）
* 对象的“编辑”框(如果它具有新的Adobe Workfront Experience外观)（例如，“编辑项目”框和“编辑任务”框）

添加Adobe XD文件：

1. 在屏幕左侧，查找 **Adobe XD** 然后将其拖动到画布上的某个区域。
1. 键入或编辑小部件的以下任意属性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在小部件上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要</b>：避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统标识构件的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够自由地更改用户看到的标签，而不必更改系统看到的名称。</p>
    <p><b>重要</b>：   
      <ul> 
      <li>虽然可以这样做，但我们建议您在或其他用户开始使用Workfront中的自定义表单后，不要更改此名称。 如果这样做，系统将不再识别现在可能在Workfront其他区域引用它的自定义字段。 <p>例如，如果您将自定义字段添加到报表后更改其名称，Workfront将无法在报表中识别该字段，并且除非您使用新名称将其重新添加到报表，否则将无法在该报表中正常发挥作用。</p> </li>
      <li> <p>我们建议您不要键入已用于内置Workfront字段的名称。</p> </li>
      <li><p>我们建议您在自定义字段名称中不要使用句点/点字符，以防止在Workfront的不同区域使用字段时出错。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴有效的XD原型链接。</p> 
      <p>注意：Adobe XD中“共享”选项卡上的“链接访问”设置必须设置为具有链接的任何人。 否则，用户将无法查看原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关小部件的任何其他信息。 当用户填写自定义表单时，可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改小部件的显示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复上一步以添加任何其他字段或构件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击 **应用** 并转到另一个部分以继续构建您的表单。

   或

   单击 **保存并关闭**.

## 使用表单设计器组织和预览表单

有关如何组织和查看表单预览的信息，请参阅 [使用表单设计器组织和预览表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).