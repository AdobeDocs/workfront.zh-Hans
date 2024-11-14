---
title: 组织和预览表单
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 您可以使用表单Designer来组织自定义表单。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 400ca2ac10a94ccfa79bef8daf06b924dadac230
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 0%

---

# 组织和预览表单

{{preview-fast-release-general}}

您可以使用表单设计器组织自定义表单，并预览该表单以验证设置是否正确。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

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

## 添加分区界限

您可以将自定义表单中的自定义字段和小组件分组到具有标题的部分。 这对于向将填写表单的用户展示组织好的体验非常有用。 此外，如果您需要限制特定用户访问某些自定义字段和小部件，则可以将这些字段和小部件放入分区，然后仅向这些用户授予对分区的访问权限。

例如，如果您需要跟踪只有系统管理员才能查看或编辑的敏感信息，则可以使用“仅限管理员”权限创建分区界限，并将敏感字段放置在该分区中。

为部分选择的访问设置直接与用户在附加自定义表单的Workfront对象上拥有的权限相关联。 您可以根据用户是否具有查看、参与或管理该对象的权限来隐藏或显示部分。 或者，您也可以将部分设置为“仅管理员”，以便只有具有系统管理员访问权限级别的用户才能访问它。

有关对象权限的信息，请参阅[对象权限共享概述](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

有关自定义表单中的自定义字段和小部件的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

### 创建和配置自定义表单中分区的访问权限

1. 开始创建或编辑自定义表单并添加字段，如[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)中所述。

1. 单击&#x200B;**分区界限**&#x200B;并将其拖动到画布上的所需位置。

1. 在右侧面板中，为部分配置所需的选项：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在该部分上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要提示</b>：请避免在此标签中使用特殊字符。 它们在报表中无法正确显示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>如果要向用户说明此部分的用途，请键入文本。 这会显示在自定义表单上部分的标签下方。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>授予访问权限</p> </td> 
      <td> <p> 选择用户在附加自定义表单的对象上所需的权限，以便查看此分区并编辑其字段值。 
       <p>以下权限在<b>下可用：具有对象访问权限的用户可以查看字段值</b>：</p> 
         <ul>
          <li><strong>查看</strong>：查看对象的权限</li>
          <li><p><b>有限的编辑</b>： （仅当对象是项目、任务、问题或用户时才可用）：</p> 
          <p>允许用户在对象是项目、任务或问题时，向该对象投稿。</p>
          <p>如果用户是用户，则允许用户编辑配置文件或拥有对象的配置文件权限。</p></li> 
          <li><b>编辑</b>：管理对象的权限 </li> 
          <li><b>仅限管理员</b>：系统管理员访问级别</li> 
         </ul> </li> 
        <p>在<b>下有以下权限可用。具有对象访问权限的用户可以编辑字段值</b>： </p> 
         <ul> 
          <li> <p><b>有限的编辑</b>： （仅当对象是项目、任务、问题或用户时才可用）：</p> 
           <p>如果对象是项目、任务或问题，则此权限允许用户向对象投稿</p>
          <p>如果对象是用户，则此权限允许用户编辑配置文件或拥有对该对象的配置文件权限。</p> 
          <li><b>编辑</b>：管理对象的权限 </li> 
          <li><b>仅限管理员</b>：系统管理员访问级别</li> 
         </ul> </li> 
       </ul> 
       <p>有关对象权限的信息，请参阅<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">对象权限共享概述</a>。</p> 
       <p><b>注释</b>：  
       <ul> 
       <li> <p>没有您在此处指定的权限的用户看不到部分中的自定义字段和小部件。 </p> <p>如果您在报表中显示字段的值，或在文本模式报表的计算字段中使用它们，也是如此。</p> </li> 
       <li><p>对于请求/问题自定义表单：如果需要查看访问权限才能查看分区界限中的字段，但需要管理员访问权限才能编辑字段，则非管理员在填写表单时将看不到分区及其所有字段。 创建请求后，具有查看权限的用户可以查看部分中的字段。</p></li>
       <li> <p>将多个对象类型与表单关联可以更改这些步骤中可用的查看和编辑权限。 有关详细信息，请参阅本文中的<a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">多个对象类型如何影响自定义表单中的分区界限权限</a>。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>添加逻辑</p></td> 
      <td><p>根据用户在填写表单时在多选自定义字段中做出的选择，使用显示逻辑指定是否在表单上显示部分。</p><p><strong>注意：</strong>如果分区界限下的所有单个字段都应用了显示逻辑，并且它们都因该逻辑而隐藏，则整个分区将在自定义表单上隐藏。 即使未将显示逻辑应用于分区界限，也会发生这种情况。</p><p>有关详细信息，请参阅<a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">使用表单设计器添加显示逻辑和跳过逻辑</a>。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 将至少一个自定义字段或构件拖动或添加到新分区。 在保存部分之前，必须先完成此操作。

1. 单击&#x200B;**完成**。

   >[!TIP]
   >
   >在创建自定义表单时，您可以随时单击&#x200B;**应用**&#x200B;以保存更改并保持表单打开。

### 多个对象类型如何影响分区界限权限 {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

自定义表单分区界限的“有限编辑”权限仅适用于“项目”、“任务”、“问题”和“用户”对象类型。

在配置了“有限编辑”权限的分区界限的自定义表单中，如果您向表单中添加了其他对象类型(Portfolio、程序、文档、公司、账单记录、小版本、费用或组)之一，则系统会提示您切换到“编辑”权限，该权限与该对象类型和表单上的现有对象类型都兼容。

>[!INFO]
>
>**示例：**&#x200B;在与Project对象类型关联的自定义表单中，分区界限配置有有限的编辑权限。
>
>您将Portfolio对象类型添加到表单，这意味着有限编辑权限选项不再可用于表单中的分区界限。
>
>屏幕消息会提示您切换到“编辑”权限，该权限是与项目对象类型和Portfolio对象类型兼容的最低级别权限。


## 在自定义表单中放置自定义字段和小部件


1. 开始创建或编辑自定义表单，如[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)中所述。

1. 要将自定义字段和小组件放置在同一行，请将一个字段和小组件拖动到另一个字段和小组件之间，直到它们之间出现一行。

   >[!NOTE]
   >
   >* 您可以使用右上角的&#x200B;**预览**&#x200B;按钮了解自定义字段和小组件在表单中的显示方式。
   >* 自定义字段和小组件在表单中的显示方式可能并不总是相同，具体取决于用户查看表单时可用的屏幕空间量。 例如，如果水平空间受限，一行字段中的第三个字段可能会换行到下一行字段。

1. （可选）要将自定义字段或小组件放置在另一个字段或小组件的上方或下方，请将其拖动到上方或下方，直到项目之间出现一条水平蓝线。

1. 要将自定义字段移动到表单上的另一个分区，您可以将其拖放到适当位置，<span class="preview">或单击字段上的&#x200B;**移至**&#x200B;图标并选择要将其移动到的分区。</span>

   <span class="preview">预览环境中的示例图像：</span>
   ![将字段移动到节](assets/move-field-to-section.png)

1. 若要保存更改，请单击&#x200B;**应用**

   或

   单击&#x200B;**保存并关闭**。

## 预览自定义表单

1. 开始创建或编辑自定义表单并添加字段，如[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)中所述。

1. 单击右上角的&#x200B;**预览**&#x200B;查看表单在使用时的外观，然后单击&#x200B;**结束预览**&#x200B;返回编辑表单。

