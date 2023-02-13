---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 文本解析器疑难解答 [!DNL Adobe Workfront Fusion]
description: 如果无法获取文本解析器以生成任何输出，请使用此信息。
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# 文本解析器疑难解答 [!DNL Adobe Workfront Fusion]

如果无法获取文本解析器以生成任何输出，请使用此信息。

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

## 疑难解答

示例情景示例，您要解析文件文档“filename.docx”的文件类型，文件名的扩展名始终从DOCX到PDF到CSV。

在本例中，您可以选择使用的表达式是 [!DNL \..+]

如果要在regex101.com上的正则表达式中使用此函数，将获得完全匹配。

![](assets/regex-expression-350x130.png)

在上图上，文件扩展名已正确匹配。 如果您采用此方法并尝试在文本解析器中实施它：

![](assets/text-parser-350x602.png)

您将不会获得匹配项：

![](assets/text-parser-you-dont-get-a-match-350x365.png)

原因是“i”仅显示每次匹配的匹配数，因此在此例中，我们有2个匹配，因此在“i”之后有一个数值1和2。 其用例是，如果您曾经需要仅通过第二个匹配的值来匹配或传递数据，则可以指定由数值表示的值。

![](assets/text-parser-matches-350x355.png)

为了能够获取在要解析的部分中添加括号所需的匹配值（例如，从“filename.docx” — “docx”中提取），然后，根据我们在本例中使用的正则表达式表达式，应在\上应用括号。(.+)

这会捕获DOCX，将其放入组中，并保留“。” 从中解脱出来。

![](assets/text-parser-get-matches-350x592.png)

在下图所示的输出中，捕获组将匹配任何字符（除行终结器外）。

![](assets/text-parser-output-350x389.png)

还包含正则表达式的另一个解决方法是使用replace函数

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

然后，替换 `abcdefghijklmno pqr stuvw xyz.docx` 的值。
