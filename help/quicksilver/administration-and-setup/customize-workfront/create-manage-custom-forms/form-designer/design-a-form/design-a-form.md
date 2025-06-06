---
title: 创建自定义表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器设计自定义表单。 您可以将自定义表单附加到不同的Workfront对象，以捕获有关这些对象的数据。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 886a348e-1a52-418f-b4c4-57b2e690b81d
source-git-commit: 0ff02569d3c7fb532a2faafc46fe4235ce77acd4
workflow-type: tm+mt
source-wordcount: '6494'
ht-degree: 5%

---

# 创建自定义表单

<!-- Audited: 6/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>   -->

您可以使用Adobe Workfront中的表单设计器设计自定义表单。 您可以将自定义表单附加到不同的Workfront对象，以捕获有关这些对象的数据。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划</p> </td> 
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
   <td> <p>对自定义表单的管理访问权限</p> </td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 开始设计自定义表单

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**自定义Forms**，然后选择&#x200B;**Forms**。

1. 单击&#x200B;**新建自定义表单。**
1. 选择要将自定义表单附加到的对象类型，然后单击&#x200B;**继续**。

   ![选择对象类型](assets/choose-object-type.jpg)

1. 在&#x200B;**添加表单名称**&#x200B;区域，键入自定义表单标题。
1. （可选）如果要向表单中添加更多对象类型，以便可以将其附加到更多对象，请单击&#x200B;**对象类型**&#x200B;旁边的&#x200B;**添加**&#x200B;图标![添加对象图标](assets/add-objects-icon.png)，然后在显示的菜单中选择所需的类型。 您可以重复此操作，以添加所需数量的对象类型。

   将多个对象添加到表单后，可以单击对象类型上的X将其从表单中删除。

   >[!CAUTION]
   >
   >删除自定义表单也会删除与表单关联的对象上的所有自定义数据。 无法恢复已删除的数据。 或者，您可以停用不再使用的自定义表单，这会保留所有关联的历史数据。
   >
   >有关详细信息，请参阅[从现有自定义表单中添加或删除对象类型](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/add-or-remove-objects-from-a-form.md)和[停用或重新激活自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/activate-deactivate-form.md)。


1. 接下来，您可以开始向自定义表单添加字段。 有关更多信息，请参阅以下部分：
   * [重用已在其他自定义表单中使用的现有字段或构件](#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [有关字段名称和标签的说明](#notes-on-field-names-and-labels)
   * [添加文本字段](#add-text-fields)
   * [添加计算字段](#add-calculated-fields)
   * [添加单选按钮、复选框组和下拉列表](#add-radio-buttons-checkbox-groups-and-drop-downs)
   * [添加预输入和日期字段](#add-typeahead-and-date-fields)
   * [添加外部查找字段](#add-external-lookup-fields)
   * [添加图像、PDF和视频](#add-images-pdfs-and-videos)
   * [添加Workfront本机字段](#add-workfront-native-fields)
   * [添加Adobe XD文件](#add-adobe-xd-files)
   * [添加Planning连接字段](#add-planning-connection-fields)

## 向自定义表单中添加新字段或现有字段

在设计自定义表单时，您可以使用新的或现有的字段。

自定义表单限制为500个字段。 左下方的计数器显示表单上使用了多少字段，当您在表单设计器中滚动时，它始终可见。

### 重用已在其他自定义表单中使用的现有字段或构件

1. 在屏幕的左上角，单击&#x200B;**字段库**。

1. 将所需的字段或构件拖放到画布上。 重复此步骤以添加任何其他字段或构件。

   >[!NOTE]
   >
   >您最多可以在单个自定义表单上添加500个字段和小部件。 但是，当表单中存在超过100个时，可能会发生性能下降，具体取决于表单的复杂性。
   >
   >
   >复杂表单的示例包括带有层叠参数的表单、计算的自定义数据字段以及单个字段中的多个值选项。

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 有关字段名称和标签的说明 {#notes-on-field-names-and-labels}

标签适用于大多数字段。 它是一个描述性标签，显示在自定义表单上的字段或小部件的上方。 您可以随时更改标签。

>[!NOTE]
>
>避免在此标签中使用特殊字符，因为它们无法在报表中正确显示。

每个字段都需要名称。 此名称是向Workfront中的各个区域添加自定义字段时（例如报表、主页和API交互）系统识别该字段的方式。 首次配置字段或小组件并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。

每个自定义字段名称在贵组织的Workfront实例中必须唯一。 这样，您就可以重复使用已经为其他自定义表单创建的表单。

>[!NOTE]
>
>虽然可以这样做，但我们建议，在您或其他用户开始使用Workfront中的自定义表单后，不要更改此名称。 如果这样做，系统将不再能够识别Workfront其他区域中现在可能引用该字段的自定义字段。
>>例如，如果您将自定义字段添加到报表后更改其名称，Workfront将无法识别该字段在报表中的名称，并且除非您使用新名称将其重新添加到报表，否则该字段将在报表中停止正常工作。
>
>我们建议您不要键入已用于内置Workfront字段的名称。
>
>我们建议您在自定义字段名称中不要使用句点/点字符，以免在Workfront的其他区域使用字段时出错。

自定义字段标签和名称不支持以下特殊字符。

* \t
* \n
* \r
* \f
* `[`
* `]`
* (
* )
* ：
* `{`
* `}`

### 添加文本字段

您可以向自定义表单添加多个不同的文本字段。

+++ 展开以查看可用文本字段的说明。

* **单行文本字段**：允许用户在该字段中键入单行文本。
* **段落字段**：允许用户在该字段中键入多行文本。
* **带格式的文本字段**：允许用户在该字段中键入多行文本，并用粗体、斜体、下划线、项目符号、编号、超链接和块引号设置文本的格式。 15,000个字符的限制允许使用大量文本和格式。

  列表和报告上的过滤器不支持此自定义字段类型。

  有关通过API访问此字段的信息，请参阅API中的[富文本字段存储](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md)。

  >[!NOTE]
  >
  >带格式的文本字段不适用于Workfront移动应用程序（在即将发布的版本中提供）。

* **描述性文本**：允许您包含说明和指向Workfront外部页面的链接。

+++

要添加文本字段，请执行以下操作：

1. 在屏幕左侧的&#x200B;**新字段**&#x200B;选项卡中，找到以下文本字段之一，并将其拖动到画布上的某个部分：

   * 单行文本
   * 段落
   * 带格式文本
   * 描述性文本

   ![将字段拖到节](assets/drag-field-to-section.png)

1. 在屏幕右侧，配置可用于要添加的自定义字段类型的选项：

   <table>
    <tr>
    <td>输入到</td>
    <td>描述</td>
    <td>可用于 </td>
    </tr>
    <tr>
    <td>大小</td>
    <td><p>（可选）更改表单中文本字段的大小。<p>
   </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    <li>带格式文本</li>
    <li>描述性文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>标签</td>
    <td><p>（必需）键入要在该字段上方显示的描述性标签。 您可以随时更改标签。<p>
    <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p></td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    <li>带格式文本</li>
    </ul></td>
    </tr>
    <tr>
     <td>名称</td>
    <td><p>（必需）此名称是系统标识字段的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p>
    <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p>
    </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    <li>带格式文本</li>
    <li>描述性文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>说明</td>
    <td>键入有关该字段的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。
    <img src="assets/instructions-form-designer.png">
    </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    <li>带格式文本</li>
    </ul></td>
    </tr>
    <tr>
    <td>格式化</td>
    <td><p>选择将在自定义字段中捕获的数据类型。</p> <p><b>注释</b>：   
    <ul> 
    <li>保存表单后无法编辑此字段。 如果要在数学计算中使用字段，请确保选择“数字”或“货币”格式。</li> 
    <li>选择“数字”或“货币”时，系统会自动截断以0开头的数字。</li>
    <li>数字字段的字符限制为16。 您还可以使用文本字段输入数字并避免限制。</li>
     </ul></p></td> </td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    </ul></td>
    </tr>
    <tr>
    <td>显示类型</td>
    <td>在单行文本字段和段落文本字段之间切换。</td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    </ul></td>
    </tr>
    <tr>
    <td>超链接</td>
    <td> 如果要将超链接应用于已键入的描述性文本，请在此处添加它。 描述性文本在附加表单的对象上显示为链接。</td>
    <td><ul><li>描述性文本</li></ul></td>
    </tr>
    <tr> 
      <td role="rowheader">设为必填字段</td>
      <td><p>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。</p></td>
    <td><ul>
    <li>单行文本</li>
    <li>段落</li>
    <li>带格式文本</li>
    </ul></td> 
    </tr> 
   </table>

1. （可选）重复上一步以添加任何其他字段或小组件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 添加计算字段

在自定义表单中，您可以添加计算自定义字段，该字段在自定义表单附加到对象时使用现有数据生成新数据。

要添加计算字段，请参阅[使用表单设计器添加计算字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。

### 添加单选按钮、复选框组和下拉列表

您可以将单选按钮、复选框组、下拉列表和多选下拉列表添加到自定义表单中。

+++ 展开以查看可用字段的描述。

* **单选按钮**：要求用户仅选择一个选项。
* **复选框组**：允许用户选择多个选项。
* **单选下拉列表**：提供下拉选项列表。
* **多选下拉列表**：允许用户从下拉列表中选择多个选项。

+++

>[!NOTE]
>
>允许进行多项选择的字段，例如复选框组和多项选择下拉列表，很难在报告中进行图表和分组。 为了更便于在报告中使用图表和进行分组，您可以为每个选择创建单独的字段（例如，单行文本字段）。

要添加单选按钮、复选框组和下拉列表，请执行以下操作：

1. 在屏幕左侧的&#x200B;**新字段**&#x200B;选项卡中，找到以下字段之一并将其拖动到画布上的某个部分：

   * 单选按钮
   * 复选框组
   * 单选下拉菜单
   * 多选下拉框

   ![将字段拖到画布上](assets/drag-field-to-section.png)

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
     <td> <p>（必需）键入要显示在自定义字段上方的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
     <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul></td>
     </tr> 
     <tr> 
    <td role="rowheader">名称</td> 
     <td> <p>（必需）此名称是系统标识字段的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p> 
    <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td>
     <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">说明</td> 
    <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> 
    <p>  <img src="assets/instructions-form-designer.png"> </p>
    </td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul></td>
    </tr> 
    <tr> 
    <td role="rowheader">格式化</td> 
    <td> <p>选择将在自定义字段中捕获的数据类型。</p> <p><b>注释</b>：   
     <ul> 
    <li>保存表单后无法编辑此字段。 如果要在数学计算中使用字段，请确保选择“数字”或“货币”格式。<br></li> 
    <li>选择“数字”或“货币”时，系统会自动截断以0开头的数字。</li>
    <li>数字字段的字符限制为16。 您还可以使用文本字段输入数字并避免限制。</li>
     </ul></p></td> 
     <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul></td>
    </tr> 
    <tr> 
     <td role="rowheader">显示类型</td> 
    <td>在字段的单选按钮、复选框组、单选下拉列表或多选下拉列表之间切换。</td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul></td>
    </tr> 
    <td role="rowheader">选项 </td> 
    <td> 
    <p>选择以下任一选项：</p> 
    <ul> 
    <li><strong>显示值</strong>：显示字段中每个选择的值。 默认情况下，将显示每个选项的标签。</li>
   <li><strong>选择排序A-Z</strong>：按字母顺序对您在字段中添加的选择进行排序。</li>
    </ul>
     <p>对于您为用户添加的每个选项，单击齿轮图标<img src="assets/gear-icon-settings.png">，然后选择以下选项之一：</p> 
    <ul> 
    <li><strong>默认选择</strong>：在字段中选择默认选择。</li> 
    <li> <p><strong>隐藏选择</strong>：隐藏字段中的选择。 隐藏选项在报表中仍可访问。</p> </li> 
    <li> <p><strong>删除选择</strong>：从字段中删除选择。</p> <p><b>警告</b>：如果当前对象使用此选项，请不要将其从字段中移除。 删除它将会导致历史数据丢失。 相反，选择选项可隐藏它，这会阻止用户将来选择它。</p> </li> 
    </ul>   
    <p><b>注意：</b>您可以选择的选项数量没有限制。 </p>    
    </td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul>
    </td>
     </tr> 
          <tr> 
    <td role="rowheader">设为必填字段</td> 
    <td>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。 </td> 
    <td><ul>
    <li>单选按钮</li>
    <li>复选框组</li>
    <li>单选下拉菜单</li>
    <li>多选下拉框</li>
    </ul></td>
     </tr> 
    <tr> 
    </tbody> 
    </table>

1. （可选）重复上一步以添加任何其他字段或小组件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 添加预输入和日期字段

您可以将预输入和日期字段添加到自定义表单。

+++ 展开以查看可用字段的描述。

* **提前键入**：允许用户键入Workfront中存在的对象的名称。 用户开始键入内容时，将显示建议列表。 此字段类型支持以下对象：
   * 用户
   * 组
   * 工作角色
   * 项目组合
   * 项目群
   * 项目
   * 团队
   * 模板
   * 公司
* **日期**：显示一个日历，用户可以在其中选择日期和时间。

+++

要添加预输入和日期字段，请执行以下操作：

1. 在屏幕左侧的&#x200B;**新字段**&#x200B;选项卡中，找到以下字段之一并将其拖动到画布上的某个部分。

   * 键盘缓冲
   * 日期

   ![将字段拖到节](assets/drag-field-to-section.png)

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
      <td> <p>（必需）键入要显示在自定义字段上方的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
       <td><ul>
    <li>键盘缓冲</li>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统标识字段的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p> 
      <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td>
    <td><ul>
    <li>键盘缓冲</li>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> 
      <p> <img src="assets/instructions-form-designer.png"> </p>
      </td> 
         <td><ul>
    <li>键盘缓冲</li>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">显示当日时间</td> 
      <td>如果要在字段中显示一天中的时间和日期，请选择此选项。</td> 
         <td><ul>
    <li>日期</li>
    </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">参考对象类型</td> 
      <td> <p>选择要与字段关联的对象类型。</p> <p>单击<b>应用</b>或<b>保存并关闭</b>后，无法更改该字段的对象类型。</p> <p><b>注释</b>：   
        <ul> 
         <li>如果您的Workfront管理员在Workfront用户界面中为项目组合、程序或项目自定义了名称，则该对象的默认Workfront名称将显示在此下拉列表中，而不是自定义名称中。 如果您需要此方面的帮助，请咨询您的Workfront管理员。<br></li> 
         <li>iOS和Android Workfront Mobile应用程序支持以下对象类型：用户、公司、组、工作角色、Portfolio、项目、项目和模板。</li> 
        </ul> </p> </td> 
         <td><ul>
    <li>键盘缓冲</li>
    </ul></td>
     </tr>
     <tr>
      <td role="rowheader">添加筛选器</td>
      <td><p>为对象类型添加过滤器，以限制用户在使用该字段时可以选择的对象。 </p> <p>例如，您可以限制一个字段，这样只有当用户名满足以下条件时才可以选择用户名：</p> 
       <ul> 
        <li>它们属于您指定的一个或多个组。</li> 
        <li>它们与您指定的角色或职称相关联。</li> 
        <li>他们与使用字段的人属于同一组。</li> 
       </ul> <p>必须使用文本模式语法为所选对象类型定义过滤器。 有关使用文本模式创建过滤器的信息，请参阅<a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">使用文本模式编辑过滤器</a>。</p>
       <p><b>注释</b>：
       <ul> 
        <li>如果您正在编辑现有的自定义表单，则将过滤器添加到“预输入”字段不会移除用户已使用该字段添加的任何对象（在过滤器的范围外）。</li> 
        <li>此筛选器在移动设备上不可用。 如果您将过滤器用于“预输入”字段，则该字段将显示在不受过滤器影响的用户移动设备上。</li> 
        </ul></p></td> 
      <td>
       <ul>
       <li>键盘缓冲</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">设为必填字段</td> 
      <td>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。 </td> 
       <td><ul>
    <li>键盘缓冲</li>
    <li>日期</li>
    </ul></td>
     </tr> 
    </tbody> 
   </table>

1. （可选）重复上一步以添加任何其他字段或小组件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 添加外部查找字段

外部查找字段调用外部API，并在下拉字段中作为选项返回值。 使用自定义表单附加到的对象的用户可以从下拉列表中选择一个或多个选项。 列表和报告中也提供了“外部查找”字段。

有关使用外部查找字段调用同一Workfront实例或公共API的示例，请参阅[自定义表单中的外部查找字段示例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)。

>[!NOTE]
>
>* Outlook插件不支持外部查找字段。
>* 当外部查找字段依赖于另一个字段时，该字段在列表中不可用。

要添加外部查找，请执行以下操作：

1. 在屏幕左侧的&#x200B;**新字段**&#x200B;选项卡中，找到&#x200B;**外部查找**&#x200B;并将其拖动到画布上的某个部分。
1. 在屏幕右侧，配置自定义字段的选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要显示在自定义字段上方的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统标识字段的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够选择更改用户看到的标签，而不必更改系统看到的名称。</p>
      <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td>
     </tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关自定义字段的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">格式化</td>
      <td><p>选择将在自定义字段中捕获的数据类型。</p>
      <p><strong>注意：</strong></p>
      <ul><li>保存表单后，可以更改格式类型，但有一个限制：对象上的所有现有值都必须能够转换为新类型。 （例如，如果格式类型为“文本”，并且对象正在存储“abc”值，则您无法转换该字段，并且会收到一个错误，说明系统无法将“abc”转换为数字/货币。） 如果要在数学计算中使用字段，请确保选择“数字”或“货币”格式。</li>
      <li>选择“数字”或“货币”时，系统会自动截断以0开头的数字。</li>
      <li>数字字段的字符限制为16。 您还可以使用文本字段输入数字并避免限制。</li>
      </ul></td>
     </tr> 
     <tr> 
      <td role="rowheader">基本 API URL</td> 
      <td><p>键入或粘贴API的URL。</p><p>API URL必须返回要在下拉列表中显示的选项的JSON内容。 您可以使用JSON路径字段从返回的JSON中选择特定值作为下拉选项。</p><p>输入API URL时，您可以选择在URL中传递以下值：</p>
      <ul>
      <li>$$HOST — 表示当前Workfront主机，可用于对Workfront API进行/搜索API调用。 使用此通配符时，将处理身份验证，用户无需发送身份验证标头。 （例如，用户可以使用基本URL <code>$$HOST/attask/api/task/search</code>搜索任务，它将允许搜索任务并从返回的任务列表中选择值。）</li>
      <li><p>$$QUERY — 这表示最终用户在字段中键入的搜索文本，并允许您为最终用户实施查询筛选。 （用户将在下拉列表中搜索值。）</p>
      <p>如果所引用的API允许这样做，则还可以在搜索查询中包含修饰符以标识搜索应如何工作。 例如，您可以使用以下内容作为基本API URL，以允许人员搜索包含特定文本的任何Workfront项目： <code>$$HOST/attask/api/v15.0/proj/search?name=$$QUERY&name_Mod=contains</code>。</p><p>在<a href="/help/quicksilver/wf-api/general/api-basics.md">API基础知识</a>中了解有关Workfront搜索修饰符的更多信息。</p>
      <p><strong>注意：</strong>如果您未使用$$QUERY，并且搜索框中的用户类型文本会缩小您现有的选择范围。 但是，如果您使用$$QUERY并且用户键入了任何内容，则会对您的API执行新的网络调用。 因此，如果您的API中有超过2000个值，并且该API支持查询，则您可以利用$$QUERY不仅从现有2000个值中进行搜索，还可以从具有缩小选项的原始API中进行搜索。</p></li>
      <li><p>{fieldName} — 其中fieldName是Workfront中的任何自定义或本机字段。 这样，在将已选字段的值传递到外部查找字段以筛选下拉选项时，您可以实施级联下拉选项过滤器。 （例如，表单上已存在区域字段，并且您正在将国家/地区列表从API缩小到特定区域的国家/地区。）</p>
      <p>对于依赖其他字段的外部查找字段（使用{fieldName}语法），从API返回的选项仅限于匹配在其他字段中输入的任何字符串或值的选项。 （列表和报告不支持此功能。）</p></li>
      <li>{referenceObject}。{fieldName} — 其中字段是对象的一部分。 此语法类似于自定义表达式。 (例如，portfolioID={project}。{portfolioID})</li></ul>
      <p><strong>提示：</strong>查看文档以了解您正在使用的API，以便获取您可以定义的特定查询。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">HTTP 方法</td> 
      <td>为方法选择<strong>Get</strong>、<strong>Post</strong>或<strong>Put</strong>。</td> 
     </tr>
     <tr> 
      <td role="rowheader">JSON 路径</td>
      <td><p>键入或粘贴API的JSON路径。</p> <p>此选项允许从API URL返回的JSON中提取数据。 它提供了一种方法，用于选择在JSON内的哪些值将显示在下拉选项中。</p><p>例如，如果API URL按以下格式返回JSON，则可以使用“$.data[*].name”选择“美国”和“加拿大”作为下拉选项：</br>
      <pre>
      {
       数据： {
         { name： "USA"}，
         { name： "Canada"}
       }
      }
      </pre>
      </p>
     <p>有关JSON路径并确保编写正确JSON路径的更多信息，请参阅<a href="https://jsonpath.com/">https://jsonpath.com/</a>。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">标头</td>
      <td><p>单击<strong>添加标头</strong>，然后键入或粘贴使用API进行身份验证所需的密钥值对。</p><p><strong>注意：</strong>标头字段不是存储凭据的安全位置，您应该小心输入和保存的内容。</p></td>
     </tr>
     <tr> 
      <td role="rowheader">多选下拉框</td>
      <td><p>选择此选项可允许用户在下拉列表中选择多个值。</p></td>
     </tr>
     </tr>
     <tr> 
      <td role="rowheader">设为必填字段</td>
      <td><p>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。</p></td>
     </tr>       
    </tbody>
   </table>

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

>[!NOTE]
>
>以下项目是对外部API调用的技术限制：
>
>* 最大选项数：2000（仅显示返回的JSON中的前2000个唯一选项）
>* 超时：30秒
>* 重试次数：3
>* 重试之间的等待持续时间：500毫秒
>* 预期响应状态： 2xx

### 添加图像、PDF和视频

您可以将图像、PDF和视频添加到自定义表单。 使用附加到自定义表单的对象的用户只能在以下区域查看图像、PDF或视频：

* 对象的“详细信息”区域（例如，对于项目，“项目详细信息”区域）。
* 对象的“编辑”框(如果它具有新的Adobe Workfront Experience外观)（例如，“编辑项目”和“编辑任务”框）。

<!-- Do we need to tell them where they can't see it if we tell them where they can see it?
Currently, users cannot see the widget in the following areas:​
Lists and reports
Home and Summary
The Edit box for the object, if it doesn't have the new Adobe Workfront experience look and feel (for example, the Edit Expense box)
The Workfront Mobile app -->

+++ 展开以查看可用字段的描述。

* **图像**：允许用户添加图像文件。
* **PDF**：允许用户添加PDF
* **视频**：允许用户添加视频文件。

+++

要添加图像、PDF或视频，请执行以下操作：

1. 在屏幕左侧的&#x200B;**新字段**&#x200B;选项卡中，找到以下字段之一并将其拖动到画布上的某个部分。

   * 图像
   * PDF
   * 视频

   ![将字段拖到节](assets/drag-field-to-section.png)

1. 键入或编辑构件的以下任意属性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改构件的显示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在小部件上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统标识构件的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p> <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴构件存储在Internet上的URL。</p> 
      <p>如果要添加视频构件，当前可通过在URL框中添加以下内容来实现此目的：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo链接</p> </li> 
      <li> <p>Google Drive视频链接</p> </li> 
      <li> <p>视频链接，带有MP4和MOV扩展</p> </li> 
      <li> <p>视频链接已上传到Workfront实例中的文档区域。 有关说明，请参阅本文中的“文档”区域</a>中的<a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">将视频小组件添加到自定义表单。</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关构件的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复上一步以添加任何其他字段或小组件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

#### 从文档区域将视频添加到自定义表单{#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以这种方式将视频添加到自定义表单时，当用户访问对象上的表单时，“文档”区域中设置的权限将应用于视频。

1. 转到“文档”区域中的视频并为其生成验证，如[为网站或其他Web内容创建交互式验证](/help/quicksilver/review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md)中所述。
1. 打开证明。
1. 右键单击视频上的任意位置，然后选择&#x200B;**复制视频地址**。
1. 在您添加视频小部件的自定义表单中，将复制的地址粘贴到&#x200B;**URL**&#x200B;框中。
1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 添加Workfront本机字段

您可以将Workfront原生字段添加到自定义表单。 将自定义表单附加到对象时，会从对象数据填充字段。 例如，附加到项目的自定义表单上的描述字段将拉入项目描述。 （如果没有可用数据，则字段可能显示“不适用”。）

+++ 展开以查看支持的本机字段列表。

此表列出了自定义表单中特定Workfront对象的可用本机字段。

| 字段名称 | 项目 | 任务 | 问题 | 模板 | 模板任务 | 项目组合 | 项目群 | 组 |
|--------------------------- |-------- |------- |------- |--------- |-------------- | --------- |-------- |------ |
| 实际完成日期 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 实际持续时间 | ✓ |   |   |   |   |   |   |   |
| 实际小时数 | ✓ |   | ✓ |   |   |   |   |   |
| 实际开始日期 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 公司 | ✓ |   |   | ✓ |   |   |   |   |
| 完成情况 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 完成情况类型 | ✓ |   |   | ✓ |   |   |   |   |
| 描述 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| 持续时间 |   | ✓ |   |   | ✓ |   |   |   |
| 持续时间类型 |   | ✓ |   |   | ✓ |   |   |   |
| 持续时间单位 |   | ✓ |   |   | ✓ |   |   |   |
| 输入者 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| 输入日期 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   | ✓ |
| 组 | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| 上次更新者 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 上次更新日期 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 名称 | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| 所有者 | ✓ |   |   | ✓ |   | ✓ | ✓ |   |
| 规划完成日期 | ✓ | ✓ | ✓ |   |   |   |   |   |
| 计划持续时间 | ✓ |   |   | ✓ |   |   |   |   |
| 规划小时数 | ✓ | ✓ | ✓ |   | ✓ |   |   |   |
| 计划开始日期 | ✓ |   |   |   |   |   |   |   |
| 项目组合 | ✓ |   |   | ✓ |   |   | ✓ |   |
| 优先级 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 项目群 | ✓ |   |   | ✓ |   |   |   |   |
| 预计完成日期 | ✓ | ✓ |   |   |   |   |   |   |
| 预计持续时间分钟数 |   | ✓ |   |   |   |   |   |   |
| 预计开始日期 | ✓ | ✓ |   |   |   |   |   |   |
| 参考号 | ✓ | ✓ | ✓ | ✓ | ✓ |   |   |   |
| 计划模式 | ✓ |   |   | ✓ |   |   |   |   |
| 严重性 |   |   | ✓ |   |   |   |   |   |
| 发起人 | ✓ |   |   | ✓ |   |   |   |   |
| 状态 | ✓ | ✓ |   |   |   |   |   |   |
| 故事点数 |   | ✓ |   |   |   |   |   |   |
| 模板 | ✓ |   |   |   |   |   |   |   |
| URL | ✓ | ✓ |   | ✓ | ✓ |   |   |   |

{style="table-layout:auto"}

+++

1. 在屏幕左侧的&#x200B;**新建字段**&#x200B;选项卡中，找到&#x200B;**本机字段引用**，并将其拖动到画布上的部分。
1. 在屏幕右侧，配置自定义字段的选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改字段的显示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在该字段上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td>
      <td> <p>（必需）此名称是系统标识字段的方式。 当您首次配置字段并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p>
      <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关该字段的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">参考字段</td> 
      <td><p>（必需）选择Workfront原生字段。<p><p>仅表单对象的本机字段可用。 例如，如果表单设计器顶部的“对象类型”列表显示“项目”，则您将能够选择项目的本机字段，但不能选择特定于任务的字段。</p></td>
     </tr>
     <tr>
      <td role="rowheader">添加筛选器</td>
      <td><p>为参考字段添加过滤器，以限制用户在使用字段时可以选择的项目列表。 </p> <p>例如，您可以限制一个字段，这样只有当用户名满足以下条件时才可以选择用户名：</p> 
       <ul>
        <li>它们属于您指定的一个或多个组。</li> 
        <li>它们与您指定的角色或职称相关联。</li> 
        <li>他们与使用字段的人属于同一组。</li> 
       </ul>
       <p>必须使用文本模式语法为所选的引用字段定义过滤器。 有关信息，请参阅<a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md">使用文本模式编辑筛选器</a>。</p>
       <p><b>注释</b>：
       <ul> 
        <li>仅当您引用本机预输入字段(如“Portfolio”、“公司”或“所有者”)时，过滤器选项才可用。</li>
        <li>如果您正在编辑现有的自定义表单，将过滤器添加到本机字段不会移除用户已使用该字段添加的任何对象（在过滤器的范围外）。</li> 
        <li>此筛选器在移动设备上不可用。 如果您将过滤器用于本机字段，则该字段将显示在不受过滤器影响的用户移动设备上。</li> 
        </ul></p></td> 
      <td>
     </tr>
     <tr> 
      <td role="rowheader">设为必填字段</td>
      <td><p>如果希望该字段是用户完成自定义表单所必需的，请选择此选项。</p></td>
     </tr> 
    </tbody> 
   </table>

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 添加Adobe XD文件

您可以将Adobe XD原型直接添加到自定义表单。 使用附加到自定义表单的对象的用户只能在以下区域查看Adobe XD文件：

* 对象的“详细信息”区域（例如，对于项目，“项目详细信息”区域）
* 对象的“编辑”框(如果它具有新的Adobe Workfront Experience外观)（例如，“编辑项目”和“编辑任务”框）

添加Adobe XD文件：

1. 在屏幕左侧的&#x200B;**新字段**&#x200B;选项卡中，找到&#x200B;**Adobe XD**&#x200B;并将其拖动到画布上的某个部分。
1. 键入或编辑构件的以下任意属性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
         <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改构件的显示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在小部件上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>：请避免在此标签中使用特殊字符，因为这些字符在报表中无法正确显示。 有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统标识构件的方式。 首次配置构件并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p>
    <p>有关详细信息，请参阅<a href="design-a-form.md#notes-on-field-names-and-labels">有关字段名称和标签的注释</a>。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴有效的XD原型链接。</p> 
      <p><b>注意</b>： Adobe XD中“共享”选项卡上的“链接访问”设置必须设置为具有链接的任何人。 否则，用户将无法查看原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关构件的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。
    <img src="assets/instructions-form-designer.png"></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）重复上一步以添加任何其他字段或小组件。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

### 添加Planning连接字段

>[!IMPORTANT]
>
>本节中的信息介绍了Adobe Workfront Planning，它是Adobe Workfront的一项附加功能。
>
>要访问Workfront Planning，您必须具备以下条件：
>
>* 新的Workfront计划和许可证。 Workfront Planning不适用于旧版Workfront计划或许可证。
>* Workfront Planning的附加包。
>* 您组织的Workfront实例必须载入到Adobe Unified Experience。
>
> 有关访问Workfront Planning的完整要求列表，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。
> 
>有关Workfront Planning的更多信息，请参阅[Adobe Workfront Planning概述](/help/quicksilver/planning/general/planning-overview.md)。

通过将Workfront连接自定义字段添加到对象的自定义表单，您可以在Workfront对象的自定义字段中查看从Planning连接的记录。

可将Planning连接字段添加到所有对象的自定义表单中。 但是，您只能在与Workfront对象(可从Workfront Planning连接)关联的自定义表单上显示连接的记录。

>[!NOTE]
>
>在自定义字段中查看信息的用户必须有权访问Workfront Planning，并且有权访问包含连接到Workfront对象的记录类型的工作区。

要添加Planning连接字段：

1. 在屏幕左侧的&#x200B;**新建字段**&#x200B;选项卡中，找到&#x200B;**Planning连接**，并将其拖动到画布上的某个部分。
1. 在屏幕右侧，配置自定义字段的选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改构件的显示大小。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在该字段上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要提示</b>：请避免在此标签中使用特殊字符。</p> 
      <p>我们建议您选择一个帮助您轻松识别Planning记录来源的标签。 添加诸如工作区名称或记录类型名称之类的信息。 </p>   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td>
      <td> <p>（必需）名称是系统标识字段的方式。 当您首次配置字段并键入标签时，会自动填充名称字段以匹配它。 “标签”和“名称”字段不同步。 这样，您就可以选择更改用户看到的标签，而不必更改系统看到的名称。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>（推荐）键入有关字段的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p>
      <p>在这里，您可以添加有关记录和所连接对象的详细信息。 </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">对象类型</td> 
      <td><p>（必需）选择连接到Workfront Planning中的记录类型的Workfront对象类型。</p>
      您可以从以下对象类型中进行选择：
      <ul><li> 项目</li>
      <li> 项目组合</li><li> 项目群</li><li> 公司</li><li> 组</li></ul>
       <p>只有表单对象类型的Workfront对象类型可用。</p> <p> 例如，如果表单设计器顶部的“对象类型”列表显示“项目”，则只能在此字段中选择“项目”，而不能选择“项目组合”，尽管项目组合也可以连接到记录类型。</p>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">Workspace</td> 
      <td> <p>（必需）选择您要在Workfront中显示的记录来自的Planning工作区。</p> <p> 只有连接到您在“对象类型”字段中选择的对象类型的工作区才会显示。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">记录类型</td> 
      <td><p>（必需）选择与Workfront对象类型相关的Workfront Planning记录类型。</p><p>只显示与您在对象类型字段中选择的对象类型有连接的记录类型。 </p></td> 
     </tr>
     <tr> 
      <td role="rowheader">连接字段</td> 
      <td><p>（必需）选择要在Workfront对象上显示的选定Planning记录类型与Workfront对象类型之间的连接字段。 </p> <p> <b>注意</b>：同一对象和记录类型之间可以有多个连接字段，但只能选择一个字段。</p>  </td> 
     </tr>

<tr> 
      <td role="rowheader">记录类型字段</td> 
      <td><p>（可选）从连接的记录类型中选择最多7个查找字段以在自定义表单中显示。 默认情况下，主字段处于选中状态，无法编辑。 </p> <p> 您选择的已连接记录的字段显示在自定义表单的表视图中。 将表单附加到Workfront对象时，表格视图为只读。 </p>  
    <img src="assets/planning-connections-field-with-table-on-form-preview.png"></td> 
     </tr>
      </tbody> 
   </table>

1. （可选）重复上述步骤以添加任何其他字段。

   或

   要复制字段，请将鼠标悬停在字段上，然后单击复制图标。

   ![复制图标](assets/copy-field.png)

1. 要保存更改，请单击&#x200B;**应用**，然后转到其他部分以继续构建表单。

   或

   单击&#x200B;**保存并关闭**。

   您现在可以将表单附加到从Workfront Planning连接的对象，并执行以下操作之一：

   * 查看连接到Workfront对象的Workfront Planning记录类型（如果有）。
   * 从Workfront对象连接或断开记录。

   有关详细信息，请参阅[管理来自Workfront对象的记录连接](/help/quicksilver/planning/records/manage-records-in-planning-section.md)

## 使用表单设计器组织和预览表单

有关如何组织带有分区界限的自定义表单并查看表单预览的信息，请参阅[使用表单设计器组织和预览表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。



