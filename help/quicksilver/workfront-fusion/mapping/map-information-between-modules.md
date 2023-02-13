---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: 在 [!DNL Adobe Workfront Fusion]
description: 映射是将模块的输出（结构化为项目）分配给另一个模块的输入字段的过程。
author: Becky
feature: Workfront Fusion
exl-id: e8d619e9-6425-4136-ac71-47d979d68a2d
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# 在 [!DNL Adobe Workfront Fusion]

映射是将模块的输出（结构化为项目）分配给另一个模块的输入字段的过程。

当您单击要在其中插入方案中前一个模块输出的值的字段时，将显示映射面板。 在模块内可用于映射的任意字段中，您可以使用映射面板中的函数和映射项目的任意组合来创建公式，其中包含您键入的静态文本。 这些元素可以相互嵌套。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 包和项目

模块的操作会生成零、一个或多个包作为其输出。 包由一个或多个项目组成。

要探索模块的输出，请执行以下操作：

1. 单击 **[!UICONTROL 运行一次]** 执行模块。
1. 单击模块上方的气泡。

   此时会显示包含模块所有阶段的日志。 您可以在 **[!UICONTROL 输出]** 标题。 每个包都包含其项目和每个项目的值。

>[!INFO]
>
>**示例：** 此示例显示了模块 [!UICONTROL 电子邮件] > [!UICONTROL 观看电子邮件]. 您可以看到，它执行了1个操作，生成包含各种项目(如 `Date`, `Email ID (UID)`, `size`，等等。
>
>![](assets/watch-emails-350x298.png)

>[!NOTE]
>
>封装在 [!UICONTROL 迭代器] 和 [!UICONTROL 聚合器] 在 [!UICONTROL 聚合器] 模块。

## 映射项目

在通过链接两个或多个模块来创建一系列模块后，每个模块都可以处理其前面的模块输出的项目值。

要将项目分配给模块的输入字段，请执行以下操作：

1. 单击应处理上一个模块或模块输出的模块。
1. 在显示的“模块设置”面板中，单击要在其中使用从前一个模块输出的项目值的字段。

   将打开映射面板。

1. 单击映射面板中的某个项目以将其插入到字段中。
1. （可选）要在映射面板中搜索特定字段，请单击映射面板搜索栏，然后键入要搜索的术语。 当字段显示在列表中时，单击该字段。

   搜索结果包含搜索词，不区分大小写。

有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

## 公式

您可以将多个项目映射到一个字段，将它们与文本（固定值）组合，然后使用运算符和函数来构建复杂的公式：

![](assets/operators-and-functions-350x187.png)

您可以在映射面板的其中一个选项卡下方找到函数和运算符。

![](assets/functions-toolbar-350x189.png)

第一个选项卡 ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （在打开面板时显示）显示可从其他模块映射的项目。

其他选项卡包含以下类型的函数：

* **一般函数** ![](assets/toolbar-icon-general-function.png)  — 请参阅 [中的常规函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) 以了解更多信息。

* **数学函数** ![](assets/toolbar-icon-math-functions.png)  — 请参阅 [中的数学函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) 以了解更多信息。

* **文本和二进制函数** ![](assets/toolbar-icon-text&binary-functions.png)  — 请参阅 [中的字符串函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) 以了解更多信息。

* **日期和时间** ![](assets/toolbar-icon-date&time-functions.png)  — 请参阅 [中的日期和时间函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 和以下文章以了解更多信息。

   * [中用于日期和时间格式的令牌 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [用于Adobe Workfront Fusion中日期和时间解析的令牌](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **使用数组的函数** ![](assets/toolbar-icon-functions-for-arrays.png)  — 请参阅 [中的数组函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) 以了解更多信息。

>[!TIP]
>
>创建要在另一个字段中重复使用的复杂公式时，可以单击包含该组合的字段，使用Command-A或Ctrl-A选择该公式，然后将其复制并粘贴到另一个字段中。

有关使用函数映射项目的更多信息，请参阅 [使用 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/map-using-functions.md).

## 收藏集

某些项目可以包含多种类型的值。 这些是集合类型项目。

您可以识别 [!UICONTROL 收藏集] 按项目标签右侧显示的小黑色矩形键入项目，并自动展开子项目列表：

![](assets/collection.png)

>[!NOTE]
>
>在大多数情况下，您会映射集合的子项目，而不是表示整个集合的项目。

有关收藏集的更多信息，请参阅 [中的项目数据类型 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

## 阵列

某些项目可以包含同一类型的多个元素。 这些是数组类型项。

您可以通过项目标签末尾的方括号来标识数组类型项目。 单击项目标签右侧的黑色小矩形以显示元素的项目：

![](assets/array.png)

有关阵列的更多信息，请参阅 [中的项目数据类型 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md)

### 映射数组的第一个元素

如果映射数组的 `Recipient name` 项目时，它会在字段中显示如下：

![](assets/map-array-1st-element.png)

方括号中的数字是一个索引，用于确定将使用数组的哪个元素。 默认情况下，该值设置为1。

### 映射数组的第n个元素

如果要访问其他元素，请单击方括号并编辑索引值：

![](assets/access-another-element.png)

### 使用给定键映射数组的元素

某些数组包含多个包含键项和值项的集合。 这些通常是各种元数据、属性等。

以下示例显示了 [!DNL Jira] 应用程序。

![](assets/output-of-jira-app-350x100.png)

在此示例中，我们从特定附件的附件数组中获取一个文件名，其ID为10108。

输出自 [!DNL Jira] 如下所示：

![](assets/output-from-jira-350x261.png)

典型的要求是根据其给定的键值查找元素，并从值项中获取相应的值。 这可以通过使用 `map()` 和 `get()` 函数。

以下是公式的详细划分：

1. 的第一个参数 `map()` 函数是整个数组项。
1. 第二个参数是值项的原始名称。 要获取原始名称，请将鼠标悬停在 [!UICONTROL 映射] 面板：

   ![](assets/obtain-raw-name-350x124.png)

   >[!NOTE]
   >
   >所有参数都区分大小写。 即使在此特定示例中，项目的标签与其原始名称仅在大小写中不同，仍必须使用原始名称，与标签Value相比，原始名称全部为小写值。

1. 第三个参数是关键项的原始名称：

   ![](assets/3rd-parameter-350x166.png)

1. 第4个参数是给定的键值。

因为 `map()` 函数会返回一个数组（因为具有给定键值的元素可能会更多），因此需要应用 `get()` 函数来获取其第一个元素：

* 的第1个参数 `get()` 函数是 `map()` 函数。

* 第2个参数是元素的索引 — 1。

有关 `map()` 函数，请参阅 [中的数组函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

有关 `get()` 函数，请参阅 [中的常规函数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

## 将元素转换为一系列包

使用 [!UICONTROL 迭代器] 模块。 有关更多信息，请参阅 [[!UICONTROL 迭代器] 模块 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles-350x169.png)

## 疑难解答

### 映射面板中缺少项

对于每个模块，映射面板会显示由模块作者列出的所有输出项。 在某些情况下，此列表可能因各种原因而不完整，并且可能缺少某些项目。 [!DNL Workfront Fusion] 在方案编辑器中运行模块时，可以自动发现缺少的输出项。 具体过程会因模块的类型而略有不同：

#### 即时触发器

1. 右键单击模块，然后单击 **[!UICONTROL 仅运行此模块]** 中。

   如果没有排队的Webhook，则模块会等待新的Webhook进行处理。

1. 生成网页挂钩。

   例如，Webhook模块 **[!DNL Slack]>[!UICONTROL 侦听新事件]** （用于监视渠道中的新渠道消息）向渠道发送消息。

1. 当模块完成运行时，单击模块上方的气泡以浏览其完整输出。

   映射面板将包含在模块输出中发现的所有项目。

#### 轮询触发器

1. 右键单击模块，然后单击 **[!UICONTROL 仅运行此模块]** 中。
1. 如果没有输出，请单击 **[!UICONTROL 选择开始位置]** 并调整设置。
1. 如果没有要处理的事件，请创建一个事件，然后返回到步骤2。

   例如，Webhook模块 **[!UICONTROL Gmail] >[!UICONTROL 观看电子邮件]** 向模块正在监视的文件夹发送电子邮件。

1. 当模块完成运行时，单击模块上方的气泡以浏览其完整输出。

   映射面板现在包含在模块输出中发现的所有项目。

#### 其他模块

您可以选择执行：

* 整个方案（或仅包含模块的部分）

   如果您的方案以触发器开头，请参阅 [即时触发器](#instant-trigger) 或 [轮询触发器](#polling-trigger) 部分。

* 仅单个模块

如果您选择仅执行单个模块：

1. 右键单击模块，然后单击 **[!UICONTROL 仅运行此模块]** 在显示的菜单中……
1. 为输入项提供示例值，然后单击 **[!UICONTROL 确定]** .
1. 当模块完成运行时，单击模块上方的气泡以浏览其完整输出。

   映射面板现在包含在模块输出中发现的所有项目。
