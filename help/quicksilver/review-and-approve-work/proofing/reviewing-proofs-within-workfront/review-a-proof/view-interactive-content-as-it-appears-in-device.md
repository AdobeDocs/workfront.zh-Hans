---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 在验证查看器中更改交互式验证分辨率
description: 您可以预览交互式验证在各种设备上的外观，从而了解内容基于不同分辨率的显示和响应方式。
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: d4fa663e22daf25fec77be79a452eb207857bdda
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 1%

---

# 在验证查看器中更改交互式验证分辨率

您可以预览交互式验证在各种设备上的外观，从而了解内容基于不同分辨率的显示和响应方式。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

## 桌面验证查看器与Web验证查看器中的设备和分辨率视图

您的Adobe Workfront管理员已配置您的系统，以便在桌面验证查看器中或作为ZIP文件中的捆绑内容在Web验证查看器中查看交互式内容：

* 在桌面校对查看器中，您可以查看内容在各种分辨率和各种设备上的显示和响应方式。 当查看者指定某个设备时，内容将按该设备的用户界面规范在该设备上显示出来。 例如，一个智能手机品牌上的红色按钮可能为另一个品牌上的蓝色按钮。

* 在Web校对查看器中，可以查看各种设备分辨率中显示的交互式内容。 但Web验证查看器不会在这些设备上使用界面规范（如按钮颜色）来模拟内容。

  >[!NOTE]
  >
  >您的Workfront管理员可以为贵组织中的用户配置自定义设备，如[为贵组织配置验证设置](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md)一文中的[为验证配置自定义设备](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs)中所述。

## 使用预设设备或分辨率设置查看校样

1. 转到包含要打开的校样的文档列表。
1. 将鼠标悬停在文档上，然后单击&#x200B;**打开验证**。
1. 单击验证查看器中底部的&#x200B;**响应**。

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. 在桌面校对查看器中显示的设备和分辨率列表中，单击所需的设备和分辨率。

   或

   在Web验证查看器中，在显示的分辨率列表中，单击所需的分辨率。

   如果需要有关这两个查看器的差异的信息，请参阅[Web验证查看器和桌面验证查看器之间的差异概述](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)。

   交互式验证会以您选择的分辨率呈现。

## 查看具有自定义分辨率设置的验证

1. 转到包含要打开的校样的文档列表。
1. 将鼠标悬停在文档上，然后单击&#x200B;**打开验证**。
1. 单击验证查看器中底部的&#x200B;**响应**。
1. 键入自定义&#x200B;**响应式**&#x200B;分辨率。

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   或

   将鼠标悬停在交互式内容上，并将右下角、右边缘或下边缘的蓝色边框拖动到所需的分辨率。

   ![Drag_blue_edges_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   自定义分辨率显示在以下位置：

   * 在查看器底部中央的&#x200B;**分辨率**&#x200B;面板中。\
     ![Screenshot_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * 在任意评论中，审阅人添加到验证中。 每个注释都包括查看者创建注释时选择的屏幕分辨率。
