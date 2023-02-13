---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: “Adobe Workfront Fusion方案示例：连接电子邮件、文本解析器和Google表'
description: 此方案可帮助您创建所有电子邮件的日志，并标记它们以在电子表格中执行进一步操作。 它会使用正则表达式(Regex)作为搜索模式，在电子表格的两个单独表格中捕获电子邮件正文。 第一模式搜索短语，第二模式搜索相同短语和电子邮件地址。
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 方案示例：连接电子邮件， [!UICONTROL 文本解析器]和 [!DNL Google Sheets]

此方案可帮助您创建所有电子邮件的日志，并标记它们以在电子表格中执行进一步操作。 它会使用正则表达式(Regex)作为搜索模式，在电子表格的两个单独表格中捕获电子邮件正文。 第一模式搜索短语，第二模式搜索相同短语和电子邮件地址。

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

## 先决条件

本教程需要对正则表达式有基本的知识。 要了解Regex，请访问 [https://regexone.com](https://regexone.com/).

添加并配置第一个模块

1. 搜索电子邮件并选择 **[!UICONTROL 观看电子邮件]** 作为触发器。

   >[!NOTE]
   >
   >当您可以 [!DNL Google] 使用E的帐户邮件模块，您还可以使用 [!DNL Gmail] 模块。

1. 连接 [!DNL Google] 帐户或任何其他基于IMAP的电子邮件客户端(例如 [!DNL Outlook])。
1. 连接后，选择要监视其传入电子邮件的文件夹，例如 [!UICONTROL 收件箱].
1. 在 [!UICONTROL 标准]，选择 **[!UICONTROL 所有电子邮件]** （或将其缩小为已读或未读电子邮件）。

   您还可以选择将已获取的电子邮件标记为已读或未读。

1. 设置 [!UICONTROL 最大结果数] 到1。

   ![](assets/save-max-as-1-350x304.png)

   您可以根据收到的消息量更改此设置。 但是，建议设置一个低值并更频繁地运行该方案。

1. 单击 **[!UICONTROL 显示高级设置]** 在底部。

   ![](assets/show-adv-settings-350x332.png)

1. 按 [!UICONTROL 发件人地址], [!UICONTROL 主题] 和 [!UICONTROL 短语].

   这样，您便能够仅观看相关电子邮件。 在本例中，我们仅添加了一个“主题”过滤器，并将其他2个留空。

   >[!NOTE]
   >
   >我们将添加路由器，以使用 [!UICONTROL 匹配模式] 迭代器和正则表达式(Regex)作为搜索模式。 这还使我们能够构建多实用程序方案。

1. 完成配置后，系统会提示您指定从何处开始观看电子邮件，请单击 **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. 继续 [搜索 [!UICONTROL 流量控制] 并添加 [!UICONTROL 路由器]](#search-for-flow-control-and-add-a-router)

## 搜索 [!UICONTROL 流量控制] 并添加 [!UICONTROL 路由器]

1. 在任意模块之后添加路由器，以在将数据发送到下一个模块之前对数据进行拆分或复制。

   在这里，我们用了 [!UICONTROL 路由器] 向 [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## 使用 [!UICONTROL 文本解析器] 模块

1. 添加 [!UICONTROL 匹配模式] 转换器来在电子邮件中搜索短语。

   我们将搜索短语“[!UICONTROL 文本解析器模块]“ ”，以捕获与该短语匹配的正文文本和发件人名称。

   1. 将模式写为正则表达式：

      text\sparser\smodule

   1. （可选）使用任何其他模式选项。

      ![](assets/pattern-350x318.png)

      如果文本包含多行，并且您需要在每行中搜索模式，则多行非常有用。 在本教程中，我们需要在整个电子邮件正文文本中搜索模式，因此我们将将其保留为未选中状态。

   1. 在 [!UICONTROL 文本] 字段，单击属性 **文本内容** 列表中。

      ![](assets/text-content-350x264.png)

      这是用于存储电子邮件正文中的文本的属性，我们将在其中搜索模式。

1. 添加其他 [!UICONTROL 匹配模式] 搜索同一短语和电子邮件地址。

   如果您的客户帐户具有多个用户，则此功能会特别有用。 为了节省时间，您可以克隆 [!UICONTROL 文本解析器] 模块，并将其链接到路由器。

   ![](assets/clone.png)

1. 按如下方式编辑模式：

   text\sparser\smodule.+\s([\w -]+@[\w -]+)

   ![](assets/text-parser-350x202.png)

   此模式搜索短语“[!UICONTROL 文本解析器模块]和john.doe@gmail.com之类的电子邮件地址，并且只返回电子邮件地址。

   >[!NOTE]
   >
   >根据您接受的电子邮件地址的规范编写正则表达式非常重要，但上述规范将处理大多数标准电子邮件地址。

   * 如果您只想搜索电子邮件地址，则可以使用以下正则表达式：

      ([\w -]+@[\w -]+)

   * 您也只能使用下面的正则表达式搜索电话号码：

      ^[+]?\(?(\d{1,3})\?[\s-]?\(?(\d{3})\?[\s-]?\d{3}[\s-]?\d{3,4}上述模式涵盖写入电话号码的最常见格式。
   要测试您的模式，我们建议使用 [[!DNL https://regex101.com]](https://regex101.com/) with [!DNL javascript] 作为风味。

   其余的配置与之前的配置相同。

## 添加 [!DNL Google Sheets] 模块

对于 [!DNL Sheets]，我们需要首先创建一个包含必需标题的电子表格。

1. 创建一个电子表格，其中包含要在其中捕获用户数据的列。 （您也可以使用现有文件）。

   例如，创建一个名为“电子邮件数据：“支持票证”中的“发件人名称”、“发件人电子邮件”和“电子邮件内容”列。 将工作表命名为“contains:文本解析器模块。”

1. 添加 [!UICONTROL Google工作表] 模块 **[!UICONTROL 添加行]** 作为操作。

   ![](assets/add-a-row-350x174.png)

1. 连接 [!DNL Google] 帐户（如果尚未启用）。 选择之前创建的文件，然后选择要在其中捕获数据的工作表。

   您的设置应如下所示：

   ![](assets/connect-google-acct-350x279.png)

1. 映射相关字段（列）中的属性以完成模块设置。

   ![](assets/map-attributes-350x282.png)

1. 克隆刚刚创建的模块，并将其链接到第二个模块 [!UICONTROL 文本解析器] 模块。

   1. 转到您的电子表格，复制之前创建的工作表并为其命名。

      例如，将其命名为“contains:文本解析器模块和电子邮件。”

   1. 添加另一列以存储电子邮件正文包含的电子邮件地址。

      例如，将其命名为“Email Address Shared”。

   1. 单击克隆的 [!DNL Google Sheets] 模块来配置设置。
   1. 将工作表更改为您刚刚创建的新工作表。
   1. 映射 [!UICONTROL 匹配模式] 模块($1)到要存储电子邮件地址（共享电子邮件地址）的列。

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. 单击 **[!UICONTROL 确定]**，保存方案，然后将其运行测试。

      您需要向连接的电子邮件地址发送两封单独的电子邮件，如下所示：

      * 包含短语“[!UICONTROL 文本解析器模块]“（无电子邮件地址）

         ![](assets/text-parser-module-350x103.png)

      * 包含上述短语和电子邮件地址

         ![](assets/above-phrase-and-email-350x106.png)

         如果您的设置中没有错误，您将看到第一个工作表会捕获包含短语“[!UICONTROL 文本解析器模块]“ ”，而第二个工作表仅捕获包含短语“ ”的工作表[!UICONTROL 文本解析器模块]和电子邮件地址。 您可以参阅下面的屏幕截图。

         工作表1:

         ![](assets/worksheet-1-350x57.png)

         工作表2:

         ![](assets/worksheet-2-350x41.png)

## 资源

* [免费练习](https://regexone.com/) 了解正则表达式
* [了解电话号码匹配](https://regexone.com/problem/matching_phone_numbers) 使用Regex
* [了解电子邮件匹配](https://regexone.com/problem/matching_emails) 使用Regex
* [测试正则表达式](https://regex101.com/)
