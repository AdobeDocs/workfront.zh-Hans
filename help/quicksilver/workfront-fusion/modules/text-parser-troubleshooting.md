---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: 中的文本解析器故障排除 [!DNL Adobe Workfront Fusion]
description: 如果无法获取文本解析器来生成任何输出，请使用此信息。
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# 中的文本解析器故障排除 [!DNL Adobe Workfront Fusion]

如果无法获取文本解析器来生成任何输出，请使用此信息。

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

## 故障排除

案例场景示例，您希望解析文件文档“filename.docx”的文件类型，并且文件名的扩展名在DOCX、PDF和CSV之间始终不同。

在这种情况下，您可以选择使用的表达式是 [!DNL \..+]

如果您要在regex101.com上的正则表达式上使用它，则将获得完全匹配。

![](assets/regex-expression-350x130.png)

在上图中，文件扩展名正确匹配。 如果您接受此内容并尝试在文本解析器中实施它：

![](assets/text-parser-350x602.png)

您不会获得匹配项：

![](assets/text-parser-you-dont-get-a-match-350x365.png)

原因在于“i”仅显示每个匹配的匹配数，因此在本例中，我们有2个匹配，因此“i”后面有一个数值1和2。 用例是，如果您只需要匹配或传递过滤器中的数据，或者只需要第二个匹配的值，则可以指定由数值表示的值。

![](assets/text-parser-matches-350x355.png)

为了能够获取将括号添加到要分析的部分所需的匹配值（例如，从“filename.docx” — “docx”中提取），然后根据我们用于此案例的正则表达式方案，应将括号应用于\。(.+)

这会捕获DOCX，将其放入一个组中，并保留“。” 别想了。

![](assets/text-parser-get-matches-350x592.png)

在下图所示的输出中，捕获组将匹配任何字符（行终止符除外）。

![](assets/text-parser-output-350x389.png)

另一个同时包含正则表达式的解决方法是使用replace函数

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

然后替换 `abcdefghijklmno pqr stuvw xyz.docx` 以及实际文件名变量。
