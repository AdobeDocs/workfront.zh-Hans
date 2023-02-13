---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 为网站或其他Web内容创建交互式校样
description: 您可以为Web内容生成新的交互式校样或现有交互式校样的新版本。 这可以是网站或其他类型的交互式内容，如带有流视频或音频的广告、HTML动画和交互式横幅。
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# 为网站或其他Web内容创建交互式校样

您可以为Web内容生成新的交互式校样或现有交互式校样的新版本。 这可以是网站或其他类型的交互式内容，如带有流视频或音频的广告、HTML动画和交互式横幅。

在交互式校样中，审阅人可以像往常一样导航和与网站或其他Web内容交互。

>[!IMPORTANT]
>
>确保要审阅网站或交互式内容的人员可以访问该网站或交互式内容。 只有当用户也可以在Internet上访问校样流程时，他们才能在校样流程中访问该页面。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校对权限配置文件 </td> 
   <td>经理或更高级别</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对文档的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 为网站或其他Web内容创建交互式校样

1. 转到要创建新网站校样或现有网站校样新版本的项目、任务或问题。
1. 单击 **文档** 中。
1. （视情况而定）如果要创建新校样，请单击 **新增**，然后单击 **校样** 中。

1. （视情况而定）在 **新校样** 页面时，如果您正在创建现有校样的新版本，则会显示该页面：

   1. 将鼠标悬停在要为其创建新版本的URL校样上，然后通过单击其周围的浅蓝色背景中的以将其选中。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 在 **新增** 下拉菜单，单击 **版本** > **校样**.

1. 在 **添加文件** ，键入要校样的网站的URL，然后按 **输入**.

   ![proof_website.png](assets/proof-website-350x65.png)

   您可以重复此过程以添加多个要校验的网站。

1. 单击您添加的URL。

   ![](assets/click-url-350x137.png)

1. （可选）如果要将校样的名称从网站URL更改为其他内容，请键入 **校样名称**.
1. 选择 **交互式**，然后单击 **完成**.

   >[!NOTE]
   >
   >如果向现有URL校样添加新版本，则在原始校样或之前版本上配置的任何选项都将在此版本中进行维护。

1. 单击 **创建校样** 创建简单的校样，而不进行审核过程。\
   或\
   继续配置高级校样：

   * [使用基本工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
