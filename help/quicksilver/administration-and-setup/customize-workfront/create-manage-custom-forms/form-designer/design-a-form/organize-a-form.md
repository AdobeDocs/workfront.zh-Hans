---
title: 使用表单设计器组织和预览表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单设计器组织自定义表单。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 6e06e7892542c7dd96b6bf8b857583333efc883d
workflow-type: tm+mt
source-wordcount: '1107'
ht-degree: 0%

---


# 使用表单设计器组织和预览表单

您可以使用表单设计器组织自定义表单。

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
   <p>旧版计划：计划</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>对自定义表单的管理访问权限</p> <p>有关Workfront管理员如何授予此访问权限的信息，请参阅 <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">授予用户对特定区域的管理访问权限</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## 添加节分符

您可以将自定义表单中的自定义字段和小组件分组为包含标题的部分。 这对于向填写表单的用户展示有组织的体验非常有用。 此外，如果您需要限制特定用户对特定自定义字段和小组件的访问权限，则可以将这些字段和小组件放置在某个部分中，然后仅向这些用户授予对该部分的访问权限。

例如，如果您需要跟踪只有系统管理员才能查看或编辑的敏感信息，则可以创建具有“仅管理员”权限的分区，并将敏感字段放在该分区中。

您为部分选择的访问设置会直接绑定到用户在附加了自定义表单的Workfront对象上拥有的权限。 您可以根据用户是否有权查看、贡献或管理该对象来隐藏或显示部分。 或者，您也可以将部分设置为“仅管理员”，以便只有具有系统管理员访问权限级别的用户才能访问该部分。

有关对象权限的信息，请参阅 [对象共享权限概述](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

有关自定义表单中的自定义字段和小组件的信息，请参阅 [设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### 在自定义表单中创建和配置对部分的访问权限

1. 开始创建或编辑自定义表单和添加字段，如 [设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 单击 **区域划分** 并将其拖到画布上的所需位置。

1. 在右侧面板中，配置所需部分的选项：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在部分上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>:避免在此标签中使用特殊字符。 无法在报表中正确显示它们。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>如果要向用户说明该部分的用途，请键入文本。 它显示在自定义表单上区域标签的下方。</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>授予访问权限</p> </td> 
      <td> <p> 选择用户对附加了自定义表单的对象所需的权限，以查看此部分并编辑其字段值。 
       <p>以下权限位于 <b>具有此对象访问权限的用户可以查看字段值</b>:</p> 
         <ul>  
          <li><p><b>有限编辑</b>:（仅当对象是项目、任务、问题或用户时才可用）：</p> 
          <p>允许用户在对象是项目、任务或问题时对对象进行投稿。</p>
          <p>允许用户编辑配置文件或拥有对象（如果用户）的配置文件权限。</p></li> 
          <li><b>编辑</b>:管理对象的权限 </li> 
          <li><b>仅管理员</b>:系统管理员访问级别</li> 
         </ul> </li> 
        <p>以下权限位于 <b>具有此对象访问权限的用户可以编辑字段值</b>: </p> 
         <ul> 
          <li> <p><b>有限编辑</b>:（仅当对象是项目、任务、问题或用户时才可用）：</p> 
           <p>如果对象是项目、任务或问题，则此权限允许用户对该对象进行贡献</p>
          <p>如果对象是用户，则此权限允许用户编辑配置文件或拥有该对象的配置文件权限。</p> 
          <li><b>编辑</b>:管理对象的权限 </li> 
          <li><b>仅管理员</b>:系统管理员访问级别</li> 
         </ul> </li> 
       </ul> 
       <p>有关对象权限的信息，请参阅 <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象共享权限概述</a>.</p> 
       <p><b>注释</b>:  
       <ul> 
       <li> <p>没有此处指定权限的用户在部分中看不到自定义字段和小组件。 </p> <p>如果您在报表中显示字段值或在文本模式报表中的计算字段中使用这些值，则也会出现这种情况。</p> </li> 
       <li> <p>将多个对象类型与您的表单关联，可能会更改这些步骤中提供的查看和编辑权限。 有关更多信息，请参阅 <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">在自定义表单中，多个对象类型如何影响节点划分权限</a> 在本文中。</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 将至少一个自定义字段或小组件拖放或添加到新部分。 在保存部分之前，需要执行此操作。

1. 单击 **完成**.

   >[!TIP]
   >
   >您可以单击 **应用** 创建自定义表单以保存所做更改并保持表单打开时，随时可以执行此操作。

### 多种对象类型如何影响节划分权限 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

自定义表单部分中断的“有限编辑”权限仅适用于项目、任务、问题和用户对象类型。

在自定义表单中，如果向表单添加其他对象类型(“Portfolio”、“程序”、“文档”、“公司”、“帐单记录”、“小版本”、“费用”或“组”)，则系统会提示您切换到“编辑”权限，该权限与表单上该对象类型和现有对象类型都兼容。

>[!INFO]
>
>**示例：** 在与项目对象类型关联的自定义表单中，会使用“有限编辑”权限配置节断点。
>
>您将Portfolio对象类型添加到表单中，这意味着“有限编辑”权限选项不再可用于表单中的部分中断。
>
>屏幕上的消息会提示您切换到“编辑”权限，该权限是与“项目”对象类型和“Portfolio”对象类型兼容的最低级别权限。


## 在自定义表单中放置自定义字段和小组件


1. 开始创建或编辑自定义表单，如 [设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 要将自定义字段和小组件放置在同一行上，请将一个字段和小组件拖动到另一行旁边，直到它们之间出现一条线。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 您可以使用 **预览** 按钮，以了解自定义字段和小组件在表单中的显示方式。
>* 自定义字段和小组件在表单中的显示方式可能并不总是相同，具体取决于用户查看时屏幕空间的可用程度。 例如，如果水平空间有限，一行字段中的第三个字段可能会换到下一行字段。


1. （可选）要将自定义字段或小组件置于另一个字段或小组件上方或下方，请将其拖动到上方或下方，直到项目之间出现水平蓝线。

1. 要保存更改，请单击 **应用**

   或

   单击 **保存并关闭**.

## 预览自定义表单

1. 开始创建或编辑自定义表单和添加字段，如 [设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. 单击 **预览** 查看使用表单时的外观，然后单击 **结束预览** 以返回编辑表单。