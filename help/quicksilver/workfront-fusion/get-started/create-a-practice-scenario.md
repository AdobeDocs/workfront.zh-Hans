---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在Adobe Workfront Fusion中创建实践集成方案
description: 本文介绍了如何创建与Adobe Workfront Fusion的集成方案。 集成方案将不同的应用程序连接在一起，从而允许您的数据通过不同的应用程序流动。
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中创建实践集成方案

本文介绍了如何创建与Adobe Workfront Fusion的集成方案。 集成方案将不同的应用程序连接在一起，从而允许您的数据通过不同的应用程序流动。

要创建集成方案，您的组织必须具有 [!DNL Workfront Fusion for Work Automation and Integration] 许可证。

有关构建仅限Workfront的自动化方案的说明，请参阅 [在Adobe Workfront Fusion中创建实践自动化方案](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

有关Workfront Fusion许可证的更多信息，请参阅 [Adobe Workfront Fusion许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>贵组织可能不允许访问Google工作表。 如果出现这种情况，您将无法设置此集成，但此处提供的信息可用作集成方案功能的一般示例。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

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
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 创建实践方案

的角色 [!DNL Adobe Workfront Fusion] 是自动执行您的流程，以便您能够专注于新任务，而不是一遍又一遍地重复相同的任务。 它可以通过在应用程序和服务内部以及之间链接操作来工作，从而创建一种可自动传输和转换数据的方案。 您创建的方案会监控应用程序或服务中的数据，并处理该数据以提供所需的结果。

方案由一系列模块组成，这些模块指示数据应如何在应用程序内进行转换或在应用程序和Web服务之间进行传输。

在您学习如何使用时，说明如何创建情景并强化最佳实践 [!DNL Workfront Fusion]，本文将分步介绍该过程。 我们将创建一个方案，在 [!DNL Workfront] 每一行 [!DNL Google Sheets] 电子表格。

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>如果您有一个电子表格，其中列出了需要在中使用项目来处理的项目，则此类情景将非常有用 [!DNL Workfront]. 此方案可以“观看”电子表格中的新行，并在 [!DNL Workfront] 每一个。

创建方案包含几个主要任务：

## 选择应用程序并命名方案

1. 下载此 [电子表格](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)，然后将其上传到 [!DNL Google Drive] ，以便在本练习中使用。

   或

   创建或查找您自己的简单 [!DNL Google Sheets] 与此类似的电子表格：

   ![](assets/spreadsheet-headers-350x55.png)

1. 登录 [!DNL Workfront Fusion] 帐户。
1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) 中。

   在显示的左侧面板中，您可以将方案组织到文件夹中。

   在右侧主区域的顶部，您可以查看 **[!UICONTROL 全部]** 您构建的方案，您的 **[!UICONTROL 活动方案]** 和 **[!UICONTROL 不活动方案]**&#x200B;和 **[!UICONTROL 概念]**，这些情况在之前需要进一步处理 [!DNL Workfront Fusion] 可以将其分类为活动或不活动。

   ![](assets/scenarios-left-panel-350x215.png)

1. 在左侧面板中，单击 **[!UICONTROL 添加文件夹]** 图标 ![](assets/add-folder-icon.png)，然后为第一个文件夹键入“实践方案”等名称。

1. 打开文件夹，然后单击 **[!UICONTROL 创建新方案]** 的双曲余切值。

   显示的登陆页面允许您预加载要在要构建的方案中使用的任何应用程序。

1. 对于本练习，请搜索并选择 **[!UICONTROL Google工作表]** 应用程序。
1. 单击 **[!UICONTROL 继续]** 中。

   此时会显示方案编辑器，其中心包含一个空模块，即 [!DNL Google Sheets] 应用程序，以及底部工具栏中的一些选项。

   ![](assets/scenario-editor-350x235.png)

   当您开始创建新方案时，最好首先为其创建一个名称。

1. 选择 **[!UICONTROL 新方案]** 占位符名称，然后键入一个名称，如“练习方案1”。
1. 继续 [添加和配置第一个模块](#add-and-configure-the-first-module) 下。

## 添加和配置第一个模块

带有问号的空模块表示您需要添加的触发器模块。 此模块每次运行时将启动该方案。 空模块上的时钟图标指示是计划的模块。

![](assets/empty-module.png)

此模块将包含您希望方案监视的数据。

1. 单击空模块以选择要从中选择模块的应用程序。

   您之前预加载的应用程序将显示在空模块旁边。 您可以使用 [!UICONTROL 搜索] 框中。

   ![](assets/pre-loaded-apps-350x139.png)

1. 单击 **[!DNL Google Sheets]**.

   列表将更改为显示所有 [!DNL Google Sheets] 模块。

1. 单击触发器模块 **[!UICONTROL 监视记录]**.

   现在，您需要建立与Google帐户的已验证连接。 您添加到方案的每个模块都必须具有与其应用程序的连接。

1. 在 **[!DNL Google Sheets]** 框中 **[!UICONTROL 连接]**，单击 **[!UICONTROL 添加]**，然后键入连接的名称，如“Olivia&#39;s Google account”，然后单击 **[!UICONTROL 继续]**.
1. 在显示的窗口中验证连接。

   验证连接的过程在应用程序之间可能会有所不同。 您可能需要登录到应用程序。 您通常需要单击 **[!UICONTROL 允许]** 按钮。 如果您需要帮助，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 到应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 配置第一个模块

连接后 [!DNL Workfront Fusion] 至 [!DNL Google Sheets] 帐户，您可以指定 [!DNL Google Sheets] 您有权访问的电子表格以及您希望第一个模块处理的数据。

1. 单击 **[!UICONTROL 电子表格]** 框中，然后选择 **[!UICONTROL Workfront融合实践场景] #1** 显示列表中的电子表格。

   此电子表格包含2个工作表（制表符），因此我们需要指定包含所需数据的工作表：

1. 在 **[!UICONTROL 工作表]** 下拉列表中，选择 **[!UICONTROL 项目]**.

   我们的电子表格中包含标题，我们希望模块能够使用这些标题来标识我们要处理的数据：

   ![](assets/spreadsheet-headers-350x55.png)

1. 离开 **[!UICONTROL 是]** 已选 **[!UICONTROL 表包含标题]**.

1. 在 **[!UICONTROL 包含标题的行]** 框中，您可以指定要包含的行范围，但是我们将此练习的默认A1:Z1保留在此处。
1. 在 **[!UICONTROL 限制]** 框中，键入1。

   这样，每次运行方案时，模块都只会处理电子表格中的1行。 在构建方案时，这对于简化测试运行非常有用。

1. 单击 **[!UICONTROL 确定]**.

   的 **[!UICONTROL 选择开始位置]** 框会提示您指定希望模块开始处理的电子表格位置。

1. 单击 **[!UICONTROL 手动选择]**，在显示的列表中选择顶部选项，然后单击 **[!UICONTROL 确定]**.
1. 右键单击模块，单击 **[!UICONTROL 重命名]**，然后键入描述您希望模块执行的操作的名称（如“观看项目列表”），然后单击 **[!UICONTROL 确定]**.

   该名称显示在模块的正下方。 在这之下， [!DNL Workfront Fusion] 包括对模块所执行操作类型的简要说明。

   ![](assets/module-renamed-350x388.png)

1. 继续 [添加和配置第二个模块](#add-and-configure-the-second-module).

## 添加和配置第二个模块

1. 单击模块右侧的部分圆圈可 **[!UICONTROL 添加其他模块]**.

   第二个模块需要 [!DNL Workfront] 模块，但我们没有预加载 [!DNL Workfront] 应用程序。

1. 查找 [!DNL Workfront] 应用程序，开始键入“[!DNL Workfront]“ ”，然后在出现该应用程序时单击该应用程序。
1. 在 [!DNL Workfront] 出现的模块，单击 **[!UICONTROL 创建记录]**.

1. 正如您之前在Google工作表应用程序中所做的那样，单击 **[!UICONTROL 添加]** 在 [!DNL Workfront] 框中，可在Workfront Fusion和Workfront之间添加连接。

   现在，我们将开始指定要处理电子表格中数据的方式。

1. 单击 **[!UICONTROL 记录类型]**，然后选择 **[!UICONTROL 项目]** 因为我们想在 [!DNL Workfront] 使用电子表格中的某行。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 项目]** 在列表中开始键入“[!UICONTROL 项目].&quot;

   此框将展开以显示所有可用的 [!DNL Workfront] 项目字段中，您可以放置第一个模块找到的信息。

   我们将使用 **[!UICONTROL 名称]** 字段：我们希望此模块将 [!DNL Workfront] 在 [!UICONTROL Google工作表] 行。

1. 查找并单击 **[!UICONTROL 名称]** 字段。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] 操作系统)或 **Ctrl-F**([!DNL Windows] 操作系统)以快速查找字段。

   此时将打开可在 **[!UICONTROL 名称]** 字段，以定义在Workfront中创建的每个项目的名称。

   ![](assets/list-of-available-variables-350x261.png)

   请注意，列表顶部附近的变量与电子表格中的列标题相对应。

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 单击变量 **[!UICONTROL 我的项目名称(A)]** 将其添加到 **[!UICONTROL 名称]** 字段。

   您刚刚为此方案映射了第一段数据。

   让我们将电子表格中的另一段数据映射到 [!DNL Workfront]:每个项目的开始日期。

1. 查找并单击 **[!UICONTROL 计划开始日期]** 字段，然后单击 **[!UICONTROL 计划开始日期(E)]** 变量，以从电子表格中的该列提取数据。

1. 单击 **[!UICONTROL 确定]**.

   现在，您有一个工作方案。

1. 为第二个模块指定一个名称，如“创建Workfront项目”，然后继续 [测试方案](#test-the-scenario).

## 测试方案

在激活方案之前，请务必至少运行一次并查看结果以对其进行测试。 这有助于您了解数据如何在情景中流动，并查找任何错误。

我们选择处理电子表格中的1行，以在Workfront中创建项目。 如果运行方案，则应该出现这种情况。

1. 单击 **[!UICONTROL 运行一次]** 位于方案编辑器的左下角。
1. 在方案完成运行后，单击 [!DNL Google Sheets] 模块。

   ![](assets/click-bubble.png)

   在显示的框中，您可以查看有关模块处理的数据包的信息，包括从电子表格中提取的您开始使用的行的实际数据。

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. 单击 [!DNL Workfront] 模块，用于查看信息的输入和输出，该ID是现在在 [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   您可以在以下文章中了解有关如何阅读情景执行信息的更多信息：

   * 有关一般信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 有关已处理包的信息，请参阅 [方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 转到 [!DNL Workfront] 搜索“soho down loft”，看看情景所创造的项目。 这是电子表格中的最后一行。
1. 在 [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** ![](assets/save-icon.png) 在左下角附近，以保存对方案的进度。

   >[!IMPORTANT]
   >
   >在您了解和测试情景时，请经常进行保存。

## 完成方案并再次进行测试

我们仍需要配置方案，以便为电子表格中的所有其他行创建项目。

1. 单击 **[!UICONTROL 监视行]** 为Google工作表创建的模块。
1. 更改 **[!UICONTROL 限制]** 到100。

   指定一个大于您知道电子表格中行数的数字，可确保方案将捕获所有行。

1. 右键单击 **[!UICONTROL 监视行]** 模块，单击 **[!UICONTROL 选择开始位置]**，单击 **[!UICONTROL 全部]**，然后单击 **[!UICONTROL 确定]**.

1. 单击 **[!UICONTROL 运行一次]** 看看执行检查器气泡里发生了什么。

   的 [!DNL Google] 工作表 **[!UICONTROL 监视行]** 模块运行一次以读取所有行。 然后是Workfront **[!UICONTROL 创建记录]** 模块会运行20次，以为电子表格中剩余的20行中的每行创建一个项目。

1. 单击 [!DNL Workfront] 模块可查看所有20个操作，然后单击其中一个操作可查看有关所创建项目的信息。
1. 单击 **[!UICONTROL 保存]** ![](assets/save-icon.png) 在左下角附近。
1. 转到 [!DNL Workfront] 以查看方案创建的项目。

>[!TIP]
>
>我们建议您选择但有用的做法，来添加有关每个模块的注释。
>
>1. 右键单击 [!DNL Workfront] 模块，然后单击 **[!UICONTROL 添加注释]**.
>1. 在显示的注释中，键入模块的概述。

>
>   此功能非常有用，因为您无需持续打开模块即可查看其功能。 您可以键入类似“创建一个从电子表格映射的名称、计划开始日期和优先级的项目”。
>
>   对于 [!UICONTROL Google工作表] 模块中，您可以键入类似“为添加的新行/项目查看项目列表”的内容。
>
>   您可以为模块添加多个注释。
>
>1. 关闭 **[!UICONTROL 注释]** 的上界。
>
>   向方案添加注释后， **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 位于方案编辑器底部。
>
>1. 单击 **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 查看注释。

>




## 激活方案

如果您要对实际数据使用这种情况，您最不要做的就是激活它。 在激活方案后，默认情况下，每15分钟运行一次方案。 您可以通过定义您希望何时以及多久运行一次来更改此设置。

有关激活方案的更多信息，请参阅 [在Adobe Workfront Fusion中激活或停用方案](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

有关计划的信息，请参阅 [在Adobe Workfront Fusion中计划方案](../../workfront-fusion/scenarios/schedule-a-scenario.md).
