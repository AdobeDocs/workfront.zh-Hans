---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: XML应用程序允许您通过XML &gt；解析XML格式的文本解析XML模块并将其转换为包，以使数据可供其他模块使用。 您还可以通过XML &gt；将包转换为XML格式的文本创建XML模块
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 1%

---

# XML

的 [!UICONTROL XML] 应用程序允许您通过 [!UICONTROL XML] > [!UICONTROL 解析XML] 模块，并将其转换为包，以使数据可供其他模块使用。 您还可以通过 [!UICONTROL XML] > [!UICONTROL 创建XML] 模块

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
  <td> <p>[!UICONTROL Pro]或更高版本</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
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

## [!UICONTROL 解析XML]

的 [!UICONTROL XML] > [!UICONTROL 解析XML] 模块解析XML格式的文本，并输出包含从XML中提取的所有信息的单个包。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL数据结构]</p> </td> 
   <td> <p>数据结构描述了XML的结构，以便在映射面板中为以下模块提供模块的输出。</p> <p>如果您有要解析的XML示例，则可以使用它生成数据结构：</p> 
    <ol> 
     <li value="1">单击 <strong>[!UICONTROL Add]</strong> 按钮。</li> 
     <li value="2">单击 <strong>[!UICONTROL生成器]</strong> 按钮。</li> 
     <li value="3">将XML示例复制并粘贴到 <strong>[!UICONTROL示例数据]</strong> 字段。</li> 
     <li value="4">单击 <strong>[!UICONTROL Save]</strong>.</li> 
     <li value="5">验证是否已成功生成数据结构。</li> 
     <li value="6"> <p>单击 <strong>[!UICONTROL Save]</strong> 按钮来保存数据结构。</p> <p>您可以跳过步骤2-5以提供空数据结构。 如果数据结构为空，则在至少执行一次模块之前，在映射面板中无法显示模块的输出。</p> </li> 
    </ol> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">中的数据结构 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL将数字保留为文本]</td> 
   <td>启用此选项可确保数字保持为文本（字符串）值。 否则，数字会被转换为数字值。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>输入或映射要解析的XML格式文本。</p> <p>如果使用公式，请确保其结果值类型是（或可以自动强制转换为）[!UICONTROL Text]数据类型。 </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>如果结果值类型为[!UICONTROL Buffer]（二进制数据），则使用 <code>toString()</code> 函数将其转换为文本数据类型。 有关更多信息，请参阅 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">在中键入强制 [!DNL Adobe Workfront Fusion]</a> 和 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的项目数据类型</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 要从URL下载XML文件并解析其内容，请执行以下操作：
>
>1. 创建新方案。
>1. 插入 [!UICONTROL HTTP] > [!UICONTROL 获取文件] 模块
>1. 打开模块的配置并按如下方式对其进行配置：

>
>   **URL**:XML文件的URL(例如， `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. 单击 **[!UICONTROL 确定]**&#x200B;保存并关闭模块的配置。
1. 添加 [!UICONTROL XML] > [!UICONTROL 解析XML] 模块，在 [!UICONTROL HTTP] > [!UICONTROL 获取文件] 模块并按如下方式对其进行配置：
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL数据结构]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">单击 <strong>[!UICONTROL Add]</strong> 按钮。</li> 
&gt;        <li value="2">单击 <strong>[!UICONTROL生成器]</strong> 按钮。</li> 
&gt;        <li value="3">在Web浏览器中，打开一个新的选项卡或窗口。</li> 
&gt;        <li value="4">将您在第三步中使用的URL放在地址栏中，并获取XML文件。</li> 
&gt;        <li value="5">选择所有XML文本并将其复制到剪贴板。</li> 
&gt;        <li value="6">关闭选项卡或窗口，然后返回到您的方案。</li> 
&gt;        <li value="7">将复制的XML文本粘贴到Sample data字段中。</li> 
&gt;        <li value="8">单击 <strong>[!UICONTROL Save]</strong>.</li> 
&gt;        <li value="9">验证是否已成功生成数据结构。</li> 
&gt;        <li value="10">单击 <strong>[!UICONTROL Save]</strong> 以保存数据结构。</li> 
&gt;       </ol> <p>您可以跳过步骤2至9以提供空数据结构。 如果数据结构为空，则在至少执行一次模块之前，在映射面板中无法显示模块的输出。</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>映射 <code>Data </code>[!UICONTROL HTTP] &gt; [!UICONTROL获取文件]模块的输出中的项目添加到字段中。 使用 <code>toString()</code> 函数将其值从[!UICONTROL缓冲区]（二进制数据）类型转换为[!UICONTROL文本]数据类型。</p> <p>您可以将公式的代码复制并粘贴到字段中： <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>有关缓冲和文本数据类型的详细信息，请参阅 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion中的项目数据类型</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>


## [!UICONTROL 解析XML属性]

默认情况下， [!UICONTROL XML] > [!UICONTROL 解析XML] 模块将属性放入特殊收藏集 `_attributes` 作为具有这些属性的节点的子项。 如果节点是文本节点，并且具有属性，则会添加两个特殊属性： `_attributes` 对于属性和 `_value` 的文本内容。

>[!INFO]
**示例：** 此XML:

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

将转换为此包：

![](assets/xml-converted-to-bundle.png)

## 创建XML

的 [!UICONTROL XML] > [!UICONTROL 创建XML] 模块将包转换为XML格式的文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL数据结构]</p> </td> 
   <td> <p>数据结构描述生成的XML的结构。 如果您有要创建的XML示例，则可以使用它生成数据结构：</p> 
    <ol> 
     <li value="1">单击 <strong>[!UICONTROL Add]</strong> 按钮。</li> 
     <li value="2">单击 <strong>[!UICONTROL生成器]</strong> 按钮。</li> 
     <li value="3">将XML示例复制并粘贴到Sample数据字段中。</li> 
     <li value="4">单击 <strong>[!UICONTROL Save]</strong> 按钮。</li> 
     <li value="5">验证是否已成功生成数据结构。</li> 
     <li value="6">单击 <strong>[!UICONTROL Save]</strong> 以保存数据结构。</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL根元素名称]</td> 
   <td>输入XML的根元素的名称。 默认值为 <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>输入要在<code> !DOCTYPE SYSTEM</code> 声明</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>输入要在<code> !DOCTYPE PUBLIC</code> 声明</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml声明]</td> 
   <td>启用此选项可删除XML声明 <code>&lt;?xml ... ?&gt;</code> 和 <code>&lt;!DOCTYPE ... &gt;</code>并仅保留XML根元素及其内容。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
**示例:**
典型的用例是从 [!DNL Google] 将电子表格转换为XML。
1. 将 [!DNL Google Sheets] > [!UICONTROL 选择行] 模块来获取数据。 设置模块以从 [!DNL Google] 电子表格。 设置&#x200B;**[!UICONTROL 返回的最大行数]** 值较小，但出于测试目的大于1（例如，3）。 执行 [!DNL Google Sheets] 模块，方法是右键单击该模块并选择“**[!UICONTROL 仅运行此模块]**.&quot; 验证模块的输出。
1. 连接 [!UICONTROL 阵列聚合器] 模块之后 [!DNL Google Sheets] 模块。 在模块的设置中，选择 [!DNL Google Sheets] 模块 **[!UICONTROL 源节点]** 字段。 暂时保留其他字段。
1. 连接 [!UICONTROL XML] > [!UICONTROL 创建XML] 模块之后 [!UICONTROL 阵列聚合器] 模块。
   模块的设置需要描述XML输出结构的数据结构。 单击 **[!UICONTROL 添加]** 按钮以打开数据结构设置。 创建此数据结构的最简单方法是从XML示例自动生成此数据结构。
1. 单击 **[!UICONTROL 发电机]** 按钮并将XML示例粘贴到 [!UICONTROL 示例数据] 字段：

![](assets/sample-data-field-350x146.png)
1. 单击&#x200B;**[!UICONTROL 保存]**。“数据结构”中的“规范”字段现在包含生成的结构。
1. 将数据结构的名称更改为更具体的内容，然后单击 **[!UICONTROL 保存]**. 与根数组属性对应的字段在JSON模块的设置中显示为可映射的字段。
1. 单击 **[!UICONTROL 地图]** 按钮，并映射 `Array[]` 项目 [!UICONTROL 阵列聚合器] 输出到它：
1. 单击 **[!UICONTROL 确定]** 关闭XML模块的设置。
1. 打开的设置 [!UICONTROL 阵列聚合器] 模块。 更改 **[!UICONTROL 目标结构]** 从自定义到与父XML元素对应的XML模块字段。映射 [!DNL Google Sheets] 模块。
1. 单击 **[!UICONTROL 确定]** 关闭阵列聚合器模块的设置。
1. 运行方案。

   XML模块输出正确的XML文件。
1. 打开的设置 [!DNL Google Sheets] 模块并增加 [!UICONTROL 返回的最大行数] 值大于电子表格中的行数以处理所有数据。
   生成的XML可保存到 [!DNL Dropbox]、通过电子邮件作为附件发送、通过FTP上传到服务器等。


## 添加XML属性

如果要向复杂节点（将包含其他节点的节点）添加属性，则必须添加名为的集合 `_attributes` ，以了解自定义数据结构中的复杂注释。 此集合将映射到节点属性。 如果要向文本节点添加属性(例如： `<node attr="1">abc</node>`)，则必须添加收藏集 `_attributes` 属性和文本属性的 `_value` 用于自定义数据结构中此节点的节点值。

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

## 疑难解答：无法映射 [!UICONTROL 解析XML] 模块

确保正确定义数据结构。 或者，您可以使用空数据结构并至少执行一次模块以处理XML输入。
