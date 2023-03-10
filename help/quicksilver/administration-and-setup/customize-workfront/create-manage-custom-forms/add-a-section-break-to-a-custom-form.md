---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 使用旧版表单生成器向自定义表单添加分区界限
description: 您可以将自定义表单中的自定义字段和小组件分组到具有标题的部分。 这对于向将填写表单的用户展示组织好的体验非常有用。 此外，如果您需要限制特定用户访问某些自定义字段和小部件，您可以将它们放在分区中，然后仅向这些用户授予对分区的访问权限。
feature: System Setup and Administration
role: Admin
exl-id: 44a52767-60a7-4aaa-b3b8-6b8fb7da7e72
source-git-commit: e02e28d9a62a6bafbe19de7e6fda043b56210cf7
workflow-type: tm+mt
source-wordcount: '1131'
ht-degree: 0%

---

# 使用旧版表单生成器向自定义表单添加分区界限

您可以将自定义表单中的自定义字段和小组件分组到具有标题的部分。 这对于向将填写表单的用户展示组织好的体验非常有用。 此外，如果您需要限制特定用户访问某些自定义字段和小部件，您可以将它们放在分区中，然后仅向这些用户授予对分区的访问权限。

例如，如果您需要跟踪只有系统管理员才能查看或编辑的敏感信息，则可以使用“仅限管理员”权限创建分区界限，并将敏感字段放置在该分区中。

您为部分选择的访问设置直接绑定到用户在附加自定义表单的Workfront对象上拥有的权限。 您可以根据用户是否具有查看、参与或管理该对象的权限来隐藏或显示部分。 或者，您也可以将部分设置为“仅管理员”，以便只有具有系统管理员访问权限级别的用户才能访问它。

有关对象权限的信息，请参见 [对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

有关自定义表单中的自定义字段和小部件的信息，请参阅 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

<!--
>[!TIP]
>
>Section breaks that you add to custom forms are saved in your system for re-use. For information about listing them, see [List and edit custom forms and widgets added to custom forms](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/list-edit-share-custom-forms-and-custom-fields.md).
-->

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

## 为自定义表单中的部分创建和配置访问权限

1. 开始创建或编辑自定义表单，如中所述 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 向表单中添加自定义字段和小部件，如中所述 [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) 和 [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

1. 仍创建或编辑自定义表单时，在 **添加字段** 选项卡，单击 **分节符**.

   ![](assets/click-section-break.jpg)

1. 在 **字段设置** 选项卡，为部分配置所需的选项：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要显示在部分上方的描述性标签。 您可以随时更改标签。</p> <p><b>重要</b>：避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>如果要向用户说明此部分的用途，请键入文本。 显示在自定义表单上部分的标签下方。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">添加逻辑</td> 
      <td>根据用户在填写表单时在多选自定义字段中做出的选择，使用显示逻辑指定节是否应显示在表单上。 有关更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">将显示逻辑和跳过逻辑添加到自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>授予访问权限</p> </td> 
      <td> <p> 选择用户在附加自定义表单的对象上所需的权限，以便查看此分区并编辑其字段值。 
       <p>以下权限位于 <b>具有该对象访问权限的用户可以查看字段值</b>：</p> 
         <ul>  
          <li><p><b>有限编辑</b>：（仅当对象是项目、任务、问题或用户时才可用）：</p> 
          <p>允许用户在对象是项目、任务或问题时，向对象投稿。</p>
          <p>如果用户是用户，则允许用户编辑配置文件或拥有对象的配置文件权限。</p></li> 
          <li><b>编辑</b>：管理对象的权限 </li> 
          <li><b>仅管理员</b>：系统管理员访问级别</li> 
         </ul> </li> 
        <p>以下权限位于 <b>具有该对象访问权限的用户可以编辑字段值</b>： </p> 
         <ul> 
          <li> <p><b>有限编辑</b>：（仅当对象是项目、任务、问题或用户时才可用）：</p> 
           <p>如果对象是项目、任务或问题，则此权限允许用户向对象投稿</p>
          <p>如果对象是用户，则此权限允许用户编辑配置文件或拥有对该对象的配置文件权限。</p> 
          <li><b>编辑</b>：管理对象的权限 </li> 
          <li><b>仅管理员</b>：系统管理员访问级别</li> 
         </ul> </li> 
       </ul> 
       <p>有关对象权限的信息，请参见 <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象权限共享概述</a>.</p> 
       <p><b>注释</b>:  
       <ul> 
       <li> <p>没有您在此处指定的权限的用户看不到部分中的自定义字段和小部件。 </p> <p>如果您在报表中显示字段的值，或在文本模式报表的计算字段中使用这些值，则也会出现这种情况。</p> </li> 
       <li> <p>将多个对象类型与表单关联可以更改这些步骤中可用的查看和编辑权限。 有关更多信息，请参阅 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">多个对象类型如何影响自定义表单中的分区界限权限</a> 本文章中。</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 将至少一个自定义字段或构件拖动或添加到新分区。

   在保存节之前需要此项。

1. 单击 **完成**.

   >[!TIP]
   >
   >您可以单击 **应用** 创建自定义表单时，可随时保存更改并保持表单打开。

1. 如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [在自定义表单中添加或编辑资源小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [将显示逻辑和跳过逻辑添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

<!--
DRAFTED IN FLARE:
<h2>Configure access for fields without section breaks</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">************This section might get added later. Team decided not to implement.</p>
<p>In a custom form, you can also control users' access to custom fields
and image widgets that are not placed inside a defined section.</p>
<ol>
<li value="1">Begin creating or editing a custom form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Create or edit a custom form</a>.</li>
<li value="2">Add custom fields

and widgets

to the form, as described in <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md" class="MCXref xref">Add a custom field to a custom form</a>.</li>
<li value="3"> <p>While still creating or editing the custom form, open the <b>Form settings</b> tab.</p> <p>SHOW THIS </p> </li>
<li value="4"> <p>Under <b>Grant access</b>, configure the permissions that users need on an object where the custom form is attached, in order to view and edit values in fields not placed under a section break. </p> <p>If you need information about permissions on objects, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overview of sharing permissions on objects</a>.</p> <note type="note">
<ul>
<li> <p>Users without the permissions you specify here can't see the values of the fields
and image widgets that are not placed in a defined section in the custom form. This is also true if you display the values in reports or use them in calculated fields in text mode reporting.</p> </li>
<li> <p>Associating multiple object types with your form can change the viewing and editing permissions that are available in these steps. For more information, see <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">How multiple object types can affect section break permissions in a custom form</a> in this article.</p> </li>
</ul>
</note>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader"><b>Users with this access to the object can view field values</b> </td>
<td>
<ul>  
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
<tr>
<td role="rowheader">Users with this access to the object can edit field values</td>
<td>
<ul>
<li> <p><b>Limited Edit</b>: (Available only if the object is a project, task, issue, or user):</p>
<ul>
<li> <p>Contribute permission to the object if it's a project, task, or issue</p> </li>
<li> <p>Edit the profile or own the profile permission to the object if it's a user (profile)</p> </li>
</ul> </li>
<li><b>Edit</b>: Manage permissions to the object </li>
<li><b>Admin only</b>: System Administrator access level</li>
</ul> </td>
</tr>
</tbody>
</table> </li>
<li value="5"> <p>Click Done.</p> <note type="tip">
You can click
<strong>Apply</strong> at any point while you are creating a custom form to save your changes and keep the form open.
</note> </li>
<li value="6"> <p>If you want to continue building your custom form in other ways, continue on to one of the following articles:</p>
<ul>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2" class="MCXref xref">Add a custom field to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md" class="MCXref xref">Add or edit an asset widget in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Add calculated data to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md" class="MCXref xref">Position custom fields and widgets in a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a> </li>
<li><a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md" class="MCXref xref">Preview and complete a custom form</a> </li>
</ul> </li>
</ol>
</div>
-->

## 多个对象类型如何影响分区界限权限 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

自定义表单分区界限的“有限编辑”权限仅适用于“项目”、“任务”、“问题”和“用户”对象类型。

在具有“有限编辑”权限的分区界限的自定义表单中，如果您将其他对象类型(Portfolio、程序、文档、公司、账单记录、小版本、费用或组)之一添加到表单，系统将提示您切换到“编辑”权限，该权限与该对象类型和表单上的现有对象类型都兼容。

>[!INFO]
>
>**示例：** 在与项目对象类型关联的自定义表单中，分区界限配置有有限的编辑权限。
>
>将Portfolio对象类型添加到表单，这意味着有限编辑权限选项不再可用于表单中的分区界限。
>
>屏幕上的消息会提示您切换到“编辑”权限，这是与“受限编辑”最相似的选项，并且与“项目”对象类型和“Portfolio”对象类型都兼容。
