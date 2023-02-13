---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 为网站或其他Web内容创建静态校样
description: 您可以为Web内容生成新的静态校样或现有静态校样的新版本。 Web内容可以包括带有流视频的广告、HTML动画或交互式横幅，但它将被剪切为多个屏幕截图，以便进行静态校样。
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# 为网站或其他Web内容创建静态校样

您可以为Web内容生成新的静态校样或现有静态校样的新版本。 Web内容可以包括带有流视频的广告、HTML动画或交互式横幅，但它将被剪切为多个屏幕截图，以便进行静态校样。

为网站或其他Web内容创建静态校样时，请考虑以下事项：

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：选择或Premium</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
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

## 为网站或其他Web内容创建静态校样

要创建静态校样，网站需要公开访问（而不是在防火墙之后），或者贵组织的允许列表必须包含Workfront域。 Workfront无法捕获受密码保护的网站作为静态校样。

>[!TIP]
>
>对于需要授权和受密码保护的内部页面，我们建议使用交互式校样，而不是静态校样。 有关更多信息，请参阅 [交互式内容校样概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. 转到要创建新网站校样或现有网站校样新版本的项目、任务或问题。
1. 单击 **文档** 中。
1. （视情况而定）如果要创建新校样，请单击 **新增**，然后单击 **校样** 中。
1. （视情况而定）如果您正在创建现有校样的新版本：

   1. 将鼠标悬停在要为其创建新版本的URL校样上，然后通过单击其周围的浅蓝色背景来选择该校样。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 单击 **新增** > **版本** > **校样**.

1. 在 **添加文件** 区域，然后按 **输入**.

   URL显示在您键入该URL的框的下方。

   ![](assets/url-name-appears-below-350x142.png)

1. 单击您添加的URL。

   此时会显示用于配置网站校样的选项。

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. （可选）如果要将校样的名称从网站URL更改为其他内容，请键入 **校样名称。**
1. 确保 **捕获屏幕截图** ，并使用以下任意选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>屏幕截图分辨率</strong> </td> 
      <td> <p>在审阅人查看校样时，调整内容的分辨率，使审阅人能够查看校样在不同大小的设备（如手机、平板电脑和显示器）上的显示方式。</p> <p>如果选择多个分辨率，则会为您选择的每个分辨率创建单独的校样。</p> <p>注意：当审阅人对校样进行评论时，该评论包含显示评论何时发表的解析，以便其他审阅人知道与评论关联的解析。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>查找子页面</strong> </td> 
      <td> <p>捕获网站的子页面及其主页。 您可以单击全选以包含所有页面，也可以仅单击要包含的特定页面。 通过加号和减号按钮，您可以展开和关闭网站中的子页面区域。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >您无法更改您创建的校样的任何后续版本的捕获屏幕截图设置。

1. 单击 **完成**.

   如果您在步骤8中选择了多个屏幕截图分辨率，则列表将包含每个分辨率的一组屏幕截图。 您可以生成这些屏幕截图作为单独的校样，或将它们合并到单个校样中（请参阅中的）。 我们建议您将它们组合在一起，特别是当您要创建静态网站校样时。

   >[!NOTE]
   >
   >如果向现有URL校样添加新版本，则在原始校样或之前版本上配置的任何选项都将在此版本中进行维护。

1. 单击 **创建校样** 创建简单的校样，而不进行审核过程。\
   或\
   继续配置高级校样：

   * [使用基本工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动工作流创建高级校样](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
