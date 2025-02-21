---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: 为网站或其他Web内容创建交互式验证
description: 您可以为Web内容生成新的交互式验证或现有交互式验证的新版本。 这可以是网站或其他类型的交互式内容，例如带有流视频或音频的广告、HTML动画和交互式横幅。
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# 为网站或其他Web内容创建交互式验证

您可以为Web内容生成新的交互式验证或现有交互式验证的新版本。 这可以是网站或其他类型的交互式内容，例如带有流视频或音频的广告、HTML动画和交互式横幅。

在交互式验证中，查看者可以像平常一样导航和交互网站或其他Web内容。

>[!IMPORTANT]
>
>确保将要审阅该网站或交互式内容的人员能够访问它。 他们只能在校对过程中访问它，但前提是他们也可以通过互联网访问它。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：Premium</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
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
   <td> <p>编辑对文档的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、角色或验证权限配置文件，请联系您的Workfront或Workfront Proof管理员。

+++

## 为网站或其他Web内容创建交互式验证

1. 转到要创建新网站验证或现有网站验证的新版本的项目、任务或问题。
1. 单击左侧面板中的&#x200B;**文档**。
1. （视情况而定）如果要创建新校对，请单击“新增”****，然后在出现的菜单中单击“校对”****。

1. （视情况而定）如果要创建现有验证的新版本，则显示&#x200B;**新验证**&#x200B;页面：

   1. 将鼠标悬停在要为其创建新版本的URL验证上，然后单击其周围的浅蓝色背景以将其选中。

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. 在&#x200B;**添加新**&#x200B;下拉列表中，单击&#x200B;**版本** > **校对**。

1. 在&#x200B;**添加文件**&#x200B;部分中，键入要校对的网站URL，然后按&#x200B;**Enter**。  您可以重复此过程以添加多个要校对的网站。

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > URL必须少于1,000个字符。

1. 单击已添加的URL。

   ![单击URL](assets/click-url-350x137.png)

1. （可选）如果要将网站URL中的验证名称更改为其他名称，请键入&#x200B;**验证名称**。
1. 选择&#x200B;**交互式**，然后单击&#x200B;**完成**。

   >[!NOTE]
   >
   >如果您向现有URL验证添加新版本，则在此版本中维护在原始验证或以前的版本上配置的任何选项。

1. 单击&#x200B;**创建校对**&#x200B;以创建无审阅过程的简单校对。\
   或\
   配置高级校对以继续：

   * [使用基本工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [使用自动化工作流创建高级验证](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
