---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 在校样中查看自动化工作流阶段
description: 您可以方便地跟踪使用自动工作流配置的校样的进度。 您可以查看、修改、添加、启动和锁定已在校样的舞台上完成的工作。
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# 在校样中查看自动化工作流阶段

您可以方便地跟踪使用自动工作流配置的校样的进度。 您可以查看、修改、添加、启动和锁定已在校样的舞台上完成的工作。

有关使用自动工作流向校样添加阶段和用户的信息，请参阅 [在校样上将阶段和用户添加到自动工作流](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

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
   <td> <p>编辑对文档的访问</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、角色或校样权限配置文件，请联系您的Workfront或Workfront校样管理员。

## 查看自动化工作流图

1. 在包含文档的文档列表中，将鼠标悬停在包含文档的行上，然后单击 **校对工作流**.

   自动工作流的图表显示在工作流标题的正下方。

   图表中的阶段标记如下：

   ![dot.png](assets/dot.png) 活动阶段

   ![gray_dot.png](assets/grey-dot.png) 不活动阶段\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  私人舞台

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  锁定的舞台

   阶段之间的线条描述了阶段之间的依赖关系。 在激活舞台之前，指向不活动舞台的线条会一直虚线。

   您可以将鼠标悬停在图中的某个阶段上以显示其进度。 如果舞台未处于活动状态，并且您对舞台具有编辑权限，则可以单击“激活舞台”按钮 ![](assets/activate-stage-btn.png) 来开始舞台。 如果舞台处于活动状态，并且您对舞台具有编辑权限，则可以将其锁定。 ![](assets/lock-stage-btn.png) 有关进度栏(S、O、C、D)的更多信息，请参阅  [查看Workfront校样中校样的进度和状态](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## 查看阶段

1. 在包含文档的文档列表中，将鼠标悬停在包含文档的行上，然后单击 **校对工作流**.
1. 在图表上，单击要查看的阶段。

   ![](assets/view-stage-diagram-350x204.png)

1. 要展开舞台的详细信息，请单击其名称下方的侧箭头。

   ![](assets/stage-details-caret-350x167.png)

## 查看所有阶段

要在自动化工作流中查看所有阶段，请执行以下操作：

1. 单击页面顶部的Change View按钮 ![](assets/change-view-btn.png)，然后单击 **查看所有阶段**.

   自动工作流的所有阶段都在部分中列出，但详细信息是隐藏的。

1. 要展开舞台的详细信息，请单击其名称下方的侧箭头。

## 详细查看所有阶段

要查看自动化工作流的所有阶段及其详细信息，请执行以下操作：

1. 单击页面顶部的Change View按钮 ![](assets/change-view-btn.png)，然后单击 **详细查看所有阶段**.
1. 要查看舞台的详细信息，请单击其名称下方的向下箭头。
