---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: 批量编辑文档
description: 您可以在“文档”区域中一次编辑多个文档。
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
source-git-commit: f9ebf647c7672a9d471288806cf596d103007613
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# 批量编辑文档

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览Sandbox”环境中可用。</span>

您可以一次编辑多个文档中的描述、添加自定义表单和编辑自定义表单。

## 编辑自定义表单时的注意事项

批量编辑文档自定义表单时，请考虑以下事项：

* 您在所有选定文档上更改的信息将覆盖单个文档上的现有信息。
* 当您为同一字段选择具有不同值的文档时，该字段显示“多个值”指示符。 复选框、单选按钮和切换的字段旁边有一个“多个值”指示器。
* 当在多选项字段（如显示为一组切换或复选框的字段）中更新一个选项时，所选文档之间的所有其他选项必须匹配。

>[!BEGINSHADEBOX]

**示例**
您可能会有一个带有复选框字段的自定义表单，其中带有三个复选框（“选项1”、“选项2”和“选项3”），对于所有选定的文档，选项1处于未选中状态，对于某些选定的文档，选项2和3处于选中状态，对于其他选定的文档，选项3处于未选中状态。 如果要为所有文档选中选项1，则还必须使选项2和3与所有选定项目匹配，然后才能保存更改。 因此，您必须选择或取消选择它们，以使它们在所有选定项目上匹配。 如果不更改任何选项，则可以按原样保存该字段，并且文档会保留所有选项的当前选择。

>[!ENDSHADEBOX]

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p> 任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td><p> 新文档：参与者或更高版本</p> 
   <p> 当前：请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

+++

## 批量编辑文档

要批量编辑文档，请执行以下操作：

1. 从主菜单导航到项目的文档选项卡或文档区域。
1. 按键盘上的ctrl或cmd，然后选择要编辑的文档。
1. 单击编辑图标![编辑图标](assets/edit-icon.png)。
   ![编辑图标在页面上的位置](assets/edit-multiple-documents.png)
1. （可选）添加或编辑&#x200B;**描述**。 如果每个文档上的描述不同，您将在描述框中看到&#x200B;_多个值_。 您可以为所有文档添加相同的描述，但在批量编辑时无法编辑单个文档描述。
1. 对自定义表单进行以下更改：

   <table>
    <tr>
    <td><strong>添加表单</strong></td>
    <td>在<strong>添加自定义表单框</strong>中，您可以从附加的表单中选择要添加的表单。 附加的表单位于某些选定文档上，但不是全部文档上。 附加到所有选定文档的表单会自动显示在编辑窗口中。  </td>
    </tr>
    <tr>
    <td><strong>编辑表单</strong></td>
    <td>编辑任何附加的自定义表单。 您更改的信息将覆盖单个文档上的现有信息。 文档中具有不同值的字段显示为“多个值”。 </td>
    </tr>
    <tr>
    <td><strong>重新排列表单</strong></td>
    <td>单击并拖动自定义表单以重新排列。</td>
    </tr>
    </table>
1. 单击&#x200B;**保存**。

<span class="preview">

## 在文档报告中批量编辑文档

1. 导航到现有文档报告。
或
按照[创建自定义报告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明创建文档报告。
1. 选择要编辑的文档。
1. 单击编辑图标![编辑图标](assets/edit-icon.png)。
   ![编辑图标在页面上的位置](assets/edit-multiple-documents.png)
1. （可选）添加或编辑&#x200B;**描述**。 如果每个文档上的描述不同，您将在描述框中看到&#x200B;_多个值_。 您可以为所有文档添加相同的描述，但在批量编辑时无法编辑单个文档描述。
1. 对自定义表单进行以下更改：

   <table>
    <tr>
    <td><strong>添加表单</strong></td>
    <td>在<strong>添加自定义表单框</strong>中，您可以从附加的表单中选择要添加的表单。 附加的表单位于某些选定文档上，但不是全部文档上。 附加到所有选定文档的表单会自动显示在编辑窗口中。  </td>
    </tr>
    <tr>
    <td><strong>编辑表单</strong></td>
    <td>编辑任何附加的自定义表单。 您更改的信息将覆盖单个文档上的现有信息。 文档中具有不同值的字段显示为“多个值”。 </td>
    </tr>
    <tr>
    <td><strong>重新排列表单</strong></td>
    <td>单击并拖动自定义表单以重新排列。</td>
    </tr>
    </table>
1. 单击&#x200B;**保存**。

</span>