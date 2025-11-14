---
content-type: overview
product-area: portfolios
navigation-topic: create and manage programs
title: 程序概述
description: 项目群是具有统一特性的项目的集合。 这些项目通常会争夺相同的资源、预算或时限。 项目是项目组合的子组。 在将项目添加到项目组合之前，您可以将项目与项目群关联。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1c64fe00-12e3-49f6-b864-b8f89ed9140d
source-git-commit: 8cd6c47acf8de313bab5fe7298125eb63cc10faf
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 1%

---

# 程序概述

<!-- Audited: 08/2025 -->

在Adobe Workfront中，项目群是具有统一特性的项目集合。 例如，他们可能会争夺相同的预算、资源或时间范围。 项目是项目组合的子组。

本文包含有关Workfront中程序的一般信息。


## 创建程序所需的访问权限

<!--leave the table uncollapsed as this article is about access-->

您必须具有以下权限才能创建和管理项目组合：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> <p>任何</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[！UICONTROL标准版]</p>
   <p>[！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL Edit]对[！UICONTROL项目组合]和[！UICONTROL项目]的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理权限以编辑项目群或向其添加项目</p>
   <p>管理项目群所属项目组合的权限 </p>
   <p>查看查看查看程序的权限以查看它</p>
   <p>创建项目后，默认情况下，您拥有管理权限</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>New: Any</p>
   <p>Current: [!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to edit a program or add projects to it</p>
   <p>Manage permissions to the portfolio that the program belongs to </p>
   <p>View permissions to a program to view it</p>
   <p>After you create a program, you have Manage permissions to it, by default</p> 
    </td> 
  </tr> 
 </tbody> 
</table>-->


## 有关使用程序的注意事项

* 您可以同时使用项目组合和项目群来组织项目。 通过组织项目，您可以比较类似项目并确定将最佳使用资源的位置。

* 项目是项目组合的子组。 如果项目组合包含的项目太多，您可以将其划分为多个项目群，并依次按项目群和项目组合组织项目。

  例如，您可以有一个Marketing 2024项目组合，分为四个季度计划。

* 属于同一项目的项目通常会争夺相同的资源、预算或时隙。

* 您必须首先创建一个项目组合，然后可以在同一项目组合中创建多个项目。

  有关使用程序的信息，请参阅[创建程序](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)。

* 必须先创建项目组合，然后再创建项目群，然后才能将项目群与项目群和项目组合关联。

* 在创建项目、项目和项目组合时，请考虑以下事项：

   * 项目可以是独立的，不与项目或项目组合关联。
   * 项目可与项目组合关联，但也不需要也与项目群关联。
   * 项目群必须始终与项目组合关联。 它永远不可能存在于投资组合之外。
   * 与项目群关联的项目始终与项目群的项目组合关联。
   * 项目只能与一个项目组合关联。
   * 一个项目一次只能与一个项目群和项目群的项目组合相关联。
   * 一个项目组合可以有多个项目和程序。
   * 一个项目群可以有多个项目。

  有关创建项目和项目组合的信息，请参阅以下文章：
   * [创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
   * [创建项目组合](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)


* 您可以使用项目组合优化器分析项目组合中所有项目的性能。 不能仅比较同一项目群中多个项目的性能。 您必须在项目组合级别分析项目绩效。

  有关信息，请参阅[在Portfolio优化器中优化项目](/help/quicksilver/manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md)。
