---
content-type: overview
product-area: portfolios
navigation-topic: portfolios-overview
title: 了解Portfolio方法
description: Portfolio是具有统一特性的项目集合。 这些项目通常会争夺相同的资源、预算或时限。 您可以将项目组合划分为项目群，并在将项目群添加到Portfolio之前将项目群与项目群关联。
author: Alina
feature: Work Management, Strategic Planning
exl-id: b340501e-1190-415e-aa96-5aad177c4b7b
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 了解项目组合方法

<!-- Audited: 1/2024 -->

Portfolio或项目Portfolio管理(PPM)是对项目列表进行优先级划分和管理以实现特定业务目标的过程。

有关PPM的一般信息，请参阅[Portfolio管理概述](/help/quicksilver/manage-work/portfolios/portfolios-overview/portfolio-managament-overview.md)。

在Adobe Workfront中，项目组合是指一组具有统一特性的项目。 这些项目通常会争夺相同的资源、预算或时限。 您可以将项目组合划分为项目群，并在将项目群添加到Portfolio之前将项目群与项目群关联。

您可以使用项目组合和项目群来组织项目。 通过组织项目，您可以比较类似项目并确定将最佳使用资源的位置。

有关使用程序的信息，请参阅[创建程序](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

本文包含有关Workfront中的项目组合的一般信息。

## 创建项目组合所需的访问权限

<!--leave the table uncollapsed as this article is about access-->

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> <p>Workfront Prime或更高版本</p>
   <p>工作流Prime或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[！UICONTROL标准版]</p>
   <p>[！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL Edit]对项目组合的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>创建项目组合后，默认情况下，您拥有其管理权限</p> 
   <p>管理权限以编辑项目组合或向其中添加项目</p>
   <p>查看项目组合的权限以在Workfront中查看它</p>
    </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Any</p>
   <p>Current:[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## 了解[!DNL Adobe Workfront]项目组合方法

在[!DNL Workfront]中，您可以将项目添加到项目组合以创建和组织项目组合。

我们建议您按照以下步骤有效组织您的项目组合：

1. 为项目创建业务案例并将项目与Portfolio关联。

   要创建为您的组织带来价值的高效项目组合，您必须从项目请求开始，在该请求中您为以后添加到项目组合中的每个项目定义业务案例。

   [!UICONTROL 商业案例]包含以下信息：

   * 有关项目的一般信息(描述、Portfolio和项目群分配、项目所有者和发起人)
   * 项目的目的或目标
   * 估计费用成本
   * 劳力成本的资源预算
   * 一致性分数
   * 风险评估

   有关[!UICONTROL 业务案例]的详细信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

   您可以在构建项目组合的业务案例时将项目与项目组合关联。 必须先创建项目组合，然后才能将其与项目关联。 有关信息，请参阅[创建项目组合](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)

   您在构建业务案例过程中收集的详细信息用于[!UICONTROL 项目组合优化器]和[!UICONTROL 资源规划者]，以协助管理层选择项目。
1. 在构建项目的业务案例时将资源池与项目关联。

   项目组合通常配置为与资源池相对应。 Portfolio中的程序也与资源池一致。 这种关联有助于确保所有资源规划都符合Portfolio的目的，因为同一Portfolio中的项目通常会争夺相同的资源。

   有关详细信息，请参阅[创建资源池](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)。

1. 获取Portfolio经理批准的[!UICONTROL 商业案例]。

   有关信息，请参阅[批准业务案例](/help/quicksilver/manage-work/projects/define-a-business-case/approve-business-case.md)。
1. 在[!UICONTROL Portfolio Optimizer]中管理项目组合中的项目性能。

   Portfolio Manager可以使用Portfolio功能板跟踪投资组合内的财务表现。 此仪表板显示在Portfolio的标题中。

   有关Portfolio的财务字段的信息，请参阅[Portfolio Optimizer概述](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md#financial-fieds-subsection)中的[了解Portfolio Optimizer中的财务字段](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)部分。
