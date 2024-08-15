---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在Adobe Workfront Fusion中创建实践集成场景
description: 本文介绍了如何使用Adobe Workfront Fusion创建集成场景。 集成方案将不同的应用程序连接在一起，允许您的数据通过不同的应用程序流动。
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: cb4edb02aad8a0738ea80f058fcc2bc016832ce1
workflow-type: tm+mt
source-wordcount: '2139'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中创建实践集成场景

本文介绍了如何使用Adobe Workfront Fusion创建集成场景。 集成方案将不同的应用程序连接在一起，允许您的数据通过不同的应用程序流动。

要创建集成方案，您的组织必须具有[!DNL Workfront Fusion for Work Automation and Integration]许可证。

有关构建仅限Workfront的自动化方案的说明，请参阅[在Adobe Workfront Fusion中创建实践自动化方案](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

有关Workfront Fusion许可证的详细信息，请参阅[Adobe Workfront Fusion许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

>[!NOTE]
>
>您的组织可能不允许访问Google工作表。 如果是这种情况，您将无法设置此集成，但此处显示的信息可用作集成方案如何工作的一般示例。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 创建实践场景

[!DNL Adobe Workfront Fusion]的作用是自动化您的流程，以便您能够专注于新任务，而不是重复相同的任务。 它的工作方式是，关联应用程序和服务内外的操作，从而创建一个自动传输和转换数据的方案。 您创建的方案会监视应用程序或服务中的数据，并对这些数据进行处理以提供您想要的结果。

场景由一系列模块组成，这些模块指示应如何在应用程序内转换数据或在应用程序和Web服务之间传输数据。

为了说明如何在学习使用[!DNL Workfront Fusion]时创建场景并强化最佳实践，本文逐步引导您完成该过程。 我们将创建一个方案，以在[!DNL Workfront]中为[!DNL Google Sheets]电子表格中的每一行创建新记录。

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>如果您有一个电子表格列出需要在[!DNL Workfront]中使用项目时处理的项目，则此类方案会很有用。 该场景可以“监视”电子表格中的新行，并在[!DNL Workfront]中为每个行添加新项目。

创建方案由若干主要任务组成：

## 选择应用程序并命名方案

1. 下载此[电子表格](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)，然后将其上传到您的[!DNL Google Drive]以供在整个练习中使用。

   或

   创建或查找您自己的类似[!DNL Google Sheets]的电子表格：

   ![](assets/spreadsheet-headers-350x55.png)

1. 登录您的[!DNL Workfront Fusion]帐户。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]** ![](assets/scenarios-icon.png)。

   >[!NOTE]
   >
   >如果未看到左侧导航面板或其图标，请单击菜单![菜单](assets/main-menu-icon-left-nav.png)图标。

   在显示的灰色[!UICONTROL 文件夹]面板中，您可以将方案整理到文件夹中。

   在右侧主区域顶部，您可以查看已构建的&#x200B;**[!UICONTROL 所有]**&#x200B;方案、**[!UICONTROL 活动方案]**&#x200B;和&#x200B;**[!UICONTROL 非活动方案]**&#x200B;以及&#x200B;**[!UICONTROL 概念]**，这些方案需要更多工作，然后[!DNL Workfront Fusion]才能将其分类为活动或非活动。

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. 在[!UICONTROL 文件夹]面板中，单击&#x200B;**[!UICONTROL 添加文件夹]**&#x200B;图标![](assets/add-folder-icon.png)，然后为第一个文件夹键入诸如“实践场景”之类的名称。

1. 打开文件夹，然后单击页面右上角的&#x200B;**[!UICONTROL 创建新方案]**。

   显示的登陆页面允许您预加载要在要构建的场景中使用的任何应用程序。

1. 在本练习中，搜索并选择&#x200B;**[!UICONTROL Google Sheets]**&#x200B;应用程序。
1. 单击右上角的&#x200B;**[!UICONTROL 继续]**。

   此时将显示方案编辑器，其中心包含一个空模块、预加载的[!DNL Google Sheets]应用程序以及底部工具栏中的一些选项。

<!--
   ![](assets/scenario-editor.png)
-->

当您开始创建新方案时，最好从为其创建名称开始。

1. 选择左上角的&#x200B;**[!UICONTROL 新方案]**&#x200B;占位符名称，然后键入诸如“实践方案1”之类的名称。
1. 继续[添加并配置下面的第一个模块](#add-and-configure-the-first-module)。

## 添加并配置第一个模块

带问号的空模块表示您需要添加的触发器模块。 此模块将在每次运行时启动方案。 空模块上的时钟图标表示是已计划的模块。

![](assets/empty-module.png)

此模块将包含您希望方案关注的数据。

1. 单击空模块以选择要从中选择模块的应用程序。

   之前预加载的应用程序显示在空模块旁边。 您可以使用[!UICONTROL 搜索]框添加任何具有模块的其他应用。

   ![](assets/pre-loaded-apps-350x139.png)

1. 单击 **[!DNL Google Sheets]**。

   列表将更改为显示所有可用作触发器模块的[!DNL Google Sheets]模块。

1. 单击触发器模块&#x200B;**[!UICONTROL 查看记录]**。

   现在，您需要建立与您的Google帐户的经过身份验证的连接。 您添加到方案的每个模块都必须与其应用程序建立连接。

1. 在&#x200B;**[!DNL Google Sheets]**&#x200B;框的&#x200B;**[!UICONTROL 连接]**&#x200B;下，单击&#x200B;**[!UICONTROL 添加]**，然后键入连接的名称，如“Olivia的Google帐户”，然后单击&#x200B;**[!UICONTROL 继续]**。
1. 在显示的窗口中验证连接。

   对连接进行身份验证的过程在应用程序之间可能会有所不同。 您可能需要登录到应用程序。 您通常需要单击&#x200B;**[!UICONTROL 允许]**&#x200B;按钮。 如果需要帮助，请参阅[连接概述](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)。

## 配置第一个模块

将[!DNL Workfront Fusion]连接到[!DNL Google Sheets]帐户后，您可以指定有权访问的[!DNL Google Sheets]电子表格以及您希望第一个模块处理的数据。

1. 单击&#x200B;**[!UICONTROL 电子表格]**&#x200B;框，然后在显示的列表中选择&#x200B;**[!UICONTROL Workfront Fusion实践方案] #1**&#x200B;电子表格。

   此电子表格包含2个工作表（选项卡），因此我们需要指定包含所需数据的工作表：

1. 在&#x200B;**[!UICONTROL 工作表]**&#x200B;下拉列表中，选择&#x200B;**[!UICONTROL 项目]**。

   我们的电子表格中包含标头，我们希望模块使用它们来标识要处理的数据：

   ![](assets/spreadsheet-headers-350x55.png)

1. 保留为&#x200B;**[!UICONTROL 表包含标头]**&#x200B;选择&#x200B;**[!UICONTROL 是]**。

1. 在&#x200B;**[!UICONTROL Row with headers]**&#x200B;框中，您可以指定要包含的行的范围，但让此练习保留默认的A1：Z1。
1. 在&#x200B;**[!UICONTROL Limit]**&#x200B;框中，键入1。

   这样，每次运行场景时，模块将仅处理电子表格中的1行。 这对于在构建场景时简化测试运行非常有用。

1. 单击&#x200B;**[!UICONTROL 确定]**。

   **[!UICONTROL 选择开始位置]**&#x200B;框提示您指定您希望模块开始处理的电子表格位置。

1. 单击“**[!UICONTROL 手动选择]**”，在显示的列表中选择顶部选项，然后单击“**[!UICONTROL 确定]**”。
1. 右键单击该模块，单击“**[!UICONTROL 重命名]**”，键入描述您希望该模块执行的操作的名称（如“监视项目列表”），然后单击“**[!UICONTROL 确定]**”。

   该名称显示在模块正下方。 在其下方，[!DNL Workfront Fusion]包含模块执行的操作类型的简要说明。

   ![](assets/module-renamed-350x388.png)

1. 继续[添加并配置第二个模块](#add-and-configure-the-second-module)。

## 添加并配置第二个模块

1. 单击模块右侧的部分圆圈以&#x200B;**[!UICONTROL 添加另一个模块]**。

   第二个模块需要是[!DNL Workfront]模块，但我们没有预加载[!DNL Workfront]应用程序。

1. 要查找[!DNL Workfront]应用程序，请开始键入“[!DNL Workfront]”，并在应用程序出现时单击该应用程序。
1. 在出现的[!DNL Workfront]模块列表中，单击&#x200B;**[!UICONTROL 创建记录]**。

1. 与以前使用Google Sheets应用程序时一样，单击[!DNL Workfront]框中的&#x200B;**[!UICONTROL 添加]**&#x200B;以在Workfront Fusion和Workfront之间添加连接。

   现在，我们将开始指定要如何处理电子表格中的数据。

1. 单击&#x200B;**[!UICONTROL 记录类型]**，然后选择&#x200B;**[!UICONTROL 项目]**，因为我们希望使用电子表格中的行在[!DNL Workfront]中创建项目。

   >[!TIP]
   >
   >如果您开始输入“[!UICONTROL 项目]”，则可以在列表中找到&#x200B;**[!UICONTROL 项目]**。

   该框将展开以显示所有可用的[!DNL Workfront]项目字段，您可以在其中放置第一个模块找到的信息。

   我们将使用&#x200B;**[!UICONTROL Name]**&#x200B;字段：我们希望此模块使用相应[!UICONTROL Google工作表]行中的文本来命名[!DNL Workfront]中的每个项目。

1. 查找并单击&#x200B;**[!UICONTROL 名称]**&#x200B;字段。

   >[!TIP]
   >
   >您可以使用&#x200B;**Cmd+F** （[!DNL Mac]操作系统）或&#x200B;**Ctrl-F**（[!DNL Windows]操作系统）快速查找字段。

   这将打开可在&#x200B;**[!UICONTROL 名称]**&#x200B;字段中使用的变量列表，以定义在Workfront中创建的每个项目的名称。

   ![](assets/list-of-available-variables-350x261.png)

   请注意，列表顶部附近的变量对应于电子表格中的列标题。

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 单击变量&#x200B;**[!UICONTROL 我的项目名称(A)]**&#x200B;以将其添加到&#x200B;**[!UICONTROL 名称]**&#x200B;字段。

   您刚刚为此方案映射了您的第一段数据。

   让我们将电子表格中的一段或多段数据映射到[!DNL Workfront]：每个项目的开始日期。

1. 查找并单击&#x200B;**[!UICONTROL 计划开始日期]**&#x200B;字段，然后单击&#x200B;**[!UICONTROL 计划开始日期(E)]**&#x200B;变量，以从电子表格中的该列提取数据。

1. 单击&#x200B;**[!UICONTROL 确定]**。

   现在您有一个可行的方案。

1. 为第二个模块命名，如“创建Workfront项目”，然后继续[测试方案](#test-the-scenario)。

## 测试场景

在激活方案之前，请务必至少运行一次方案并查看结果以对其进行测试。 这有助于您了解数据如何在场景中流动并查找任何错误。

我们选择处理电子表格中的1行，以便在Workfront中创建项目。 如果您运行场景，则应该发生这种情况。

1. 在方案编辑器的左下角单击&#x200B;**[!UICONTROL 运行一次]**。
1. 方案运行完毕后，单击[!DNL Google Sheets]模块上方的气泡。

   ![](assets/click-bubble.png)

   在显示的框中，您可以查看有关模块处理的数据包的信息，包括从电子表格中为开始使用的行提取的实际数据。

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. 单击[!DNL Workfront]模块上方的执行检查器气泡可查看信息输入和输出，它是现在在[!DNL Workfront]中创建的项目的ID

   ![](assets/execution-inspector-wf-350x384.png)

   您可在以下文章中了解有关如何读取场景执行信息的更多信息：

   * 有关一般信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[方案执行流程。
   * 有关已处理捆绑包的信息，请参阅[方案执行、周期和 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md)中的阶段。

1. 转到[!DNL Workfront]并搜索“soho downtown loft”以查看场景创建的项目。 这是电子表格中的最后一行。
1. 在[!DNL Workfront Fusion]中，单击左下角附近的&#x200B;**[!UICONTROL 保存]** ![](assets/save-icon.png)以保存方案进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 最终确定方案并再次进行测试

我们仍需要配置场景以便为电子表格中的所有其他行创建项目。

1. 单击您为Google Sheets创建的&#x200B;**[!UICONTROL 监视行]**&#x200B;模块。
1. 将&#x200B;**[!UICONTROL 限制]**&#x200B;更改为100。

   在电子表格中指定一个大于已知行数的数字，可确保方案捕获所有这些行。

1. 右键单击&#x200B;**[!UICONTROL 监视行]**&#x200B;模块，单击&#x200B;**[!UICONTROL 选择开始位置]**，单击&#x200B;**[!UICONTROL 全部]**，然后单击&#x200B;**[!UICONTROL 确定]**。

1. 单击&#x200B;**[!UICONTROL 运行一次]**&#x200B;并观察执行检查器气泡中发生的情况。

   [!DNL Google]表&#x200B;**[!UICONTROL 监视行]**&#x200B;模块运行一次，以读取所有行。 然后Workfront **[!UICONTROL 创建记录]**&#x200B;模块运行20次，为电子表格中剩余的20行中的每一行创建一个项目。

1. 单击[!DNL Workfront]模块的执行检查器气泡查看所有20个操作，然后单击其中一个操作查看有关所创建项目的信息。
1. 单击左下角附近的&#x200B;**[!UICONTROL 保存]** ![](assets/save-icon.png)。
1. 转到[!DNL Workfront]查看场景创建的项目。

>[!TIP]
>
>我们建议您选择添加有关每个模块的注释这一有用但可选的实践。
>
>1. 右键单击[!DNL Workfront]模块，然后单击&#x200B;**[!UICONTROL 添加备注]**。
>1. 在显示的注释中，键入模块的概述。
>
>    这很有用，因为您无需持续打开模块即可查看其功能。 您可以键入类似于“创建项目，该项目具有从电子表格映射的名称、计划开始日期和优先级”的内容。
>
>    对于[!UICONTROL Google Sheets]模块，您可以键入诸如“关注添加的新行/项目的项目列表”之类的内容。
>
>    您可以为一个模块添加多个注释。
>
>1. 关闭&#x200B;**[!UICONTROL 注释]**&#x200B;区域。
>
>    向方案添加注释后，方案编辑器底部的&#x200B;**[!UICONTROL 注释]**&#x200B;图标![](assets/notes-icon-w-dot.png)上会显示一个橙色点。
>
>1. 单击&#x200B;**[!UICONTROL 备注]**&#x200B;图标![](assets/notes-icon-w-dot.png)查看您的备注。
>



## 激活方案

如果这是您用于真实数据的场景，则您最不想做的就是激活它。 在激活方案后，默认情况下，它每15分钟运行一次。 您可以通过定义运行的时间和频率来更改此设置。

有关激活方案的详细信息，请参阅[在Adobe Workfront Fusion中激活或停用方案](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)。

有关计划的信息，请参阅[在Adobe Workfront Fusion中计划方案](../../workfront-fusion/scenarios/schedule-a-scenario.md)。
