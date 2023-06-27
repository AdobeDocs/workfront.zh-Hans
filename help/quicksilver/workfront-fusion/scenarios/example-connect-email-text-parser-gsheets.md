---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Adobe Workfront Fusion场景示例：连接电子邮件、文本解析器和Google工作表'
description: 此方案可帮助您创建包含所有电子邮件的日志，并标记它们以便在电子表格中执行进一步操作。 它使用正则表达式(Regex)作为搜索模式，在电子表格中的两个单独表中捕获电子邮件正文。 第一模式搜索短语，而第二模式搜索相同的短语和电子邮件地址。
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1214'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] 场景示例：连接电子邮件， [!UICONTROL 文本解析器]、和 [!DNL Google Sheets]

此方案可帮助您创建包含所有电子邮件的日志，并标记它们以便在电子表格中执行进一步操作。 它使用正则表达式(Regex)作为搜索模式，在电子表格中的两个单独表中捕获电子邮件正文。 第一模式搜索短语，而第二模式搜索相同的短语和电子邮件地址。

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

## 先决条件

本教程需要具备正则表达式的基本知识。 要了解正则表达式，请访问 [https://regexone.com](https://regexone.com/).

添加第一个模块并进行配置

1. 搜索电子邮件并选择 **[!UICONTROL 观看电子邮件]** 作为触发器。

   >[!NOTE]
   >
   >虽然您可以连接 [!DNL Google] 使用E的帐户邮件模块，您也可以使用 [!DNL Gmail] 模块。

1. 连接 [!DNL Google] 帐户或其他任何基于IMAP的电子邮件客户端(例如 [!DNL Outlook])。
1. 连接后，选择要监视其传入电子邮件的文件夹，例如 [!UICONTROL 收件箱].
1. 下 [!UICONTROL 标准]，选择 **[!UICONTROL 所有电子邮件]** （或者将其缩小到读取或未读取的电子邮件）。

   您还可以选择将获取的电子邮件标记为已读或未读。

1. 设置 [!UICONTROL 最大结果数] 到1。

   ![](assets/save-max-as-1-350x304.png)

   您可以根据收到的消息量更改此值。 但是，建议设置一个低值并更频繁地运行该方案。

1. 单击 **[!UICONTROL 显示高级设置]** 在底部。

   ![](assets/show-adv-settings-350x332.png)

1. 按筛选电子邮件 [!UICONTROL 发件人地址]， [!UICONTROL 主题] 和 [!UICONTROL 短语].

   这样，您就可以只查看相关电子邮件。 在本例中，我们仅添加了一个“主题”过滤器，并将另外2个留空。

   >[!NOTE]
   >
   >我们将添加路由器，以使用在电子邮件中查找短语 [!UICONTROL 匹配模式] 迭代器和正则表达式（正则表达式）作为搜索模式。 这还使我们能够构建一个多用途方案。

1. 配置完成后，系统会提示您指定从何处开始观看电子邮件，请单击 **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. 继续访问 [搜索 [!UICONTROL 流量控制] 并添加 [!UICONTROL 路由器]](#search-for-flow-control-and-add-a-router)

## 搜索 [!UICONTROL 流量控制] 并添加 [!UICONTROL 路由器]

1. 在任何模块之后添加路由器，以拆分或复制数据，然后再将其发送到下一个模块。

   这里，我们用了 [!UICONTROL 路由器] 将电子邮件正文文本发送到 [!DNL Google Sheet].

   ![](assets/search-for-flow-control-350x220.png)

## 使用 [!UICONTROL 文本解析器] 模块

1. 添加 [!UICONTROL 匹配模式] 转换程序以搜索电子邮件中的短语。

   我们将搜索短语“[!UICONTROL 文本解析器模块]”在所有传入电子邮件中捕获，以捕获匹配该短语的正文和发件人姓名。

   1. 将模式写入为正则表达式：

      文本\稀疏器\模块

   1. （可选）使用任何其他模式选项。

      ![](assets/pattern-350x318.png)

      如果文本包含多行，并且需要搜索每行中的模式，则多行很有用。 在本教程中，我们需要在整个电子邮件正文文本中搜索模式，因此我们将取消选中该模式。

   1. 在 [!UICONTROL 文本] 字段中，单击属性 **文本内容** 在列表中。

      ![](assets/text-content-350x264.png)

      这是用于存储电子邮件正文文本的属性，我们将在其中搜索模式。

1. 添加另一个 [!UICONTROL 匹配模式] 会搜索相同的短语和电子邮件地址。

   如果您的客户帐户具有多个用户，则此功能特别有用。 要节省时间，您可以克隆 [!UICONTROL 文本解析器] 您刚刚创建的模块并将其链接到路由器。

   ![](assets/clone.png)

1. 按如下方式编辑模式：

   text\sparser\smodule。+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   此模式搜索短语“ ”[!UICONTROL 文本解析器模块]”和john.doe@gmail.com等电子邮件地址，并且只返回电子邮件地址。

   >[!NOTE]
   >
   >根据您接受的电子邮件地址规范编写正则表达式很重要，但上述规范会处理大多数标准电子邮件地址。

   * 如果您只想搜索电子邮件地址，可以使用下面的正则表达式：

     ([\w.-]+@[\w.-]+)

   * 您还可以使用以下正则表达式仅搜索电话号码：

     ^[+]？\(？(\d{1，3})\)？[\s-]？\(？(\d{3})\)？[\s-]？\d{3}[\s-]？\d{3，4}
上述模式涵盖了写入电话号码的最常见格式。

   要测试您的模式，我们建议使用 [[!DNL https://regex101.com]](https://regex101.com/) 替换为 [!DNL javascript] 作为“风味”。

   其余配置与之前的配置相同。

## 添加 [!DNL Google Sheets] 模块

对象 [!DNL Sheets]，我们需要首先创建一个具有所需标头的电子表格。

1. 创建一个电子表格，其中包含您要在其下捕获用户数据的列。 （您也可以使用现有文件）。

   例如，创建一个名为“Email Data： Support Ticket”的文件，将“发件人姓名”、“发件人电子邮件”和“电子邮件内容”列为列。 将工作表命名为“包含：文本解析器模块”。

1. 添加 [!UICONTROL Google工作表] 模块 **[!UICONTROL 添加行]** 作为操作。

   ![](assets/add-a-row-350x174.png)

1. 连接您的 [!DNL Google] 帐户（如果尚未提供）。 选择您之前创建的文件，然后选择要在其中捕获数据的工作表。

   您的设置应如下所示：

   ![](assets/connect-google-acct-350x279.png)

1. 映射相关字段（列）中的属性以完成模块设置。

   ![](assets/map-attributes-350x282.png)

1. 克隆您刚刚创建的模块，并将其链接到第二个模块 [!UICONTROL 文本解析器] 模块。

   1. 转到电子表格，复制之前创建的工作表并为其命名。

      例如，将其命名为“contains： text parser module and email”。

   1. 添加另一列以存储电子邮件正文包含的电子邮件地址。

      例如，将其命名为“Email Address Shared”。

   1. 单击克隆的 [!DNL Google Sheets] 模块以配置设置。
   1. 将工作表更改为您刚刚创建的新工作表。
   1. 映射输出 [!UICONTROL 匹配模式] 模块($1)添加到要存储电子邮件地址（已共享电子邮件地址）的列。

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. 单击 **[!UICONTROL 确定]**，保存场景，并将其用于测试运行。

      您将需要向连接的电子邮件地址发送两封单独的电子邮件，如下所示：

      * 包含短语&quot;[!UICONTROL 文本解析器模块]“”（没有电子邮件地址）

        ![](assets/text-parser-module-350x103.png)

      * 包含上述短语和电子邮件地址

        ![](assets/above-phrase-and-email-350x106.png)

        如果您的设置中没有错误，您将看到第一个工作表捕获包含短语“ ”的所有电子邮件[!UICONTROL 文本解析器模块]“而第二个工作表则仅捕获包含短语”的单词[!UICONTROL 文本解析器模块]”和电子邮件地址。 您可以参阅下面的屏幕截图。

        工作表1：

        ![](assets/worksheet-1-350x57.png)

        工作表2：

        ![](assets/worksheet-2-350x41.png)

## 资源

* [免费练习](https://regexone.com/) 了解正则表达式
* [了解电话号码匹配](https://regexone.com/problem/matching_phone_numbers) 使用Regex
* [了解电子邮件匹配](https://regexone.com/problem/matching_emails) 使用Regex
* [测试正则表达式](https://regex101.com/)
