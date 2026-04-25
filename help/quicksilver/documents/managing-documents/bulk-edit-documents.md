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
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 2%

---

# 批量编辑文档

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

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>使用旧版Workfront存储管理文档的任何Workfront软件包</p>
<p>用于使用Adobe企业存储管理文档的任意工作流包</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td><p>参与者或更高版本</p> 
   <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对文档的访问</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Edit documents in bulk in the legacy documents area

如果您的组织位于旧版Workfront存储中，则当您访问Workfront中的文档时，将会看到旧版文档区域。 有关Workfront存储的详细信息，请参阅[Adobe企业存储与旧版Workfront存储之间的差异](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage)。

To edit documents in bulk:

1. Navigate to the Documents tab of a project or the Documents area from the main menu.
1. Press ctrl or cmd on your keyboard, and select the documents you want to edit.
1. Click the Edit icon ![edit icon](assets/edit-icon.png).
   ![edit icon location on page](assets/edit-multiple-documents.png)
1. (Optional) Add or edit the **Description**. If the description on each document is different, you will see _Multiple values_ in the description box. You can add the same description for all documents, but you cannot edit individual document descriptions when editing in bulk.
1. Make the following changes with custom forms:

   <table>
    <tr>
    <td><strong>Add forms</strong></td>
    <td>In the <strong>Add custom form box</strong>, you can choose from Attached forms and forms to add. Attached forms are on some of the selected documents, but not all. A form attached to all selected document displays in the edit window automatically.  </td>
    </tr>
    <tr>
    <td><strong>Edit forms</strong></td>
    <td>Edit any attached custom forms. The information you change overwrites the existing information on individual documents. Fields with different values across documents display as "Multiple values". </td>
    </tr>
    <tr>
    <td><strong>Rearrange forms</strong></td>
    <td>Click and drag the custom form to rearrange.</td>
    </tr>
    </table>
1. 单击&#x200B;**保存**。

## Edit documents in bulk in the new documents area


如果您的组织使用企业存储，则当您访问Workfront中的文档时，将会看到“新建文档”区域。 有关企业存储的更多信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

要批量编辑文档，请执行以下操作：

1. 转到包含文档的项目、任务或问题，然后选择&#x200B;**文档**。
1. 按键盘上的ctrl或cmd，然后选择要编辑的文档。
1. 单击页面底部的“编辑”。
   ![编辑多个文档](assets/bulk-edit-documents.png)
1. （可选）添加或编辑&#x200B;**描述**。 如果每个文档上的描述不同，您将在描述框中看到&#x200B;_多个值_。 您可以为所有文档添加相同的描述，但在批量编辑时无法编辑单个文档描述。
1. 对自定义表单进行以下更改：

   <table>
    <tr>
    <td><strong>添加表单</strong></td>
    <td>在<strong>自定义表单</strong>分区中，可以将新的自定义表单添加到所选文档。 附加到所有选定文档的自定义表单显示在公共</strong>分区中的<strong>自定义表单中。  </td>
    </tr>
    <tr>
    <td><strong>编辑表单</strong></td>
    <td>编辑任何附加的自定义表单。 您更改的信息将覆盖单个文档上的现有信息。 文档中具有不同值的字段显示为“多个值”。 </td>
    </tr>
    </table>
1. 单击&#x200B;**保存**。

## 在文档报告中批量编辑文档

1. 导航到现有文档报告。
或
按照[创建自定义报告](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中的说明创建文档报告。
1. 选择要编辑的文档。
1. 单击编辑图标![编辑图标](assets/edit-icon.png)。
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
