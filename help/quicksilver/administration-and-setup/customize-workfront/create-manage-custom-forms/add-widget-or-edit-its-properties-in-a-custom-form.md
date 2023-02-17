---
title: 在自定义表单中添加或编辑图像或其他资产小组件
description: 您可以在自定义表单中添加或编辑以下任何资产小组件(如图像、视频、PDF文件和Adobe XD文件)的属性。 当您需要包含可视内容（如品牌图像、指导性视频或您设计的应用程序的交互式原型）时，此功能非常有用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: 8e903592456512f1ebf5f1e8d6e496e577a7b352
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 1%

---

# 在自定义表单中添加或编辑图像或其他资产小组件

您可以在自定义表单中添加或编辑以下任何资产小组件的属性：

* 图像
* 视频
* PDF文件
* Adobe XD文件

当您需要包含可视内容（如品牌图像、指导性视频或您设计的应用程序的交互式原型）时，此功能非常有用。

将包含小组件的自定义表单附加到对象后，使用该对象的用户可以在以下区域看到该对象：

* 对象的“详细信息”区域（例如，对于项目，“项目详细信息”区域）
* 对象的“编辑”框(如果具有新的Adobe Workfront体验外观)（例如，“编辑项目”和“编辑任务”框）

目前，用户在以下区域中看不到小组件&#x200B;:

* 列表和报表
* 主页和摘要
* 对象的“编辑”框(如果它没有新的Adobe Workfront体验外观)（例如，“编辑费用”框）
* Workfront移动设备应用程序


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

## 在自定义表单中添加或编辑资产小组件

1. 开始使用自定义表单，如 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 使用 **添加字段** 选项卡，执行下列操作之一：

   * 如果要添加新小组件，请选择 **图像**, **PDF**&#x200B;或 **视频** 要在表单底部添加该组件，或将其拖动到表单上所需的位置。

      ![](assets/add-widget.png)


   * 如果要添加已添加到其他自定义表单的小组件，请单击 **字段库**，然后在显示的列表中单击小组件的名称。 有关更多信息，请参阅 [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * 如果您正在编辑已添加到自定义表单的小组件，请选择它。

1. 为小组件键入或编辑以下任意属性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在小组件上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>:避免在此标签中使用特殊字符。 无法在报表中正确显示它们。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统识别小组件的方式。</p> <p>首次配置小组件并键入标签时，“名称”字段会自动填充以匹配该小组件。 但“标签”和“名称”字段未同步，这可让您自由更改用户看到的标签，而无需更改系统看到的名称。</p> <p><b>重要信息</b>:虽然可以这样做，但建议您在或其他用户开始使用小组件中的自定义表单后，不要更改此名称。 如果您这样做，系统将不再识别现在可能在Workfront其他区域引用该小组件的小组件。 </p> <p>在贵组织的Workfront实例中，每个小组件名称必须唯一。 这样，您就可以重复使用已为其他自定义表单创建的表单。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴存储在Internet上的小组件的URL。</p> 
       <p><strong>重要信息</strong>:的URL必须是公共URL。 </p>
      <p>如果您添加视频小组件，当前可以通过在URL框中添加以下内容来执行此操作：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo链接</p> </li> 
      <li> <p>Google Drive视频链接</p> </li> 
      <li> <p>链接到扩展为MP4和MOV的视频</p> </li> 
      <li> <p>已上传到Workfront实例中“文档”区域的视频的链接。 有关说明，请参阅 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">从“文档”区域将视频小组件添加到自定义表单</a> 在本文中。</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关小组件的任何其他信息。 当用户填写自定义表单时，他们可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>根据需要更改小组件的显示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **应用**.
1. 如果您希望以其他方式继续构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中放置自定义字段和小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重复使用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## 将XD文件添加到自定义表单

1. 开始使用自定义表单，如 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 使用 **添加字段** 选项卡打开，选择 **Adobe XD**.
1. 为小组件键入或编辑以下任意属性：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">标签</td> 
      <td> <p>（必需）键入要在小组件上方显示的描述性标签。 您可以随时更改标签。</p> <p><b>重要信息</b>:避免在此标签中使用特殊字符。 无法在报表中正确显示它们。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>（必需）此名称是系统识别小组件的方式。</p> <p>首次配置小组件并键入标签时，“名称”字段会自动填充以匹配该小组件。 但“标签”和“名称”字段未同步，这可让您自由更改用户看到的标签，而无需更改系统看到的名称。</p> <p><b>重要信息</b>:虽然可以这样做，但建议您在或其他用户开始使用小组件中的自定义表单后，不要更改此名称。 如果您这样做，系统将不再识别现在可能在Workfront其他区域引用该小组件的小组件。 </p> <p>在贵组织的Workfront实例中，每个小组件名称必须唯一。 这样，您就可以重复使用已为其他自定义表单创建的表单。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴有效的XD原型链接。</p> 
      <p>注意：在Adobe XD中，“共享”选项卡上的“链接访问”设置必须设置为具有该链接的任何人。 否则，用户将无法查看原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>（可选）键入有关小组件的任何其他信息。 当用户填写自定义表单时，他们可以将鼠标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改小组件的显示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 如果您希望以其他方式继续构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中放置自定义字段和小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自定义表单中重复使用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [将计算数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重复使用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 从“文档”区域将视频小组件添加到自定义表单 {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以这种方式将视频添加到自定义表单时，当用户访问对象上的表单时，只有为自定义表单设置的权限才会应用到视频，而不是“文档”区域中为视频设置的权限。

1. 转到“文档”区域中的视频，并为其生成校样，如 [为网站或其他Web内容创建交互式校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 打开校样。
1. 右键单击视频上的任意位置，然后选择 **复制视频地址**.
1. 在添加视频小组件的自定义表单中，将复制的地址粘贴到 **URL** 框中。
