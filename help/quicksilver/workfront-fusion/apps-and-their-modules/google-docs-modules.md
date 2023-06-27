---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google文档模块
description: Adobe Workfront Fusion [!DNL Google Docs] 模块允许您监视、创建、编辑和检索中的文档 [!DNL Google Docs] 和 [!DNL Google Docs] （对于[！DNL G Suite]用户）。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '4090'
ht-degree: 0%

---

# [!DNL Google Docs] 模块

此 [!DNL Adobe Workfront Fusion] [!DNL Google Docs] 模块允许您监视、创建、编辑和检索中的文档 [!DNL Google Docs] 和 [!DNL Google Docs] (对于 [!DNL G Suite] 用户)。

要使用 [!DNL Google Docs] 替换为 [!DNL Adobe Workfront Fusion]，则必须拥有 [!DNL Google] 帐户。 如果您没有 [!DNL Google] 帐户，则可以在以下位置创建一个 [!DNL Google] 帐户帮助页面。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## 先决条件

使用 [!DNL Google Docs] 模块时，您必须拥有Google帐户。

## [!DNL Google Docs] 模块及其字段

配置时 [!DNL Google Docs] 模块， [!UICONTROL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Google Docs] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 文档

* [[!UICONTROL Watch文档]](#watch-documents)
* [[!UICONTROL 列出文档]](#list-documents)
* [[!UICONTROL 获取文档内容]](#get-content-of-a-document)
* [[!UICONTROL 创建文档]](#create-a-document)
* [[!UICONTROL 从模板创建文档]](#create-a-document-from-a-template)
* [[!UICONTROL 在文档中插入段落]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL 将图像插入到文档]](#insert-an-image-to-a-document)
* [[!UICONTROL 用新图像替换图像]](#replace-an-image-with-a-new-image)
* [[!UICONTROL 替换文档中的文本]](#replace-text-in-a-document)
* [[!UICONTROL 下载文档]](#download-a-document)
* [[!UICONTROL 删除文档]](#delete-a-document)

#### [!UICONTROL Watch文档]

在所选文件夹中创建或修改新文档时，此触发器模块返回文档详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Watch文档]</td> 
   <td> <p style="color: #000000;">选择是要观看已创建([！UICONTROL By Created Date])文档还是已修改([！UICONTROL By Modified Date])文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要监视的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要监视创建或修改文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要监视创建或修改文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要监视的共享驱动器。</p> <p>注意：如果已选择 [!DNL Google Shared Drive] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置Workfront Fusion在一个执行周期内返回的最大文档数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出文档]

此操作模块从所选文件夹检索文档列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要从中列出文档的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要从中列出文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要从中列出文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要从中列出文档的共享驱动器。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置最大文档数 [!DNL Workfront Fusion] 在一个执行周期内返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文档内容]

此操作模块检索指定的文档。

您可能需要扩展您的权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Get Content of a Document]</td> 
   <td> <p>选择是要映射文档的文档ID，还是手动从下拉菜单中选择文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择包含要检索的文档的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择包含要检索的文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择包含要检索的文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择包含要检索的文档的共享驱动器。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL筛选器]</p> </td> 
   <td> <p>选择您希望在模块输出中返回的对象。</p> 
    <ul> 
     <li>[！UICONTROL图像]（默认）</li> 
     <li>[！UICONTROL Drawing]</li> 
     <li>[！UICONTROL图表]</li> 
    </ul> <p>注释:  <p>要进一步映射这些对象，请在此模块的输出中使用[！UICONTROL内联对象数组]值（而不是[！UICONTROL inlineObjects]）。</p> <p>[！UICONTROL Inline Objects Array]对象按照它们在文档中的显示顺序排序。 这样一来，任何进一步处理都会更轻松。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文档]

此操作模块允许您在选定的文件夹中创建新文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL名称] </td> 
   <td> <p>输入文档的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL内容]</td> 
   <td> <p>输入文档的内容。 支持HTML。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要创建文档的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要创建文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要创建文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要创建文档的共享驱动器。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入标头]</td> 
   <td> <p> 启用此选项可将页眉插入到文档，然后输入或映射页眉的文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入页脚] </td> 
   <td> <p>启用此选项可将页脚插入到文档，然后输入或映射页眉的文本。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从模板创建文档]

此操作模块会创建现有模板文档的副本并替换任何标记。 此模块还允许用户按URL将图像替换为新图像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL从模板创建文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By下拉列表]</strong> <br>选择此选项可从下拉菜单中选择文档模板。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择模板所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择模板所在的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择模板所在的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择模板所在的共享驱动器。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL值]</p> </td> 
   <td> <p>输入将输入的值而不是新文档的变量。</p> 
    <ul> 
     <li><strong>[！UICONTROL标记]</strong> <br>输入文档模板中包含的标记。 不使用 <code>&#123;&#123;&#125;&#125;</code>. 示例：use <code>name</code> 而不是 <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[！UICONTROL替换值]</strong><br>输入标记的值。</li> 
    </ul> <p>例如，<code> &#123;&#123;name&#125;&#125;</code> 源文档中的变量将显示为“名称”字段，可在其中插入值，例如 <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL图像替换]</p> </td> 
   <td> <p>输入将替换当前图像的[！UICONTROL图像对象ID]和[！UICONTROL图像URL]的链接。</p> <p>注意：您可以使用[！UICONTROL获取文档]模块检索图像ID，其中ID包含在数组[！UICONTROL内联对象数组]中。</p> <p>我们建议您向中的图像添加替换文字 [!DNL Google] 文档。 </p> <p>将替换文字添加到 [!DNL Google Docs] 图像：</p> 
    <ol> 
     <li value="1">右键单击图像。</li> 
     <li value="2">选择[！UICONTROL替换文本]选项。</li> 
     <li value="3">在[！UICONTROL标题]字段中输入[！UICONTROL替换文本]，然后单击[！UICONTROL确定]。</li> 
    </ol> <p>在将ALT文本添加到图像后，ALT文本会显示在字段名称中，并以括号括住。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标题] </td> 
   <td> <p>输入新文档的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择模板所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要创建文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要创建文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要在其中创建文档的共享驱动器。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 在文档中插入段落]

此操作模块可向现有文档追加或插入新段落。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档。</li> 
     <li><strong>[！UICONTROL By下拉列表]</strong> <br> 选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要添加段落的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要添加段落的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要添加段落的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要添加段落的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL插入段落]</p> </td> 
   <td> <p>选择希望新文本插入文档的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL按位置规范]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL By Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>输入要在其中插入文本的索引号。 您可以使用[！UICONTROL Get a Document]模块检索索引号。</p> <p>要显示文档中的所有字符（包括隐藏字符），您可以使用[！UICONTROL Show]加载项。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到该加载项。 搜索[！UICONTROL Show]并安装[！UICONTROL Show]加载项。</p> </li> 
         <li> <p><strong>[！UICONTROL插入的文本]</strong> </p> <p>输入要插入到文档的文本。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL，按区段ID]</strong> </p> <p>选择要插入文本内容的页眉和页脚，然后输入要插入到相应字段的文本。</p> <p>如果页眉或页脚已包含文本，则新文本将添加到现有文本之前。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL通过附加到文档正文中]</strong> </p> <p>在文档正文内容的末尾附加输入的文本。</p> <p>新段落的样式将从当前插入索引处的段落中复制，包括列表和项目符号。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，附加到区段（页眉和页脚）的末尾</strong> </p> <p>选择要插入文本内容的页眉和页脚，然后输入要插入到相应字段的文本。</p> <p>如果页眉或页脚已包含文本，则新文本将添加到现有文本之后。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附加文本]</td> 
   <td>输入或映射要附加到文档的文本</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将图像插入到文档]

此操作模块将一个图像从URL插入到文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By下拉列表]</strong> <br> 选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要添加图像的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要添加图像的文档所在的文件夹，然后选择文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要添加图像的文档所在的文件夹，然后选择文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要添加图像的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL插入图像]</p> </td> 
   <td> <p>选择您希望新图像插入到文档中的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL按位置规范]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL By Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>输入要插入图像的索引编号。 您可以使用[！UICONTROL Get a Document]模块检索[！UICONTROL索引号]。</p> <p>要显示文档中的所有字符（包括隐藏字符），您可以使用[！UICONTROL Show]加载项。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到该加载项。 搜索[！UICONTROL Show]并安装[！UICONTROL Show]加载项。</p> </li> 
         <li> <p><strong>[！UICONTROL图像URL]</strong> </p> <p>输入要插入到文档中的图像的URL。</p> <p>最大图像大小为50 MB。 不得超过2500万像素。 仅支持PNG、JPEG或GIF格式。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL，按区段ID]</strong> </p> <p>选择要将图像插入到的页眉和页脚，并将图像URL输入到相应的字段。</p> <p>最大图像大小为50 MB。 图像不能超过2500万像素。 仅支持PNG、JPEG或GIF格式。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL通过附加到文档正文中]</strong> </p> <p>在文档正文内容的末尾附加特定图像。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，附加到区段（页眉和页脚）的末尾</strong> </p> <p>选择要插入图像的页眉和页脚，然后输入要插入到相应字段的图像URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL以点为单位的高度量值/以点为单位的宽度量值]</p> </td> 
   <td> <p>定义插入图像的大小。 将保持纵横比。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 用新图像替换图像]

此操作模块替换现有图像。 将保持原始图像的纵横比。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By下拉列表]</strong> <br> 选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要替换图像的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要替换图像的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要替换图像的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要替换图像的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL图像URL]</p> </td> 
   <td> <p>输入或映射将替换现有图像的新图像的URL。</p> <p>图像按其在文档中的显示顺序列出。 例如， <code>Body: Image No. 1</code> 是文档中的第一个图像。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 替换文档中的文本]

此操作模块替换文档中的文本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By下拉列表]</strong> <br> 选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要向其添加文本的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要向其添加文本的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要向其添加文本的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要向其添加文本的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL替换文本]</p> </td> 
   <td> <p>添加要替换的每个文本。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL要替换的旧文本]</strong> </p> <p>输入要替换的文本。</p> </li> 
     <li> <p><strong>[！UICONTROL要插入的新文本]</strong> </p> <p>输入新文本。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载文档]

此操作模块转换和下载所选文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要下载的文档所在的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要下载的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要下载的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要下载的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL类型] </p> </td> 
   <td> <p>选择下载文档的目标文件格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文档]

此操作模块删除文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要删除的文档所在的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要删除的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要删除的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要删除的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共享驱动器]</td> 
   <td> <p>选择包含要下载的文档的驱动器，然后选择文档。 如果已选择，则此选项可用 [!DNL Google Docs] 在[！UICONTROL选择驱动器]字段中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文档ID]</td> 
   <td> <p> 选择或映射要替换一个或多个图像的文档。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 进行API调用]](#make-an-api-call)
* [[!UICONTROL 使文档中的所有链接可点击]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL 进行API调用]

此操作模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>输入相对路径 <code>https://docs.googleapis.com/</code>. 示例: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如， <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] 为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：** 以下API调用检索Google文档中指定文档的详细信息：

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**方法:**

[!UICONTROL GET]

![](assets/api-call-example.png)

在模块的“输出”下可找到所检索文档的详细信息 [!UICONTROL 捆绑] > [!UICONTROL 正文].

![](assets/api-output.png)

#### [!UICONTROL 使文档中的所有链接可点击]

此操作模块查找文档中的所有链接并使它们可点击。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL Google] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用程序或Web服务连接到 [!DNL Workfront Fusion]</a> 在文章中 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在中创建方案 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Make All Links in a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By下拉列表]</strong> <br> 选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要使链接可点击的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要使链接可单击的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL与我共享]</strong> </p> <p>选择要使链接可单击的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google] 共享驱动器]</strong> (适用于 [!DNL G Suite] 仅限用户)</p> <p>选择是否要[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并返回请求者是管理员的所有共享驱动器。</p> <p>选择要使链接可单击的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果已选择 [!DNL Google Docs] 选项，而您不是 [!DNL G Suite] 用户，错误 <code>[400] Invalid Value</code> 会返回。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共享驱动器]</td> 
   <td> <p>选择包含要更新链接的文档的驱动器，然后选择文档。 如果已选择，则此选项可用 [!DNL Google Docs] 在[！UICONTROL中选择驱动器字段]中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文档ID]</td> 
   <td> <p> 选择或映射要更新链接的文档。</p> </td> 
  </tr> 
 </tbody> 
</table>
