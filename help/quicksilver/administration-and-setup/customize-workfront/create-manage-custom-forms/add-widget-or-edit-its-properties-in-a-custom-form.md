---
title: 使用旧版表单生成器添加或编辑自定义表单中的图像或其他资源小组件
description: 您可以在自定义表单中添加或编辑以下任何资源小部件的属性，如图像、视频、PDF文件和Adobe XD文件。 当您需要为要设计的应用程序包含可视内容（例如品牌推广图像、说明性视频或交互式原型）时，此功能非常有用。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 1%

---

# 使用旧版表单生成器添加或编辑自定义表单中的图像或其他资源小组件

{{form-designer-default}}

您可以在自定义表单中添加或编辑以下任何资源小部件的属性：

* 图像
* 视频
* PDF文件
* Adobe XD文件

当您需要为要设计的应用程序包含可视内容（例如品牌推广图像、说明性视频或交互式原型）时，此功能非常有用。

将包含小部件的自定义表单附加到对象后，使用该对象的用户可以在以下区域看到该表单：

* 对象的“详细信息”区域（例如，对于项目，“项目详细信息”区域）
* 对象的“编辑”框(如果它具有新的Adobe Workfront Experience外观)（例如，“编辑项目”和“编辑任务”框）

目前，用户无法在以下区域中看到构件：&#x200B;

* 列表和报告
* 主页和摘要
* 对象的编辑框(如果它没有新的Adobe Workfront Experience外观)（例如，编辑费用框）
* Workfront移动设备应用程序


## 访问要求

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
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

&#42;要了解您拥有的计划、许可证类型或访问级别配置，请与Workfront管理员联系。

## 在自定义表单中添加或编辑资源小组件

1. 开始处理自定义表单，如中所述 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 使用 **添加字段** 打开Tab键，执行以下操作之一：

   * 如果要添加新构件，请选择 **图像**， **PDF**，或 **视频** 将其添加到表单底部，或将其拖动到表单上所需的位置。

     ![](assets/add-widget.png)


   * 如果要添加已添加到其他自定义表单的构件，请单击 **字段库**，然后单击显示列表中小组件的名称。 有关更多信息，请参阅 [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * 如果您正在编辑已添加到自定义表单的构件，请选择它。

1. 键入或编辑构件的以下任意属性：

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
      <td> <p>（必需）此名称是系统标识构件的方式。</p> <p>首次配置构件并键入标签时，会自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够自由更改用户看到的标签，而无需更改系统看到的名称。</p> <p><b>重要</b>：虽然可以这样做，但我们建议，在您或其他用户开始使用小部件中的自定义表单后，请勿更改此名称。 如果这样做，系统将不再识别该构件可能在Workfront的其他区域中被引用的构件。 </p> <p>每个构件名称在贵组织的Workfront实例中必须唯一。 这样，您就可以重复使用已经为其他自定义表单创建的表单。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴构件存储在Internet上的URL。</p> 
       <p><strong>重要</strong>：的URL必须是公共URL。 </p>
      <p>如果要添加视频构件，当前可通过在URL框中添加以下内容来实现此目的：</p> 
      <ul> 
      <li> <p>YouTube或Vimeo链接</p> </li> 
      <li> <p>Google Drive视频链接</p> </li> 
      <li> <p>视频链接，带有MP4和MOV扩展</p> </li> 
      <li> <p>视频链接已上传到Workfront实例中的文档区域。 有关说明，请参阅 <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">从文档区域将视频小组件添加到自定义表单</a> 本文章中。</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>键入有关构件的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>根据需要更改构件的显示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **应用**.
1. 如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## 将XD文件添加到自定义表单

1. 开始处理自定义表单，如中所述 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. 使用 **添加字段** 选项卡打开，选择 **Adobe XD**.
1. 键入或编辑构件的以下任意属性：

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
      <td> <p>（必需）此名称是系统标识构件的方式。</p> <p>首次配置构件并键入标签时，会自动填充名称字段以匹配它。 但是“标签”和“名称”字段不同步，这使您能够自由更改用户看到的标签，而无需更改系统看到的名称。</p> <p><b>重要</b>：虽然可以这样做，但我们建议，在您或其他用户开始使用小部件中的自定义表单后，请勿更改此名称。 如果这样做，系统将不再识别该构件可能在Workfront的其他区域中被引用的构件。 </p> <p>每个构件名称在贵组织的Workfront实例中必须唯一。 这样，您就可以重复使用已经为其他自定义表单创建的表单。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>（必需）键入或粘贴有效的XD原型链接。</p> 
      <p>注意：在Adobe XD中，共享选项卡上的链接访问设置必须设置为具有链接的任何人。 否则，用户将无法查看原型。 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">说明</td> 
      <td> <p>（可选）键入有关构件的任何其他信息。 当用户填写自定义表单时，可以将光标悬停在问号图标上，以查看包含您在此处键入的信息的工具提示。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">大小</td> 
      <td>（可选）根据需要更改构件的显示大小。</td> 
     </tr> 
    </tbody> 
   </table>

1. 如果要继续以其他方式构建自定义表单，请继续阅读以下文章之一：

   * [在自定义表单中放置自定义字段和小部件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [将自定义字段添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [在自定义表单中重用自定义字段或小组件](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [在自定义表单中重用现有的计算自定义字段](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [向自定义表单添加显示逻辑和跳过逻辑](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [预览并完成自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## 从文档区域将视频小组件添加到自定义表单 {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>以这种方式将视频添加到自定义表单时，当用户访问对象上的表单时，只有为自定义表单设置的权限才应用于视频，而不是“文档”区域中为视频设置的权限。

1. 转到文档区域中的视频并为其生成验证，如中所述 [为网站或其他Web内容创建交互式验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. 打开证明。
1. 右键单击视频上的任意位置，然后选择 **复制视频地址**.
1. 在添加视频小部件的自定义表单中，将复制的地址粘贴到 **URL** 盒子。
