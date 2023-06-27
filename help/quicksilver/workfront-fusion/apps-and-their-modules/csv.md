---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: 通过Adobe Workfront Fusion CSV模块，您可以创建CSV文件，并根据收到的文本值或文件解析CSV文本。
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 1%

---

# CSV

此 [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] 通过模块，您可以创建CSV文件，并根据收到的文本值或文件解析CSV文本。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[！UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] （对于工作自动化和集成），[！UICONTROL [!DNL Workfront Fusion] 工作自动化]</p>
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

## [!UICONTROL 创建CSV]

此 [!UICONTROL 创建CSV] 使用聚合器，可根据收到的文本值创建csv文本。

有关聚合器的更多信息，请参阅 [中的聚合器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL源模块]</td>
        <td>选择用于聚合所需字段的模块。</td>
    </tr>
    <tr>
        <td>[！UICONTROL聚合字段]</td>
        <td>从可用字段列表中选择要聚合的字段。</td>
    </tr>
    <tr>
        <td>[！UICONTROL Include headers in the first row]</td>
        <td>选择此选项可在结果中包含标头。</td>
    </tr>
    <tr>
        <td>[！UICONTROL分组依据]</td>
        <td>输入筛选条件以将结果分组。 例如，输入日期。</td>
    </tr>
    <tr>
        <td>[！UICONTROL停止处理空聚合]</td>
        <td>选择此选项可在没有结果时停止方案。</td>
    </tr>
</table>

## [!UICONTROL 创建CSV（高级）]

此 [!UICONTROL 创建CSV（高级）] 使用聚合器，可根据收到的文本值创建CSV文本。 它采用的数据结构定义生成的CSV文件中的CSV列。 定义后，列将作为字段显示在CSV模块设置中，并可映射到场景中的后续模块。

有关聚合器的更多信息，请参阅 [中的聚合器模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL源模块]</td> 
   <td>选择用于聚合所需字段的应用程序模块。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL数据结构]</td> 
   <td> <p>选择数据结构以按您需要的方式聚合字段。 定义数据结构后，您可以将项映射到相应的字段。</p> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">中的数据结构 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Include headers in the first row] </td> 
   <td>选择此选项可在结果中包含标头。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL分组依据] </td> 
   <td>输入筛选条件以将结果分组。 例如，输入日期。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL停止处理空聚合] </td> 
   <td>选择此选项可在没有结果时停止方案。 </td> 
  </tr> 
 </tbody> 
</table>


<p>假设您想要将Google联系人导出到一个CSV文件，其中包含“全名”和“电子邮件”两列。 [！UICONTROL Google Contacts] &gt;[！UICONTROL Get contacts from a group]模块的输出包具有以下结构。 电子邮件地址存储在 <code>[!UICONTROL Emails[]]</code> item，它是一个收藏集数组，每个收藏集包含两个项目： <code>Label</code> 和 <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>如果您使用 [!DNL Create CSV] 模块中，将提供一个与捆绑包的顶级项目对应的复选框列表。 如果您尝试勾选 <code>Full name</code> 和 <code>Emails</code> 项，[！UICONTROL创建CSV]模块会生成以下输出，这可能不是您想要的：</p>
<p>"emails"，"fullName"</p>
<p>“[对象对象]”，“Shon Winer”</p>
<p>“[对象对象]”，“Lizeth Fulmore”</p>
<p>“[对象]”，“Hilario Gullatt”</p>
<p>“[对象对象]”，“Abby Eisenbarth”</p>
<p>自项目开始 <code>Full Name</code> 为简单类型“文本”，导出时不会有问题。 但是这个项目 <code>Emails</code>（属于复杂类型的集合数组）将导出为[object对象]，默认情况下，这是将集合和数组转换为文本的方式。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion中的项目数据类型</a>.</p>
<p>要导出 <code>Email </code>第一个集合的项目 <code>Emails[]</code> 相反，有必要使用[！UICONTROL创建CSV （高级）]模块。 利用模块，可定义CSV文件的各个列，并将项目映射到这些列，包括嵌套列。</p>
<ol>
<li value="1">在场景中插入模块[！UICONTROL创建CSV （高级）]并打开其配置。</li>
<li value="2">单击 <strong>[！UICONTROL添加]</strong> 按钮，用于创建新的数据结构。</li>
<li value="3"> <p>为数据结构写一个名称，然后单击 <strong>[！UICONTROL添加项]</strong> 按钮以添加单个列。 如果要导出两列：“全名”和“电子邮件”，则生成的数据结构将如下所示：</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>成功定义数据结构后，每个单独列对应的字段应会显示在[！UICONTROL创建CSV（高级）]模块的配置中，以便您映射这些项目。 从以下位置获取第一个项目： <code>[!UICONTROL Emails[]]</code> 数组并映射其项 <code>Email </code>至字段/列电子邮件：</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>执行方案。 自项目开始 <code>Emails[1]: Email</code> 映射到列“Email”的简单类型文本，它现在可以正确导出：</p> <p>"Full Name"，"Email"</p> <p>“Shon Winer”，“Shon@Winer.com”</p> <p>“Lizeth Fulmore”，“Lizeth@Fulmore.com”</p> <p>“Hilario Gullatt”，“Hilario@Gullatt.com”</p> <p>“Abby Eisenbarth”，“Abby@Eisenbarth.com”</p> </li>
</ol>
</div>

## [!UICONTROL 解析CSV]

此 [!UICONTROL 解析CSV] 转换器允许您从收到的文本值或文件解析CSV文本。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL列数]</td> 
   <td>指定CSV文件中的列数。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL CSV包含标头]</td> 
   <td> <p>如果CSV文本的第一行包含标题，请选择此选项。</p> <p>注意：模块不使用这些标头来标记输出中的列。 相反，此字段可确保标头不会包含在输出数据中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL delimiterType]</td> 
   <td> <p>选择CSV文件的分隔符。 分隔符是指示分隔值或字段之间的边界的文本字符。</p> 
    <ul> 
     <li>[！UICONTROL逗号]</li> 
     <li>[！UICONTROL选项卡]</li> 
     <li> <p>[！UICONTROL其他]</p> <p>如果选择[！UICONTROL其他]，请输入CSV文件用来分隔值的分隔符字符。 必须只输入一个字符。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL在非引号字段中保留引号]</td> 
   <td>启用此选项可保留引号。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL CSV]</td> 
   <td>输入或映射要解析的CSV文件。<p>注释: <p>如果数据以二进制形式提供（通常来自文件），则必须使用“toString()”函数将二进制数据转换为[！UICONTROL String]：</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
