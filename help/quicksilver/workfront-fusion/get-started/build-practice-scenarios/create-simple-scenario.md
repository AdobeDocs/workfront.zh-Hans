---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 在中创建基本方案 [!DNL Adobe Workfront Fusion]
description: 了解如何使用Adobe Workfront Fusion创建简单的自动化场景。 自动化场景可自动执行Workfront流程，包括数据操作和转换。 本示例将引导您完成创建场景的过程，该场景将搜索 [!DNL Workfront] Workfront中的任务并将其转换为项目。
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# 在中创建基本方案 [!DNL Adobe Workfront Fusion]

的作用 [!DNL Adobe Workfront Fusion] 是使您的流程自动化，以使您能够专注于新任务，而不是一次又一次地重复相同的任务。 它的工作方式是，关联应用程序和服务内外的操作，从而创建一个自动传输和转换数据的方案。 您创建的方案会监视应用程序或服务中的数据，并对这些数据进行处理以提供您想要的结果。

本示例将引导您完成创建场景的过程，该场景将搜索 [!DNL Workfront] Workfront中的任务并将其转换为项目。

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
1. 在 [!UICONTROL 记录类型] 框，选择 **[!UICONTROL 任务]**. 这会将模块设置为仅搜索任务。

   您可以找到 **[!UICONTROL 任务]** 在列表中(如果您开始键入“[!UICONTROL 任务]“

1. 在 **[!UICONTROL 结果集]** 框，选择 **[!UICONTROL 第一个匹配记录]**.

   这会将模块设置为仅返回它发现满足条件的第一个记录。
1. 在 **[!UICONTROL 搜索条件]** 区域，配置条件以返回特定任务。

   1. 在下的第一个框中 [!UICONTROL 搜索条件]，选择要包含在搜索中的字段。 对于此示例，请选择 **[!UICONTROL 名称]**.

      您可以找到 **[!UICONTROL 名称]** 在列表中(如果您开始键入“[!UICONTROL name]“
   1. 对于运算符，单击旁边的下拉箭头 **存在** 并将其更改为 [!UICONTROL **包含（区分大小写）**].

      这允许模块查找名称中包含您选定字词的项目，即使您未输入完整名称或输入大小写不正确（例如全部大写）的名称，也是如此。
   1. 在下的最后一个字段中 [!UICONTROL 搜索条件]，输入您知道位于所搜索任务名称中的单词或短语。

1. 在 **[!UICONTROL 输出]** 列表中，选择要模块输出的字段。 对于此示例，请选择 **[!UICONTROL ID]** 和 **[!UICONTROL 名称]** 字段。

   >[!TIP]
   >
   >您可以使用 **Cmd+F** ([!DNL Mac] OS)或 **Ctrl-F** ([!DNL Windows] OS)来快速查找字段。

1. 单击 **[!UICONTROL 确定]** 以保存模块配置。

1. 右键单击模块，然后单击 **[!UICONTROL 重命名]**，然后键入描述您希望模块执行的操作的名称（例如“Search for task”），然后单击 **[!UICONTROL 确定]**.

   该名称显示在模块正下方。 在那个下面， [!DNL Workfront Fusion] 简要说明模块执行的操作类型。

   ![](assets/module-renamed-wf.png)

1. 继续 [添加并配置第二个模块](#add-and-configure-the-second-module).

## 添加并配置第二个模块

1. 将鼠标悬停在模块右侧的部分圆上，然后单击 **[!UICONTROL 添加另一个模块]**.
1. 选择 [!DNL Adobe Workfront] 从应用程序列表中，选择模块 **[!UICONTROL 转换对象]**.
1. 在 [!UICONTROL 连接] 字段中，选择您在上一模块中使用的相同Workfront连接。
1. 在 **[!UICONTROL 记录类型]** 字段，选择 **[!UICONTROL 任务]**，因为模块将转换任务。
1. 在 **[!UICONTROL 转换为]** 字段，选择 **项目**.
1. 在任务ID字段旁边，单击映射切换开关以启用它。

   启用时，切换将变为蓝色。 这允许您映射上一个模块中的任务ID。

   ![映射切换](assets/map-toggle.png)
1. 单击 **[!UICONTROL 任务编号]** 字段。

   此时将打开一个面板，通过该面板可选择要用作要转换为项目的任务ID的内容。 由于您启用了映射，因此该面板会包含之前所有模块的输出。 您选择将ID作为上一个模块的输出，因此现在该面板中提供了该ID。

   此面板称为映射面板。 有关映射面板的详细信息，请参阅 [将信息从一个模块映射到另一个模块](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. 选择 **ID** 在映射面板中。

   ID字段中会显示一个ID块。 它显示了映射自它的模块的编号，以及映射的字段。

   ![映射ID](assets/map-id.png)

1. 单击 **模板Id** 字段中，开始键入要用于此项目的Workfront模板的名称，然后当它出现在列表中时将其选定。
1. 单击 **[!UICONTROL 确定]** 以保存模块配置。

1. 右键单击模块，然后单击 **[!UICONTROL 重命名]**，然后键入一个名称，该名称用于描述您希望模块执行的操作（例如“转换为项目”），然后单击 **[!UICONTROL 确定]**.

1. 继续 [测试场景](#test-the-scenario).

## 测试场景

在激活方案之前，请务必至少运行一次方案并查看结果以对其进行测试。 这有助于您了解数据如何在场景中流动并查找任何错误。

对于这种情况，成功的测试将导致找到新任务并将其转化为项目。

1. 单击 **[!UICONTROL 运行一次]** 位于场景编辑器的左下角。
1. 在场景结束运行后，单击第一个模块上方的气泡可查看有关模块处理的数据包的信息，包括从模块返回的任务中拉取的数据。

1. 单击第二个模块上方的执行检查器气泡，可查看输入（任务）和输出（已转换的项目）。

   有关检查气泡中数据的详细信息，请参阅：

   * 有关一般信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * 有关已处理捆绑包的信息，请参阅 [场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

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

由于此方案正在搜索特定任务，因此无需激活它。 激活场景会导致场景按计划运行，或者在应用程序中发生特定操作时运行。 在激活方案后，默认情况下，它每15分钟运行一次。 您可以通过定义运行的时间和频率来更改此设置。

有关激活方案的详细信息，请参阅 [激活或停用中的方案 [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

有关时间表的信息，请参阅 [在中计划方案 [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## 下面的步骤

* [添加触发器模块](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) 以允许方案定期查找新请求并将它们转换为项目。
* 添加webhook以允许每次输入请求时执行场景。
* 添加过滤器以确保仅将某些请求转换为项目。
* 添加一个函数以自定义新项目的名称。
* 添加错误处理以确保场景可以抵御错误。

