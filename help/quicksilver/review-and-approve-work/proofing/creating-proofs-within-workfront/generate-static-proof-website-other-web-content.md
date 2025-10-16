---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 为网站或其他Web内容创建静态验证
description: 您可以为Web内容生成新的静态验证或现有静态验证的新版本。 Web内容可能包括带流视频的广告、HTML动画或交互式横幅等，但将剪切为多个屏幕快照以实现静态校样。
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 1%

---

# 为网站或其他Web内容创建静态验证

您可以为Web内容生成新的静态验证或现有静态验证的新版本。 Web内容可能包括带流视频的广告、HTML动画或交互式横幅等，但将剪切为多个屏幕快照以实现静态校样。

为网站或其他Web内容创建静态验证时，请考虑以下事项：

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> 
   <p>标准</p>
   <p>工作或计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">校样权限配置文件 </td> 
   <td>经理或更高版本</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对文档的访问权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为网站或其他Web内容创建静态验证

要创建静态校对，网站需要可公开访问（不在防火墙内），或者您组织的允许列表必须包含Workfront域。 Workfront无法捕获受密码保护的网站作为静态校对。

>[!TIP]
>
>对于需要授权和受密码保护的页面的内部页面，我们建议使用交互式校对，而不是静态校对。 有关详细信息，请参阅[交互式内容校对概述](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md)。

1. 转到要创建新网站验证或现有网站验证的新版本的项目、任务或问题。
1. 单击左侧面板中的&#x200B;**文档**。
1. （视情况而定）如果要创建新校对，请单击“新增”****，然后在出现的菜单中单击“校对”****。
1. （视情况而定）如果您正在创建现有验证的新版本：

   1. 将鼠标悬停在要为其创建新版本的URL验证上，然后单击其周围的浅蓝色背景以将其选中。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. 单击&#x200B;**新增** > **版本** > **校对**。

1. 在&#x200B;**添加文件**&#x200B;区域键入要验证的网站URL，然后按&#x200B;**Enter**。

   >[!NOTE]
   >
   > URL必须少于2,000个字符。

1. 单击已添加的URL。

   随后会显示用于配置网站验证的选项。

   ![交互式校对](assets/interactive-proof-radio-btn-area-350x199.png)

1. （可选）如果要将校对名称从网站URL更改为其他名称，请键入&#x200B;**校对名称。**
1. 确保已选择&#x200B;**捕获屏幕快照**，并使用以下任一选项：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>屏幕快照分辨率</strong> </td> 
      <td> <p>在查看者查看验证时调整内容的分辨率，以便他们查看验证在各种大小的设备（如手机、平板电脑和显示器）上的显示方式。</p> <p>如果选择多个分辨率，则会为您选择的每个分辨率创建单独的校样。</p> <p>注意：当查看者对验证进行评论时，评论包括显示何时进行评论的分辨率，以便其他查看者知道哪个分辨率与评论相关联。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>查找子页面</strong> </td> 
      <td> <p>捕获网站的子页面及其主页。 您可以单击全选以包含所有页面，也可以仅单击要包含的特定页面。 加号和减号按钮允许您展开和关闭网站中的子页面区域。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >您无法更改所创建校对的任何后续版本的捕获屏幕快照设置。

1. 单击&#x200B;**完成**。

   如果在步骤8中选择了多个屏幕快照分辨率，则列表会包含每个分辨率的一组屏幕快照。 您可以生成这些屏幕截图作为单独的校样，或将其合并到单个校样中(请参阅  在。)。 我们建议您将它们组合在一起，尤其是当您要创建静态网站验证时。

   >[!NOTE]
   >
   >如果您向现有URL验证添加新版本，则在此版本中维护在原始验证或以前的版本上配置的任何选项。

1. 单击&#x200B;**创建校对**&#x200B;以创建无审阅过程的简单校对。\
   或\
   配置高级校对以继续：

   * [使用基本工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
