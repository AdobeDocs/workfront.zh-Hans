---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在Adobe Workfront Fusion中创建实践集成场景
description: 本文介绍了如何使用Adobe Workfront Fusion创建集成场景。 集成方案将不同的应用程序连接在一起，允许您的数据通过不同的应用程序流动。
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 99a8ad82c5fb2fb3f6adce9ff037086523be9b02
workflow-type: tm+mt
source-wordcount: '2094'
ht-degree: 0%

---

# 在Adobe Workfront Fusion中创建实践集成场景

本文介绍了如何使用Adobe Workfront Fusion创建集成场景。 集成方案将不同的应用程序连接在一起，允许您的数据通过不同的应用程序流动。

要创建集成方案，您的组织必须具有 [!DNL Workfront Fusion for Work Automation and Integration] 许可证。

有关构建仅限Workfront的自动化方案的说明，请参阅 [在Adobe Workfront Fusion中创建实践自动化场景](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

有关Workfront Fusion许可证的更多信息，请参阅 [Adobe Workfront Fusion许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>您的组织可能不允许访问Google工作表。 如果是这种情况，您将无法设置此集成，但此处显示的信息可用作集成方案如何工作的常规示例。

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
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 创建实践场景

的作用 [!DNL Adobe Workfront Fusion] 是自动化您的流程，以便您可以专注于新任务，而不是反复重复相同的任务。 它的工作方式是关联应用程序和服务内及其之间的操作，以创建自动传输和转换数据的方案。 您创建的场景将监视应用程序或服务中的数据，并处理该数据以提供您想要的结果。

场景由一系列模块组成，这些模块指示应如何在应用程序内转换数据或在应用程序和Web服务之间传输数据。

在学习使用时解释如何创建场景并强化最佳实践 [!DNL Workfront Fusion]，本文将逐步引导您完成此过程。 我们将创建一个方案，在其中创建新记录 [!DNL Workfront] 每行 [!DNL Google Sheets] 电子表格。

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>如果您有一个电子表格，其中列出了需要在中使用项目时需要处理的项目，则此类方案会很有用 [!DNL Workfront]. 该场景可以“监视”电子表格中的新行并在中添加新项目 [!DNL Workfront] 每一个。

创建场景由几个主要任务组成：

## 选择应用程序并命名方案

1. 下载此 [电子表格](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)，然后将其上传到 [!DNL Google Drive] 供在整个练习中使用。

   或

   创建或找到您自己的简单 [!DNL Google Sheets] 类似于下面的电子表格：

   ![](assets/spreadsheet-headers-350x55.png)

1. 登录您的 [!DNL Workfront Fusion] 帐户。
1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) （在左侧面板中）。

   >[!NOTE]
   >
   >如果您看不到左侧导航面板或其图标，请单击菜单 ![菜单](assets/main-menu-icon-left-nav.png) 图标。

   在灰色中 [!UICONTROL 文件夹] 在显示的面板中，您可以将方案整理到文件夹中。

   在主区域右上方，您可以查看 **[!UICONTROL 全部]** 您构建的方案，您的 **[!UICONTROL 活动方案]** 和 **[!UICONTROL 非活动方案]**、和 **[!UICONTROL 概念]**，这些之前需要执行更多操作的场景 [!DNL Workfront Fusion] 可将它们分类为活动或非活动。

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. 在 [!UICONTROL 文件夹] 面板中，单击 **[!UICONTROL 添加文件夹]** 图标 ![](assets/add-folder-icon.png)，然后为第一个文件夹键入一个名称，如“Practice scenarios”。

1. 打开文件夹，然后单击 **[!UICONTROL 创建新方案]** 页面右上角的。

   显示的登陆页面允许您预加载要在要构建的方案中使用的任何应用程序。

1. 在本练习中，搜索并选择 **[!UICONTROL Google工作表]** 应用程序。
1. 单击 **[!UICONTROL 继续]** 在右上角。

   随后将显示方案编辑器，其中心包含一个空模块， [!DNL Google Sheets] ，以及底部工具栏中的一些选项。

<!--
   ![](assets/scenario-editor-350x235.png)
-->

当您开始创建新场景时，最好先为其创建一个名称。

1. 选择 **[!UICONTROL 新方案]** 左上角的占位符名称，然后键入诸如“实践场景1”之类的名称。
1. 继续使用 [添加并配置第一个模块](#add-and-configure-the-first-module) 下面的。

## 添加并配置第一个模块

带问号的空模块表示您需要添加的触发器模块。 此模块将在每次运行时启动该方案。 空模块上的时钟图标表示是计划的模块。

![](assets/empty-module.png)

此模块将包含您希望场景关注的数据。

1. 单击空模块以选择要从中选择模块的应用程序。

   您之前预加载的应用程序显示在空模块旁边。 您可以使用添加任何具有模块的其他应用程序。 [!UICONTROL 搜索] 盒子。

   ![](assets/pre-loaded-apps-350x139.png)

1. 单击 **[!DNL Google Sheets]**.

   列表更改为全部显示 [!DNL Google Sheets] 可用作触发器模块的模块。

1. 单击触发器模块 **[!UICONTROL 留意记录]**.

   现在，您需要建立与您的Google帐户的经过身份验证的连接。 您添加到方案的每个模块都必须连接到其应用程序。

1. 在 **[!DNL Google Sheets]** 框，下 **[!UICONTROL 连接]**，单击 **[!UICONTROL 添加]**，然后键入连接的名称，如“Olivia的Google帐户”，然后单击 **[!UICONTROL 继续]**.
1. 在显示的窗口中验证连接。

   对连接进行身份验证的过程在应用程序之间可能会有所不同。 您可能需要登录到应用程序。 您通常需要单击 **[!UICONTROL 允许]** 按钮。 如果您需要帮助，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 配置第一个模块

连接后 [!DNL Workfront Fusion] 敬您的 [!DNL Google Sheets] 帐户，您可以指定 [!DNL Google Sheets] 您可以访问的电子表格以及您希望第一个模块处理的数据。

1. 单击 **[!UICONTROL 电子表格]** 框中，然后选择 **[!UICONTROL Workfront Fusion实践场景] #1** 在显示的列表中显示电子表格。

   此电子表格包含2个工作表（选项卡），因此我们需要指定包含所需数据的工作表：

1. 在 **[!UICONTROL 工作表]** 下拉列表，选择 **[!UICONTROL 项目]**.

   我们的电子表格包含标头，我们希望模块使用它们来标识要处理的数据：

   ![](assets/spreadsheet-headers-350x55.png)

1. 离开 **[!UICONTROL 是]** 选定对象 **[!UICONTROL 表包含标头]**.

1. 在 **[!UICONTROL 具有标题的行]** 框中，您可以指定要包含的行的范围，但在本练习中，我们将保留默认的A1：Z1。
1. 在 **[!UICONTROL 限制]** 框，键入1。

   这样，每次运行场景时，模块将只处理电子表格中的1行。 这对于在构建场景时简化测试运行非常有用。

1. 单击 **[!UICONTROL 确定]**.

   此 **[!UICONTROL 选择开始位置]** 框提示您指定您希望模块开始处理的电子表格位置。

1. 单击 **[!UICONTROL 手动选择]**，选择显示的列表中的顶部选项，然后单击 **[!UICONTROL 确定]**.
1. 右键单击模块，然后单击 **[!UICONTROL 重命名]**，然后键入一个名称，该名称用于描述您希望模块执行的操作（例如“观看项目列表”），然后单击 **[!UICONTROL 确定]**.

   该名称显示在模块正下方。 在那个下面， [!DNL Workfront Fusion] 包含模块所执行操作类型的简短描述。

   ![](assets/module-renamed-350x388.png)

1. 继续使用 [添加并配置第二个模块](#add-and-configure-the-second-module).

## 添加并配置第二个模块

1. 单击模块右侧的部分圆圈，以 **[!UICONTROL 添加另一个模块]**.

   第二个模块需要是 [!DNL Workfront] 模块，但我们没有预加载 [!DNL Workfront] 应用程序。

1. 要查找 [!DNL Workfront] 应用程序，开始键入»[!DNL Workfront]”并在应用程序出现时单击它。
1. 在列表中 [!DNL Workfront] 模块后，单击 **[!UICONTROL 创建记录]**.

1. 与以前使用Google Sheets应用程序时一样，单击 **[!UICONTROL 添加]** 在 [!DNL Workfront] 框，用于在Workfront Fusion和Workfront之间添加连接。

   现在，我们将开始指定要如何处理电子表格中的数据。

1. 单击 **[!UICONTROL 记录类型]**，然后选择 **[!UICONTROL 项目]** 因为我们要在中创建一个项目 [!DNL Workfront] 使用电子表格中的行。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 项目]** 在列表中(如果您开始键入“[!UICONTROL 项目].”

   该框将展开以显示所有可用的 [!DNL Workfront] 可在其中放入第一个模块找到的信息的项目字段。

   我们将使用 **[!UICONTROL 名称]** 字段：我们希望此模块命名中的各个项目 [!DNL Workfront] 使用对应文档中的文本 [!UICONTROL Google工作表] row。

1. 查找并单击 **[!UICONTROL 名称]** 字段。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F**([!DNL Windows] OS)以快速找到字段。

   这将打开可在以下位置使用的变量列表： **[!UICONTROL 名称]** 字段，用于定义在Workfront中创建的每个项目的名称。

   ![](assets/list-of-available-variables-350x261.png)

   请注意，列表顶部附近的变量对应于电子表格中的列标题。

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 单击变量 **[!UICONTROL 我的项目名称(A)]** 以将其添加到 **[!UICONTROL 名称]** 字段。

   您刚刚为此方案映射了您的第一段数据。

   让我们将电子表格中的一段数据映射到 [!DNL Workfront]：每个项目的开始日期。

1. 查找并单击 **[!UICONTROL 计划开始日期]** 字段，然后单击 **[!UICONTROL 计划开始日期(E)]** 变量来提取电子表格中该列的数据。

1. 单击 **[!UICONTROL 确定]**.

   现在您有一个工作方案。

1. 为第二个模块命名，例如“创建Workfront项目”，然后继续 [测试场景](#test-the-scenario).

## 测试场景

在激活场景之前，请务必至少运行一次场景并查看结果以测试场景。 这有助于您了解数据如何在场景中流动并查找任何错误。

我们选择处理电子表格中的1行，以便在Workfront中创建项目。 如果您运行该方案，则应该出现这种情况。

1. 单击 **[!UICONTROL 运行一次]** （在场景编辑器的左下角）。
1. 方案运行完毕后，单击 [!DNL Google Sheets] 模块。

   ![](assets/click-bubble.png)

   在显示的框中，您可以查看有关模块处理的数据包的信息，包括从电子表格中为开始使用的行提取的实际数据。

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. 单击上方的执行检查器气泡 [!DNL Workfront] 模块以查看信息的输入和输出，它是现在在中创建的项目的ID [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   您可以在以下文章中了解有关如何读取场景执行信息的更多信息：

   * 有关一般信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 有关已处理捆绑包的信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 转到 [!DNL Workfront] 搜索“soho downtown loft”，查看场景创建的项目。 这是电子表格中的最后一行。
1. In [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** ![](assets/save-icon.png) 左下角附近，保存场景进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

## 最终确定方案并再次进行测试

我们仍需要配置场景以便为电子表格中的所有其他行创建项目。

1. 单击 **[!UICONTROL 监视行]** 您为Google Sheets创建的模块。
1. 更改 **[!UICONTROL 限制]** 到100。

   在电子表格中指定一个大于已知行数的数字，可确保方案捕获所有这些行。

1. 右键单击 **[!UICONTROL 监视行]** 模块，单击 **[!UICONTROL 选择开始位置]**，单击 **[!UICONTROL 全部]**，然后单击 **[!UICONTROL 确定]**.

1. 单击 **[!UICONTROL 运行一次]** 观察执行检查器气泡中发生的情况。

   此 [!DNL Google] 工作表 **[!UICONTROL 监视行]** 模块运行一次以读取所有行。 然后是Workfront **[!UICONTROL 创建记录]** 模块运行20次，以便为电子表格中剩余的20行中的每一行创建一个项目。

1. 单击的执行检查器气泡， [!DNL Workfront] 模块以查看所有20项操作，然后单击其中一个操作以查看有关所创建项目的信息。
1. 单击 **[!UICONTROL 保存]** ![](assets/save-icon.png) 左下角附近。
1. 转到 [!DNL Workfront] 以查看场景创建的项目。

>[!TIP]
>
>我们建议您选择添加有关每个模块的注释这一可选但有用的做法。
>
>1. 右键单击 [!DNL Workfront] 模块，然后单击 **[!UICONTROL 添加注释]**.
>1. 在显示的注释中，键入模块的概述。
>
>    这非常有用，因为您无需持续打开模块即可查看其功能。 您可以键入类似于“创建项目，其名称、计划开始日期和优先级均映射自电子表格”的内容。
>
>    对于 [!UICONTROL Google工作表] 模块时，您可以键入诸如“关注添加的新行/项目的项目列表”之类的内容。
>
>    您可以为一个模块添加多个注释。
>
>1. 关闭 **[!UICONTROL 注释]** 区域。
>
>    向方案添加注释后，上会显示一个橙色圆点 **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 位于场景编辑器的底部。
>
>1. 单击 **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 以查看您的注释。
>



## 激活方案

如果这是您用于真实数据的场景，您最不想做的就是激活它。 在激活某个方案后，默认情况下，它每15分钟运行一次。 您可以通过定义运行时间和频率来更改此值。

有关激活方案的更多信息，请参阅 [在Adobe Workfront Fusion中激活或取消激活场景](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

有关时间表的信息，请参阅 [在Adobe Workfront Fusion中计划场景](../../workfront-fusion/scenarios/schedule-a-scenario.md).
