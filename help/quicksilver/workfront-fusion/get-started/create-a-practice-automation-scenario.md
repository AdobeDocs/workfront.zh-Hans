---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在 [!DNL Adobe Workfront Fusion]
description: 本文介绍了如何使用Adobe Workfront Fusion创建自动化方案。 自动化方案可自动执行Workfront流程，包括数据操作和转换。 此示例将引导您完成创建一个方案的过程，该方案会搜索某个项目，然后返回与该项目关联的所有任务。
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1782'
ht-degree: 0%

---

# 在 [!DNL Adobe Workfront Fusion]

本文介绍了如何使用Adobe Workfront Fusion创建自动化方案。 自动化方案可自动执行Workfront流程，包括数据操作和转换。 此示例将引导您完成创建一个方案的过程，该方案会搜索某个项目，然后返回与该项目关联的所有任务。

有关构建可连接不同应用程序的集成方案的说明，请参阅 [在Adobe Workfront Fusion中创建实践集成方案](../../workfront-fusion/get-started/create-a-practice-scenario.md).

有关每个Workfront Fusion许可证所提供功能的更多信息，请参阅 [Adobe Workfront Fusion许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化）</p>  </td> 
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
此示例将引导您完成创建搜索 [!DNL Workfront] ，并返回项目中的任务。

![](assets/create-practice-scenario-wf-only-350x157.png)

创建方案包含几个主要任务：

## 选择应用程序并命名方案

1. 登录 [!DNL Workfront Fusion] 帐户。
1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) 中。

   在显示的左侧面板中，您可以将方案组织到文件夹中。

   在右侧主区域的顶部，您可以查看 **[!UICONTROL 全部]** 您构建的方案，您的 **[!UICONTROL 活动方案]**, **[!UICONTROL 不活动方案]**&#x200B;和 **[!UICONTROL 概念]**. 概念是指在之前需要执行更多操作的方案 [!DNL Workfront Fusion] 可以将其分类为活动或不活动。

   ![](assets/scenarios-left-panel-350x215.png)

1. 在左侧面板中，单击 **[!UICONTROL 添加文件夹]** 图标 ![](assets/add-folder-icon.png)，然后为第一个文件夹键入“实践方案”等名称。

1. 打开文件夹，然后单击 **[!UICONTROL 创建新方案]** 的双曲余切值。

   显示的登陆页面允许您预加载要在要构建的方案中使用的任何应用程序。

1. 对于本练习，请搜索并选择 **[!DNL Workfront]** 应用程序。
1. 单击 **[!UICONTROL 继续]** 中。

   此时会显示方案编辑器，其中心包含一个空模块，即 [!DNL Workfront] 应用程序，以及底部工具栏中的一些选项。

   ![](assets/scenario-editor-350x235.png)

   当您开始创建新方案时，最好首先为其创建一个名称。

1. 选择 **[!UICONTROL 新方案]** 占位符名称，然后键入一个名称，如“练习方案1”。
1. 继续 [添加和配置第一个模块](#add-and-configure-the-first-module) 下。

## 添加和配置第一个模块

带有问号的空模块表示您需要添加的触发器模块。 此模块每次运行时将启动该方案。 空模块上的时钟图标指示是计划的模块。

![](assets/empty-module.png)

此模块将包含您希望方案监视的数据。

在本例中，我们未使用触发器模块。 相反，此方案以搜索开始。

1. 单击空模块以选择要从中选择模块的应用程序。

   您之前预加载的应用程序将显示在空模块旁边。 您可以使用 [!UICONTROL 搜索] 框中。

   ![](assets/pre-loaded-app-wf-350x172.png)

1. 单击 **[!DNL Workfront]**.

   列表将更改为显示所有 [!DNL Workfront] 模块。

1. 单击搜索模块 **[!UICONTROL 搜索]**.

   现在，您需要建立与 [!DNL Workfront] 帐户。 您添加到方案的每个模块都必须具有与其应用程序的连接。

1. 在 **[!DNL Workfront]** 框中 **[!UICONTROL 连接]**，单击 **[!UICONTROL 添加]**，然后键入连接的名称，如“Olivia&#39;s Workfront account”，然后单击 **[!UICONTROL 继续]**.
1. 在显示的窗口中验证连接。

   验证连接的过程在应用程序之间可能会有所不同。 以下流程专用于 [!DNL Workfront]，但此过程与许多应用程序类似。

   1. 输入 [!DNL Workfront] 域，然后单击 **[!UICONTROL 继续]**.
   1. 登录 [!DNL Workfront].
   1. 检查 [!DNL Workfront Fusion] 请求，然后单击 **[!UICONTROL 允许访问]**.

   如果您需要帮助，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 到应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 配置第一个模块

连接后 [!DNL Workfront Fusion] 至 [!DNL Workfront] 帐户，您可以指定 [!DNL Workfront] 请求您有权访问的队列，以及您希望第一个模块处理的数据。

1. 在 [!UICONTROL 记录类型] 框，选择 **[!UICONTROL 项目]**. 这会将模块设置为仅搜索项目。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 项目]** 在列表中开始键入“[!UICONTROL 项目].&quot;

1. 在 **[!UICONTROL 结果集]** 框，选择 **[!UICONTROL 第一条匹配记录]**. 这会将模块设置为仅返回它找到的符合标准的第一个记录。 在本例中，我们只需要返回一条记录。
1. 在 **[!UICONTROL 搜索条件]** 区域，我们将设置一个过滤器以返回特定项目。

   1. 在 [!UICONTROL 搜索条件]，选择要搜索的值的字段。 对于此示例，请选择 **[!UICONTROL 名称]**.
   1. 对于运算符，选择 [!UICONTROL 包含（不区分大小写）]. 这样，即使您没有输入整个名称，或输入名称且大小写不正确（如全部大写），模块仍可以查找名称中包含您选择词语的项目。
   1. 在 [!UICONTROL 搜索条件]，请在要搜索的项目名称中输入您知道的单词或短语。

1. 在 **[!UICONTROL 输出]** 列表中，选择希望输出问题的字段。 在本例中，选择 **[!UICONTROL ID]** 和 **[!UICONTROL 名称]** 字段。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] 操作系统)或 **Ctrl-F** ([!DNL Windows] 操作系统)以快速查找字段。

1. 单击 **[!UICONTROL 确定]**.

   >[!NOTE]
   >
   >（仅限信息）由于这不是触发器模块，因此您不会选择启动该模块的位置。 使用触发器模块时，您现在可以选择启动该模块的位置。
   >
   >
   >有关更多信息，请参阅 [选择触发器模块的开始位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. 右键单击模块，单击 **[!UICONTROL 重命名]**，然后键入描述您希望模块执行的操作的名称（如“搜索项目”），然后单击 **[!UICONTROL 确定]**.

   该名称显示在模块的正下方。 在这之下， [!DNL Workfront Fusion] 包括对模块所执行操作类型的简要说明。

   ![](assets/module-renamed-wf.png)

1. 继续 [添加和配置第二个模块](#add-and-configure-the-second-module).

## 添加和配置第二个模块

1. 单击模块右侧的部分圆圈可 **[!UICONTROL 添加其他模块]**.
1. 选择 [!DNL Workfront] 从应用程序列表中，选择搜索模块 **[!UICONTROL 读取相关记录]**.
1. 您已创建与 [!DNL Workfront] 上一个模块。 您无需在此处再次创建该模块，但必须确保此模块使用与上一个模块相同的连接。\
   在 **[!UICONTROL 连接]** 框中，选择您为上一个模块创建的连接。
1. 单击 **[!UICONTROL 记录类型]**，然后选择 **[!UICONTROL 项目]**，因为我们希望读取与项目相关的记录。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 项目]** 在列表中输入“项目”。

1. 单击 **[!UICONTROL 父记录ID]** 字段。 此字段需要要从中返回任务的项目的Workfront ID。

   单击字段会打开可在 **[!UICONTROL 父记录ID]** 字段来标识Workfront中的项目。

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 单击变量 **[!UICONTROL ID]** 将其添加到 **[!UICONTROL 父记录ID]** 字段。 这允许将从第一个模块返回的ID用作要在第二个模块中处理的项目的标识符，从而确保返回的任务将属于该项目。
1. 在 **[!UICONTROL 收藏集]** 字段，选择 **[!UICONTROL 任务]**. 这表示模块将返回与所选项目关联的任务。
1. 单击 **[!UICONTROL 确定]**

   现在，您有一个工作方案。

1. 为第二个模块指定一个名称，如“返回与项目关联的任务”，然后继续 [测试方案](#test-the-scenario).

## 测试方案

在激活方案之前，请务必至少运行一次并查看结果以对其进行测试。 这有助于您了解数据如何在情景中流动，并查找任何错误。

我们选择返回1个项目，以及与该项目关联的任务。 如果运行方案，则应该出现这种情况。

1. 单击 **[!UICONTROL 运行一次]** 位于方案编辑器的左下角。
1. 在方案完成运行后，单击第一个模块上方的气泡。

   ![](assets/click-bubble.png)

   在显示的框中，您可以查看有关模块处理的数据包的信息，包括从模块返回的项目中提取的实际数据。

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 单击“第二个”模块上方的执行检查器气泡，可查看信息的输入和输出，这是项目中包含的任务集合。

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   您可以在以下文章中了解有关如何阅读情景执行信息的更多信息：

   * 有关一般信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 有关已处理包的信息，请参阅 [方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 在 [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** ![](assets/save-icon.png) 在左下角附近，以保存对方案的进度。

   >[!IMPORTANT]
   >
   >在您了解和测试情景时，请经常进行保存。

>[!TIP]
>
>我们建议您选择但有用的做法，来添加有关每个模块的注释。
>
>1. 右键单击 [!DNL Workfront] 模块，然后单击 **[!UICONTROL 添加注释]**.
>1. 在显示的注释中，键入模块的概述。

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

此示例方案没有触发器模块。 如果是这种情况，您会将其用于实际数据，它将从触发器模块开始，而您最后要做的就是激活它。 在激活方案后，默认情况下，每15分钟运行一次方案。 您可以通过定义您希望何时以及多久运行一次来更改此设置。

有关激活方案的更多信息，请参阅 [在 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

有关计划的信息，请参阅 [在中计划方案 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
