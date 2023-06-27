---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在中创建实践自动化方案 [!DNL Adobe Workfront Fusion]
description: 本文介绍了如何使用Adobe Workfront Fusion创建自动化场景。 自动化场景可自动化Workfront流程，包括数据操作和转换。 本示例将引导您完成创建方案的过程，该方案先搜索项目，然后返回与该项目关联的所有任务。
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 0%

---

# 在中创建实践自动化方案 [!DNL Adobe Workfront Fusion]

本文介绍了如何使用Adobe Workfront Fusion创建自动化场景。 自动化场景可自动化Workfront流程，包括数据操作和转换。 本示例将引导您完成创建方案的过程，该方案先搜索项目，然后返回与该项目关联的所有任务。

有关构建连接不同应用程序的集成方案的说明，请参阅 [在Adobe Workfront Fusion中创建实践集成场景](../../workfront-fusion/get-started/create-a-practice-scenario.md).

有关每个Workfront Fusion许可证可用功能的更多信息，请参阅 [Adobe Workfront Fusion许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>
要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 创建实践场景

的作用 [!DNL Adobe Workfront Fusion] 是自动化您的流程，以便您可以专注于新任务，而不是反复重复相同的任务。 它的工作方式是关联应用程序和服务内及其之间的操作，以创建自动传输和转换数据的方案。 您创建的场景将监视应用程序或服务中的数据，并处理该数据以提供您想要的结果。

场景由一系列模块组成，这些模块指示应如何在应用程序内转换数据或在应用程序和Web服务之间传输数据。
本示例将引导您完成创建场景的过程，该场景将搜索 [!DNL Workfront] 并返回项目中的任务。

![](assets/create-practice-scenario-wf-only-350x157.png)

创建场景由几个主要任务组成：

## 选择应用程序并命名方案

1. 登录您的 [!DNL Workfront Fusion] 帐户。
1. 单击 **[!UICONTROL 方案]** ![](assets/scenarios-icon.png) （在左侧面板中）。

   >[!NOTE]
   >
   >如果您看不到左侧导航面板或其图标，请单击菜单 ![菜单](assets/main-menu-icon-left-nav.png) 图标。

   在灰色中 [!UICONTROL 文件夹] 在显示的面板中，您可以将方案整理到文件夹中。

   在主区域右上方，您可以查看 **[!UICONTROL 全部]** 您构建的方案，您的 **[!UICONTROL 活动方案]**， **[!UICONTROL 非活动方案]**、和 **[!UICONTROL 概念]**. 概念是以前需要做更多工作的场景 [!DNL Workfront Fusion] 可将它们分类为活动或非活动。

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. 在 [!UICONTROL 文件夹] 面板中，单击 **[!UICONTROL 添加文件夹]** 图标 ![](assets/add-folder-icon.png)，然后为第一个文件夹键入一个名称，如“Practice scenarios”。

1. 打开文件夹，然后单击 **[!UICONTROL 创建新方案]** 页面右上角的。

   显示的登陆页面允许您预加载要在要构建的方案中使用的任何应用程序。

1. 在本练习中，搜索并选择 **[!DNL Workfront]** 应用程序。
1. 单击 **[!UICONTROL 继续]** 在右上角。

   随后将显示方案编辑器，其中心包含一个空模块， [!DNL Workfront] ，以及底部工具栏中的一些选项。

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

在本例中，我们未使用触发器模块。 相反，此方案从搜索开始。

1. 单击空模块以选择要从中选择模块的应用程序。

   您之前预加载的应用程序显示在空模块旁边。 您可以使用添加任何具有模块的其他应用程序。 [!UICONTROL 搜索] 盒子。

   ![](assets/pre-loaded-app-wf-350x172.png)

1. 单击 **[!DNL Workfront]**.

   列表更改为全部显示 [!DNL Workfront] 可用作触发器模块的模块。

1. 单击“搜索”模块 **[!UICONTROL 搜索]**.

   现在，您需要建立与贵机构的 [!DNL Workfront] 帐户。 您添加到方案的每个模块都必须连接到其应用程序。

1. 在 **[!DNL Workfront]** 框，下 **[!UICONTROL 连接]**，单击 **[!UICONTROL 添加]**，然后键入连接的名称，如“Olivia的Workfront帐户”，然后单击 **[!UICONTROL 继续]**.
1. 在显示的窗口中验证连接。

   对连接进行身份验证的过程在应用程序之间可能会有所不同。 以下流程特定于 [!DNL Workfront]，但其过程与许多应用程序类似。

   1. 输入您的 [!DNL Workfront] 域，然后单击 **[!UICONTROL 继续]**.
   1. 登录 [!DNL Workfront].
   1. 检查访问权限 [!DNL Workfront Fusion] 请求，然后单击 **[!UICONTROL 允许访问]**.

   如果您需要帮助，请参阅 [关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 配置第一个模块

连接后 [!DNL Workfront Fusion] 敬您的 [!DNL Workfront] 帐户，您可以指定 [!DNL Workfront] 您有权访问的请求队列以及您希望第一个模块处理的数据。

1. 在 [!UICONTROL 记录类型] 框，选择 **[!UICONTROL 项目]**. 这会将模块设置为仅搜索项目。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 项目]** 在列表中(如果您开始键入“[!UICONTROL 项目].”

1. 在 **[!UICONTROL 结果集]** 框，选择 **[!UICONTROL 第一个匹配记录]**. 这会将模块设置为仅返回其发现满足条件的第一个记录。 在本例中，我们只需要返回一条记录。
1. 在 **[!UICONTROL 搜索条件]** 区域，我们将设置过滤器以返回特定项目。

   1. 在下的第一个框中 [!UICONTROL 搜索条件]中，选择要搜索其值的字段。 对于此示例，请选择 **[!UICONTROL 名称]**.
   1. 对于运算符，选择 [!UICONTROL 包含（区分大小写）]. 这允许模块查找名称中包含您选定字词的项目，即使您未输入完整名称或输入大小写不正确（例如全部大写）的名称，也是如此。
   1. 在下的最后一个字段中 [!UICONTROL 搜索条件]，输入您知道位于所搜索项目名称中的单词或短语。

1. 在 **[!UICONTROL 输出]** 列表中，选择要输出问题的字段。 对于此示例，请选择 **[!UICONTROL ID]** 和 **[!UICONTROL 名称]** 字段。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F** ([!DNL Windows] OS)以快速找到字段。

1. 单击 **[!UICONTROL 确定]**.

   >[!NOTE]
   >
   >（仅供参考）由于这不是触发器模块，因此您不会选择从何处启动它。 使用触发器模块时，您现在可以选择从何处启动它。
   >
   >
   >有关更多信息，请参阅 [选择触发器模块的开始位置 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. 右键单击模块，然后单击 **[!UICONTROL 重命名]**，然后键入一个名称，该名称用于描述您希望模块执行的操作（例如“搜索项目”），然后单击 **[!UICONTROL 确定]**.

   该名称显示在模块正下方。 在那个下面， [!DNL Workfront Fusion] 包含模块所执行操作类型的简短描述。

   ![](assets/module-renamed-wf.png)

1. 继续使用 [添加并配置第二个模块](#add-and-configure-the-second-module).

## 添加并配置第二个模块

1. 单击模块右侧的部分圆圈，以 **[!UICONTROL 添加另一个模块]**.
1. 选择 [!DNL Workfront] 从应用程序列表中选择搜索模块 **[!UICONTROL 读取相关记录]**.
1. 您已创建与的连接 [!DNL Workfront] 用于上一个模块。 您无需在此处再次创建它，但必须确保此模块使用与上一个模块相同的连接。\
   在 **[!UICONTROL 连接]** 框中，选择您为上一个模块创建的连接。
1. 单击 **[!UICONTROL 记录类型]**，然后选择 **[!UICONTROL 项目]**，因为我们希望读取与项目相关的记录。

   >[!TIP]
   >
   >您可以找到 **[!UICONTROL 项目]** 在列表中键入“project”时，才会出现这种情况。

1. 单击 **[!UICONTROL 父记录编号]** 字段。 此字段要求您想要从中返回任务的项目的Workfront ID。

   单击字段会打开可在以下位置使用的变量列表： **[!UICONTROL 父记录编号]** 用于标识Workfront中的项目的字段。

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 单击变量 **[!UICONTROL ID]** 以将其添加到 **[!UICONTROL 父记录编号]** 字段。 这允许将从第一个模块返回的ID用作要在第二个模块中处理的项目的标识符，从而确保返回的任务将属于该项目。
1. 在 **[!UICONTROL 收藏集]** 字段，选择 **[!UICONTROL 任务]**. 这表示模块将返回与所选项目关联的任务。
1. 单击 **[!UICONTROL 确定]**

   现在您有一个工作方案。

1. 为第二个模块命名，例如“返回与项目关联的任务”，然后继续 [测试场景](#test-the-scenario).

## 测试场景

在激活场景之前，请务必至少运行一次场景并查看结果以测试场景。 这有助于您了解数据如何在场景中流动并查找任何错误。

我们选择返回1个项目，以及与该项目关联的任务。 如果您运行该方案，则应该出现这种情况。

1. 单击 **[!UICONTROL 运行一次]** （在场景编辑器的左下角）。
1. 方案运行完毕后，单击第一个模块上方的气泡。

   ![](assets/click-bubble.png)

   在显示的框中，可以查看有关模块处理的数据包的信息，包括从模块返回的项目中提取的实际数据。

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 单击第二个模块上方的执行检查器气泡可查看信息输入和输出，它是项目中包含的任务集合。

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   您可以在以下文章中了解有关如何读取场景执行信息的更多信息：

   * 有关一般信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 有关已处理捆绑包的信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** ![](assets/save-icon.png) 左下角附近，保存场景进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

>[!TIP]
>
>我们建议您选择添加有关每个模块的注释这一可选但有用的做法。
>
>1. 右键单击 [!DNL Workfront] 模块，然后单击 **[!UICONTROL 添加注释]**.
>1. 在显示的注释中，键入模块的概述。
>
>    您可以为一个模块添加多个注释。
>
>1. 关闭 **[!UICONTROL 注释]** 区域。
>
>     向方案添加注释后，上会显示一个橙色圆点 **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 位于场景编辑器的底部。
>
>1. 单击 **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 以查看您的注释。
>



## 激活方案

此示例方案没有触发器模块。 如果将此方案用于实际数据，则它将以触发器模块开头，您最后会执行的是激活该模块。 在激活某个方案后，默认情况下，它每15分钟运行一次。 您可以通过定义运行时间和频率来更改此值。

有关激活方案的更多信息，请参阅 [在中激活或取消激活方案 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

有关时间表的信息，请参阅 [在中计划方案 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
