---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在中创建简单方案 [!DNL Adobe Workfront Fusion]
description: 了解如何使用Adobe Workfront Fusion创建简单的自动化场景。 自动化场景可自动执行Workfront流程，包括数据操作和转换。 本示例将引导您完成创建场景的过程，该场景会搜索问题，然后将其转换为项目。
author: Becky
hide: true
hidefromtoc: true
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 0%

---

# 在中创建基本方案 [!DNL Adobe Workfront Fusion]

的作用 [!DNL Adobe Workfront Fusion] 是使您的流程自动化，以使您能够专注于新任务，而不是一次又一次地重复相同的任务。 它的工作方式是，关联应用程序和服务内外的操作，从而创建一个自动传输和转换数据的方案。 您创建的方案会监视应用程序或服务中的数据，并对这些数据进行处理以提供您想要的结果。

此示例引导您完成以下过程：创建场景以在Workfront中搜索问题并将其转换为项目。

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## 创建实践场景

### 开始创建方案

1. 在 **方案** 区域，单击 **创建新方案**.

   <!--To locate the Scenarios area, see navigation article-->

   此时将显示方案编辑器，其中心包含一个空模块。

   <!--picture?-->

1. 选择 **[!UICONTROL 新方案]** 左上角的占位符名称，然后输入名称。
1. 继续 [添加并配置第一个模块](#add-and-configure-the-first-module) 下。

### 添加并配置第一个模块

1. 单击空模块以选择要从中选择模块的应用程序。

   应用程序列表将显示在模块的右侧。

1. 选择 **[!DNL Adobe Workfront]**。如果不可见，请单击列表底部的搜索栏，键入“Workfront”，然后在此列表出现时将其选定。

   列表将更改为全部显示 [!DNL Workfront] 您可以使用的模块。

1. 单击 **[!UICONTROL Search]** 模块。

   此时将打开模块配置窗口。

1. 在 [!UICONTROL 连接] 框中，选择您的Workfront连接。

   如果您没有Workfront连接，请参阅 [创建与的连接 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. 在 [!UICONTROL 记录类型] 框，选择 **[!UICONTROL 问题]**. 这会将模块设置为仅搜索问题。

   您可以找到 **[!UICONTROL 问题]** 在列表中(如果您开始键入“[!UICONTROL 问题]“

1. 在 **[!UICONTROL 结果集]** 框，选择 **[!UICONTROL 第一个匹配记录]**.

   这会将模块设置为仅返回它发现满足条件的第一个记录。
1. 在 **[!UICONTROL 搜索条件]** 区域，配置标准以返回特定问题。

   1. 在下的第一个框中 [!UICONTROL 搜索条件]，选择要包含在搜索中的字段。 对于此示例，请选择 **[!UICONTROL 名称]**.

      您可以找到 **[!UICONTROL 名称]** 在列表中(如果您开始键入“[!UICONTROL name]“
   1. 对于运算符，单击旁边的下拉箭头 **存在** 并将其更改为 [!UICONTROL **包含（区分大小写）**].

      这允许模块查找名称中包含您选定字词的项目，即使您未输入完整名称或输入大小写不正确（例如全部大写）的名称，也是如此。
   1. 在下的最后一个字段中 [!UICONTROL 搜索条件]，输入您知道位于正在搜索的问题名称中的单词或短语。

1. 在 **[!UICONTROL 输出]** 列表中，选择要模块输出的字段。 对于此示例，请选择 **[!UICONTROL ID]** 和 **[!UICONTROL 名称]** 字段。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F** ([!DNL Windows] OS)来快速查找字段。

1. 单击 **[!UICONTROL 确定]** 以保存模块配置。

1. 右键单击模块，然后单击 **[!UICONTROL 重命名]**，然后键入描述您希望模块执行的操作的名称（例如“Search for issue”），然后单击 **[!UICONTROL 确定]**.

   该名称显示在模块正下方。 在那个下面， [!DNL Workfront Fusion] 简要说明模块执行的操作类型。

   ![](assets/)

1. 继续 [添加并配置第二个模块](#add-and-configure-the-second-module).

## 添加并配置第二个模块

1. 将鼠标悬停在模块右侧的部分圆上，然后单击 **[!UICONTROL 添加另一个模块]**.
1. 选择 [!DNL Adobe Workfront] 从应用程序列表中，选择模块 **[!UICONTROL 其他操作]**.

   “杂项操作”模块允许您在Workfront中执行没有专用模块的操作。 在此示例中，此模块用于将问题转化为项目。
1. 在 [!UICONTROL 连接] 字段中，选择您在上一模块中使用的相同Workfront连接。
1. 在**中[!UICONTROL 记录类型]**字段，选择 **[!UICONTROL 问题]**，因为要执行的操作与问题相关。
1. 在 **[!UICONTROL 操作]** 字段，选择 **convertToProject**. 这是将选定问题转化为项目的操作。
1. 单击 **[!UICONTROL ID]** 字段。

   此时将打开一个面板，通过该面板可选择要用作要转换为项目的问题ID的内容。 该面板包括任何先前模块的输出。 由于您选择ID作为上一模块的输出，因此该面板中现在提供了该ID。

   此面板称为映射面板。 有关映射面板的详细信息，请参阅 [将信息从一个模块映射到另一个模块](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. 选择 **ID** 在映射面板中。

   ID字段中会显示一个ID块。 它显示了映射自它的模块的编号，以及映射的字段。

   ![映射ID](assets/map-id.png)

1. （可选）在项目部分中，找到所有者ID字段，并在该字段中开始键入您的姓名，然后在此字段出现时将其选定。 这会将您设置为项目的所有者，并使该项目更易于在Workfront中找到。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F** ([!DNL Windows] OS)来快速查找字段。

1. 单击 **[!UICONTROL 确定]** 以保存模块配置。

1. 右键单击模块，然后单击 **[!UICONTROL 重命名]**，然后键入一个名称，该名称用于描述您希望模块执行的操作（例如“转换为项目”），然后单击 **[!UICONTROL 确定]**.

1. 继续 [测试场景](#test-the-scenario).

## 测试场景

在激活方案之前，请务必至少运行一次方案并查看结果以对其进行测试。 这有助于您了解数据如何在场景中流动并查找任何错误。

对于这种情况，成功的测试将导致找到问题并将其转化为项目。

1. 单击 **[!UICONTROL 运行一次]** 位于场景编辑器的左下角。
1. 在场景结束运行后，单击第一个模块上方的气泡可查看有关模块处理的数据包的信息，包括从模块返回的问题中拉取的数据。

1. 单击第二个模块上方的执行检查器气泡，可查看输入（问题）和输出（已转换的项目）。

   有关检查气泡中数据的详细信息，请参阅：

   * 有关一般信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 有关已处理捆绑包的信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. 在 [!DNL Workfront Fusion]，单击 **[!UICONTROL 保存]** 左下角附近，保存场景的进度。

   >[!IMPORTANT]
   >
   >在磨练和测试场景时经常保存。

>[!TIP]
>
>我们建议您选择添加有关每个模块的注释这一有用但可选的实践。
>
>1. 右键单击 [!DNL Workfront] 模块，然后单击 **[!UICONTROL 添加注释]**.
>1. 在显示的注释中，键入模块的概述。
>
>    您可以为一个模块添加多个注释。
>
>1. 关闭 **[!UICONTROL 注释]** 区域。
>
>     向方案添加注释后， **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 位于方案编辑器的底部。
>
>1. 单击 **[!UICONTROL 注释]** 图标 ![](assets/notes-icon-w-dot.png) 查看您的备注。
>

## 激活方案

创建场景的最后一步是激活它。

由于此方案正在搜索特定问题，因此无需激活它。 激活场景会导致场景按计划运行，或者在应用程序中发生特定操作时运行。 在激活方案后，默认情况下，它每15分钟运行一次。 您可以通过定义运行的时间和频率来更改此设置。

有关激活方案的详细信息，请参阅 [激活或停用中的方案 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

有关时间表的信息，请参阅 [在中计划方案 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
