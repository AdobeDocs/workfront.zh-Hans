---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: 利用XML应用程序，可通过XML &gt；解析XML模块解析XML格式文本，并将其转换为捆绑包，以便其他模块可以使用该数据。 您还可以通过XML &gt；创建XML模块将包转换为XML格式文本
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1453'
ht-degree: 2%

---

# XML

此 [!UICONTROL XML] 应用程序允许您通过 [!UICONTROL XML] > [!UICONTROL 解析XML] 模块并将其转换为捆绑包，以便其他模块也能使用该数据。 您还可以通过以下方式将包转换为XML格式文本 [!UICONTROL XML] > [!UICONTROL 创建XML] 模块

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

## [!UICONTROL 解析XML]

此 [!UICONTROL XML] > [!UICONTROL 解析XML] 模块解析XML格式文本并输出包含从XML提取的所有信息的单个包。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL数据结构]</p> </td> 
   <td> <p>数据结构描述了XML的结构，以使模块的输出在映射面板中可用于以下模块。</p> <p>如果您有要解析的XML示例，则可以使用该示例生成数据结构：</p> 
    <ol> 
     <li value="1">单击 <strong>[！UICONTROL添加]</strong> 按钮。</li> 
     <li value="2">单击 <strong>[！UICONTROL Generator]</strong> 按钮。</li> 
     <li value="3">将XML示例复制并粘贴到 <strong>[！UICONTROL示例数据]</strong> 字段。</li> 
     <li value="4">单击 <strong>[！UICONTROL保存]</strong>.</li> 
     <li value="5">验证是否已成功生成数据结构。</li> 
     <li value="6"> <p>单击 <strong>[！UICONTROL保存]</strong> 按钮以保存数据结构。</p> <p>可跳过步骤2-5以提供空的数据结构。 如果数据结构为空，则在至少执行一次模块之前，模块的输出在映射面板中不可用。</p> </li> 
    </ol> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">中的数据结构 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL保留数字为文本]</td> 
   <td>启用此选项可确保数字保持为文本（字符串）值。 否则，数字将转换为数字值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL XML]</p> </td> 
   <td> <p>输入或映射要解析的XML格式文本。</p> <p>如果使用公式，请确保其结果值类型是（或可以自动强制到）[！UICONTROL Text]数据类型。 </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>如果结果值类型为[！UICONTROL Buffer]（二进制数据），则使用 <code>toString()</code> 函数以将其转换为Text数据类型。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">键入强制 [!DNL Adobe Workfront Fusion]</a> 和 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">[！UICONTROL Adobe Workfront Fusion]中的项目数据类型</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 要从URL下载XML文件并解析其内容，请执行以下操作：
>
>1. 创建新方案。
>1. 插入 [!UICONTROL HTTP] > [!UICONTROL 获取文件] 模块
>1. 打开模块的配置，并按照以下方式对其进行配置：
>
>   **URL**： XML文件的URL(例如， `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. 单击 **[!UICONTROL 确定]**&#x200B;保存&#x200B;并关闭模块的配置。
1. 添加 [!UICONTROL XML] > [!UICONTROL 解析XML] 模块，将其连接在 [!UICONTROL HTTP] > [!UICONTROL 获取文件] 模块并按照以下方式对其进行配置：
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[！UICONTROL数据结构]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">单击 <strong>[！UICONTROL添加]</strong> 按钮。</li> 
&gt;        <li value="2">单击 <strong>[！UICONTROL Generator]</strong> 按钮。</li> 
&gt;        <li value="3">在Web浏览器中，打开新的选项卡或窗口。</li> 
&gt;        <li value="4">将您在第三步中使用的URL放入地址栏并获取XML文件。</li> 
&gt;        <li value="5">选择所有XML文本并将其复制到剪贴板中。</li> 
&gt;        <li value="6">关闭选项卡或窗口，然后返回到场景。</li> 
&gt;        <li value="7">将复制的XML文本粘贴到“示例数据”字段中。</li> 
&gt;        <li value="8">单击 <strong>[！UICONTROL保存]</strong>.</li> 
&gt;        <li value="9">验证是否已成功生成数据结构。</li> 
&gt;        <li value="10">单击 <strong>[！UICONTROL保存]</strong> 以保存数据结构。</li> 
&gt;       </ol> <p>可跳过步骤2至9以提供空的数据结构。 如果数据结构为空，则在至少执行一次模块之前，模块的输出在映射面板中不可用。</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[！UICONTROL XML]</td> 
&gt;      <td> <p>映射 <code>Data </code>[！UICONTROL HTTP] &gt; [！UICONTROL获取文件]模块输出中的项放入字段中。 使用 <code>toString()</code> 函数将其值从[！UICONTROL Buffer]（二进制数据）类型转换为[！UICONTROL Text]数据类型。</p> <p>您可以将公式的代码复制并粘贴到字段中： <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>有关Buffer和Text数据类型的详细信息，请参见 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion中的项目数据类型</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL 分析XML属性]

默认情况下， [!UICONTROL XML] > [!UICONTROL 解析XML] 模块将属性放入特殊集合中 `_attributes` 作为具有这些属性的节点的子节点。 如果节点是文本节点并且有属性，则会添加两个特殊属性： `_attributes` 属性和 `_value` 节点的文本内容。

>[!INFO]
>
**示例：** 此XML：

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

将转换为此捆绑包：

![](assets/xml-converted-to-bundle.png)

## 创建XML

此 [!UICONTROL XML] > [!UICONTROL 创建XML] 模块将捆绑包转换为XML格式文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL数据结构]</p> </td> 
   <td> <p>数据结构描述生成的XML的结构。 如果要创建的XML示例，可以使用该示例生成数据结构：</p> 
    <ol> 
     <li value="1">单击 <strong>[！UICONTROL添加]</strong> 按钮。</li> 
     <li value="2">单击 <strong>[！UICONTROL Generator]</strong> 按钮。</li> 
     <li value="3">将XML示例复制并粘贴到示例数据字段中。</li> 
     <li value="4">单击 <strong>[！UICONTROL保存]</strong> 按钮。</li> 
     <li value="5">验证是否已成功生成数据结构。</li> 
     <li value="6">单击 <strong>[！UICONTROL保存]</strong> 以保存数据结构。</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL根元素名称]</td> 
   <td>输入XML根元素的名称。 默认值为 <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Doctype系统ID]</td> 
   <td>输入要在以下位置使用的文件名：<code> !DOCTYPE SYSTEM</code> 声明</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Doctype公共ID]</td> 
   <td>输入要在以下位置使用的文件名：<code> !DOCTYPE PUBLIC</code> 声明</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL带Xml声明]</td> 
   <td>启用此选项可删除XML声明 <code>&lt;?xml ... ?&gt;</code> 和 <code>&lt;!DOCTYPE ... &gt;</code>和仅保留XML根元素及其内容。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**示例:**
>
典型用例是将数据从 [!DNL Google] >电子表格转换为XML。
>
1. 放置 [!DNL Google Sheets] > [!UICONTROL 选择行] 模块以获取数据。 设置模块以从检索行 [!DNL Google] 电子表格。 设置&#x200B;**[!UICONTROL 返回的最大行数]** 数量较少，但出于测试目的，会大于1（例如，3）。 执行 [!DNL Google Sheets] 模块，方法是右键单击该模块并选择“**[!UICONTROL 仅运行此模块]**.” 验证模块的输出。
1. 连接 [!UICONTROL 数组汇总] 模块位于 [!DNL Google Sheets] 模块。 在模块的设置中，选择 [!DNL Google Sheets] 中的模块 **[!UICONTROL 源节点]** 字段。 暂时保留其他字段不变。
1. 连接 [!UICONTROL XML] > [!UICONTROL 创建XML] 模块位于 [!UICONTROL 数组汇总] 模块。
>
模块的设置需要一个数据结构来描述XML输出的结构。 单击 **[!UICONTROL 添加]** 按钮以打开数据结构设置。 创建此数据结构的最简单方法是从XML示例自动生成它。
>
1. 单击 **[!UICONTROL 生成器]** 按钮并将XML示例粘贴到 [!UICONTROL 示例数据] 字段：
>
![](assets/sample-data-field-350x146.png)
>
1. 单击&#x200B;**[!UICONTROL 保存]**。Data structure中的Specification字段现在包含生成的结构。
1. 将数据结构的名称更改为更具体的名称，然后单击 **[!UICONTROL 保存]**. 与root数组属性对应的字段在JSON模块的设置中显示为可映射字段。
1. 单击 **[!UICONTROL 映射]** 按钮并映射 `Array[]` 项来自 [!UICONTROL 数组汇总] 输出到它：
1. 单击 **[!UICONTROL 确定]** 关闭XML模块的设置。
1. 打开 [!UICONTROL 数组汇总] 模块。 更改 **[!UICONTROL 目标结构]** 从自定义到与父XML元素对应的XML模块的字段。从映射项 [!DNL Google Sheets] 模块到相应的字段。
1. 单击 **[!UICONTROL 确定]** 以关闭阵列聚合器模块的设置。
1. 运行方案。
>
XML模块输出正确的XML文件。
>
1. 打开 [!DNL Google Sheets] 模块并增加 [!UICONTROL 返回的最大行数] 数，以大于电子表格中用于处理所有数据的行数。
>
生成的XML可以保存到 [!DNL Dropbox]，通过电子邮件以附件形式发送，通过FTP上传到服务器，等等。

## 添加XML属性

如果要将属性添加到复杂节点（将包含其他节点的节点），则必须添加一个名为的集合 `_attributes` 自定义数据结构中的复杂注释。 此集合将映射到节点属性。 如果要向文本节点添加属性(例如： `<node attr="1">abc</node>`)，则必须添加收藏集 `_attributes` 属性和文本属性 `_value` 自定义数据结构中此节点的节点值。

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## 故障排除：无法映射来自的数据 [!UICONTROL 解析XML] 模块

确保正确定义了数据结构。 或者，您可以使用空数据结构并至少执行一次该模块以处理XML输入。
