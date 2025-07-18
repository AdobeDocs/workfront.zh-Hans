---
product-area: projects
navigation-topic: business-case-and-scorecards
title: 创建和编辑项目的风险
description: 风险是阻止项目按时完成或在预算内完成的可能事件或因素。 您可以在创建项目的业务案例时记录项目风险，也可以使用“风险”选项卡进行记录。 您可以向项目和模板添加风险。 您不能将风险与任务或问题相关联。
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 1%

---

# 创建和编辑项目风险

<!--Audited: 06/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

风险是阻止项目按时完成或在预算内完成的可能事件或因素。 您可以在创建项目的业务案例时记录风险，也可以使用“风险”选项卡记录风险。

您只能为项目或模板创建风险。 您不能将风险与任务或问题相关联。

风险可以与成本相关联，但实际风险成本不会影响项目的实际成本。

>[!NOTE]
>
>当您在项目的业务案例中定义项目风险或在项目的风险选项卡中添加项目风险时，本文会定义与项目相关的风险。
>
>有关编辑项目时可用的风险字段的信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> <p>当前计划：</p>
   <ul><li>任何计划，用于在项目的风险区域添加风险</p></li>
   <li><p>Prime或更高版本，以便在项目的商业论证中添加风险</p></li></ul>
   <p>传统计划：任何计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td> <p>当前：标准 </p>
   <p>旧版：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>编辑对项目和财务数据的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p> 管理权限包括管理要为其创建或编辑风险的项目的财务 </p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建和编辑业务案例中的风险

您可以在规划项目的业务案例时创建风险。 例如，当概率、缓解计划或成本发生更改时，您可在业务案例中编辑它们。 有关创建业务案例的信息，请参阅[为项目创建业务案例](../../../manage-work/projects/define-a-business-case/create-business-case.md)。

您的Workfront管理员或组管理员必须在“项目首选项”区域的业务案例中启用&#x200B;**风险**&#x200B;部分，然后才能在“业务案例”部分的项目级别查看。 有关设置项目首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

在业务案例中创建和编辑风险是相同的。

要在业务案例中创建或编辑风险，请执行以下操作：

1. 转到要为其创建风险的项目。
1. 单击左侧面板中的&#x200B;**业务案例**。
1. 在&#x200B;**风险**&#x200B;部分中，单击&#x200B;**编辑风险**。
1. 输入或编辑以下信息：

   * **描述：**&#x200B;描述风险。

   * **潜在成本**：表示如果发生风险，则估计成本。

   * **概率**：以百分比值表示风险发生的概率。

   * **类型：**&#x200B;指示风险所属的类别。
   * **缓解计划**：更新计划的描述以缓解风险。

   * **缓解成本**：指示为防止风险发生而必须实施的缓解计划的成本。

   ![风险](assets/crp1-350x117.png)

1. （可选）单击&#x200B;**添加其他风险**&#x200B;以添加其他风险。
1. 单击&#x200B;**保存**。

## 在“风险”区域中创建和编辑风险

除了在业务案例中创建和编辑风险之外，您还可以使用项目的&#x200B;**风险**&#x200B;部分来执行该操作。

您可以在项目或模板的风险分区中创建和编辑风险。 为模板创建风险与为项目创建风险是相同的。

### 在风险区域创建风险 {#create-risks-in-the-risks-area}

1. 转到要为其创建风险的项目。
1. 单击左侧面板中的&#x200B;**风险**。

   任务![&#128279;](assets/risks-section-on-project-2022.png)的风险部分

1. 单击&#x200B;**开始添加风险**&#x200B;并通过内联编辑其信息来创建风险。 **描述**&#x200B;是必填字段

   或

   单击&#x200B;**新风险**。

   将打开&#x200B;**新风险**&#x200B;框。

   ![新风险框](assets/new-risk-box.png)

1. （视情况而定）如果在&#x200B;**新风险**&#x200B;框中添加风险，请输入以下信息：

   * **描述**：描述风险。 这是必填字段。
   * **风险类型**：指示风险所属的类别。\
     您的Workfront管理员定义环境中可用的风险类型。 有关定义风险类型的信息，请参阅文章[编辑和创建风险类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md)。

   * **概率**：以百分比值表示风险发生的概率。
   * **潜在成本**：表示如果发生风险，则指示估计成本。
   * **缓解成本**：指明为防止风险发生而必须实施的缓解计划的成本。
   * **实际成本**：指示风险发生时的实际风险成本。
   * **缓解计划**：更新计划的描述以缓解风险。

1. （视情况而定）如果您正在创建内联风险，请单击&#x200B;**Enter**。

   或

   如果您正在编辑&#x200B;**新风险**&#x200B;框中的信息，请单击&#x200B;**保存**。

1. （可选）在为风险列表应用&#x200B;**Standard**&#x200B;视图时，在&#x200B;**Status**&#x200B;下拉菜单中，为风险选择其他&#x200B;**Status**。

   默认情况下，风险的&#x200B;**状态**&#x200B;为&#x200B;**已识别**。

### 在“风险”区域中编辑风险 {#edit-risks-in-the-risks-area}

例如，当项目的概率、潜在成本或状态发生变化时，您可以编辑项目生命过程中的风险。

您可以一次编辑一个风险，也可以批量编辑多个风险。

要编辑风险，请执行以下操作：

1. 导航到要编辑现有风险的项目。
1. 单击左侧面板中的&#x200B;**风险**。
1. 开始内联编辑您在列表中看到的风险的字段，以一次编辑一个风险。

   或

   选择一个或多个风险，然后单击&#x200B;**编辑**&#x200B;以同时编辑多个风险。

   >[!NOTE]
   >
   >当您同时编辑多个风险时，会将相同的信息应用于所有选定的风险。 在更改之前，与每个风险相关的信息将以批量编辑方式覆盖。

1. 如果您已单击&#x200B;**编辑**，则会打开&#x200B;**编辑风险**&#x200B;或&#x200B;**编辑风险**&#x200B;框。

   请考虑编辑以下字段：

   * **描述**：编辑风险的描述。
   * **风险类型**：指示风险所属的类别。
   * **概率**：以百分比值表示风险发生的概率。
   * **潜在成本**：表示如果发生风险，则指示估计成本。
   * **缓解成本**：指明为防止风险发生而必须实施的缓解计划的成本。
   * **实际成本**：指示风险发生时的实际风险成本。
   * **缓解计划**：更新计划的描述以缓解风险。

1. 单击&#x200B;**保存**。
1. （可选）为风险列表应用&#x200B;**标准**&#x200B;视图时，在&#x200B;**状态**&#x200B;下拉菜单中编辑风险的&#x200B;**状态**。

   >[!NOTE]
   >
   >您无法在&#x200B;**编辑风险**&#x200B;对话框中编辑风险的&#x200B;**状态**。 您只能在内联编辑中执行此操作。
