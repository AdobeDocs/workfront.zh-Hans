---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google文档模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '4160'
ht-degree: 0%

---

# [!DNL Google Docs]模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [Google Docs模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-docs-modules.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

通过[!DNL Adobe Workfront Fusion] [!DNL Google Docs]模块，您可以在[!DNL Google Docs]和[!DNL Google Docs]（针对[!DNL Google Workspace]用户）中监视、创建、编辑和检索文档。

要将[!DNL Google Docs]与[!DNL Adobe Workfront Fusion]一起使用，需要具有[!DNL Google]帐户。 如果您还没有[!DNL Google]帐户，则可以在[!DNL Google]帐户帮助页面中创建一个帐户。

如果需要有关创建方案的说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

有关模块的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)中的[模块。

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
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr>
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 先决条件

要使用[!DNL Google Docs]模块，您必须拥有Google帐户。

## Google Docs API信息

Google Docs连接器使用以下对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td> https://docs.googleapis.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API版本</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v1.4.13</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Docs]模块及其字段

在配置[!DNL Google Docs]模块时，[!UICONTROL Workfront Fusion]显示以下列出的字段。 除此以外，可能还会显示其他[!DNL Google Docs]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

### 文档

* [[!UICONTROL 观看文档]](#watch-documents)
* [[!UICONTROL 列出文档]](#list-documents)
* [[!UICONTROL 获取文档的内容]](#get-content-of-a-document)
* [[!UICONTROL 创建文档]](#create-a-document)
* [[!UICONTROL 从模板创建文档]](#create-a-document-from-a-template)
* [[!UICONTROL 向文档插入段落]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL 将图像插入文档]](#insert-an-image-to-a-document)
* [[!UICONTROL 用新图像替换图像]](#replace-an-image-with-a-new-image)
* [[!UICONTROL 替换文档中的文本]](#replace-text-in-a-document)
* [[!UICONTROL 下载文档]](#download-a-document)
* [[!UICONTROL 删除文档]](#delete-a-document)

#### [!UICONTROL 观看文档]

在所选文件夹中创建或修改新文档时，此触发器模块返回文档详细信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Watch文档]</td> 
   <td> <p style="color: #000000;">选择您是要观看已创建的([！UICONTROL By Created Date])文档还是已修改的([！UICONTROL By Modified Date])文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要监视的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要监视创建或修改文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要监视创建或修改文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要监视的共享驱动器。</p> <p>注意：如果您在此字段中选择了[!DNL Google Shared Drive]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置Workfront Fusion在一个执行周期中返回的最大文档数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出文档]

此操作模块从选定的文件夹中检索文档列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要从中列出文档的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要从中列出文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要从中列出文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要从中列出文档的共享驱动器。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置在一个执行周期中返回的最大文档数[!DNL Workfront Fusion]。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文档的内容]

此操作模块检索指定文档。

您可能需要扩展您的权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
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
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择包含要检索的文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择包含要检索的文档的共享驱动器。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL筛选器]</p> </td> 
   <td> <p>选择您希望模块输出中返回的对象。</p> 
    <ul> 
     <li>[！UICONTROL Image]（默认）</li> 
     <li>[！UICONTROL Drawing]</li> 
     <li>[！UICONTROL图表]</li> 
    </ul> <p>注意：  <p>要进一步映射这些对象，请在此模块的输出中使用[！UICONTROL Inline Objects Array]值（而不是[！UICONTROL inlineObjects]）。</p> <p>[！UICONTROL Inline Objects Array]对象按照它们在文档中的显示顺序排序。 这将使任何进一步的处理更容易。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文档]

此操作模块允许您在选定文件夹中创建新文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
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
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要创建文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要创建文档的共享驱动器。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入标头]</td> 
   <td> <p> 启用此选项可将页眉插入到文档，然后输入或映射页眉的文本。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL插入页脚] </td> 
   <td> <p>启用此选项可将页脚插入文档，然后输入或映射页眉的文本。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL从模板创建文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>选择此选项可从下拉菜单中选择文档模板。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择模板所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择模板所在的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择模板所在的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择模板所在的共享驱动器。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Values]</p> </td> 
   <td> <p>输入将输入的值，而不是新文档的变量。</p> 
    <ul> 
     <li><strong>[！UICONTROL标记]</strong> <br>输入文档模板中包含的标记。 不要使用<code>&#123;&#123;&#125;&#125;</code>。 示例：使用<code>name</code>而不是<code>&#123;&#123;name&#125;&#125;</code>。</li> 
     <li><strong>[！UICONTROL替换的值]</strong><br>输入标记的值。</li> 
    </ul> <p>例如，源文档中的<code> &#123;&#123;name&#125;&#125;</code>变量将显示为此处的name字段，可以插入该值，如<code>John</code>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL图像替换]</p> </td> 
   <td> <p>输入要替换当前图像的[！UICONTROL图像对象ID]和[！UICONTROL图像URL]的链接。</p> <p>注意：您可以使用[！UICONTROL获取文档]模块检索图像ID，其中ID包含在数组[！UICONTROL内联对象数组]中。</p> <p>我们建议您向[!DNL Google]文档中的图像添加替换文字。 </p> <p>向[!DNL Google Docs]图像添加替换文本：</p> 
    <ol> 
     <li value="1">右键单击图像。</li> 
     <li value="2">选择[！UICONTROL替换文本]选项。</li> 
     <li value="3">在[！UICONTROL标题]字段中输入[！UICONTROL替换文本]，然后单击[！UICONTROL确定]。</li> 
    </ol> <p>将ALT文本添加到图像后，ALT文本显示在括号中的字段名称中。</p> </td> 
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
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要创建文档的文件夹。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要创建文档的共享驱动器。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 向文档插入段落]

此操作模块可在现有文档中添加或插入新段落。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要添加段落的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要添加段落的文档所在的文件夹，然后选择文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要添加段落的文档所在的文件夹，然后选择文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要向其添加段落的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL插入段落]</p> </td> 
   <td> <p>选择希望新文本插入文档的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL，按位置规范]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL，按索引]</strong> </p> 
        <ul> 
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>输入要插入文本的索引编号。 您可以使用[！UICONTROL Get a Document]模块检索索引号。</p> <p>要显示文档中的所有字符（包括隐藏字符），您可以使用[！UICONTROL Show]加载项。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到该加载项。 搜索[！UICONTROL Show]并安装[！UICONTROL Show]加载项。</p> </li> 
         <li> <p><strong>[！UICONTROL插入文本]</strong> </p> <p>输入要插入到文档的文本。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL，按区段ID]</strong> </p> <p>选择要插入文本内容的页眉和页脚，并输入要插入到相应字段中的文本。</p> <p>如果页眉或页脚已包含文本，则新文本将添加到现有文本之前。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL，附加到文档正文中]</strong> </p> <p>在文档正文内容的末尾附加输入的文本。</p> <p>新段落的样式将从当前插入索引处的段落中复制，包括列表和项目符号。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，附加到区段（页眉和页脚）的末尾]</strong> </p> <p>选择要插入文本内容的页眉和页脚，并输入要插入到相应字段中的文本。</p> <p>如果页眉或页脚已包含文本，则新文本将添加到现有文本之后。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL附加文本]</td> 
   <td>输入或映射要附加到文档的文本</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将图像插入文档]

此操作模块会将图像从URL插入到文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要添加图像的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要添加图像的文档所在的文件夹，然后选择文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要添加图像的文档所在的文件夹，然后选择文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要添加图像的文档所在的共享驱动器，然后选择文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL插入图像]</p> </td> 
   <td> <p>选择您希望新图像插入到文档中的方式。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL，按位置规范]</strong> </p> 
      <ul> 
       <li> <p><strong>[！UICONTROL，按索引]</strong> </p> 
        <ul> 
         <li> <p><strong>[！UICONTROL索引]</strong> </p> <p>输入要插入图像的索引编号。 您可以使用[！UICONTROL Get a Document]模块检索[！UICONTROL索引号]。</p> <p>要显示文档中的所有字符（包括隐藏字符），您可以使用[！UICONTROL Show]加载项。 您可以在[！UICONTROL Add-ons] &gt; [！UICONTROL Get add-ons]下找到该加载项。 搜索[！UICONTROL Show]并安装[！UICONTROL Show]加载项。</p> </li> 
         <li> <p><strong>[！UICONTROL图像URL]</strong> </p> <p>输入要插入文档的图像的URL。</p> <p>最大图像大小为50 MB。 不得超过2500万像素。 仅支持PNG、JPEG或GIF格式。</p> </li> 
        </ul> </li> 
       <li> <p><strong>[！UICONTROL，按区段ID]</strong> </p> <p>选择要将图像插入到的页眉和页脚，并在相应的字段中输入图像URL。</p> <p>最大图像大小为50 MB。 图像不能超过2500万像素。 仅支持PNG、JPEG或GIF格式。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL，附加到文档正文中]</strong> </p> <p>在文档正文内容的末尾附加特定图像。</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL，附加到区段（页眉和页脚）的末尾]</strong> </p> <p>选择要插入图像的页眉和页脚，并输入要插入到相应字段的图像URL。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL高度模（以点为单位）/宽度模（以点为单位）]</p> </td> 
   <td> <p>定义插入图像的大小。 将保持宽高比。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要替换图像的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要替换图像的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要替换图像的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要替换图像的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL图像URL]</p> </td> 
   <td> <p>输入或映射将替换现有图像的新图像的URL。</p> <p>图像按其在文档中的显示顺序列出。 例如，<code>Body: Image No. 1</code>是文档中的第一个图像。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL选择文档]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要向其添加文本的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要向其添加文本的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要向其添加文本的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要向其添加文本的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
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

此操作模块转换并下载所选文档。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要下载的文档所在的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要下载的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要下载的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要下载的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要删除的文档所在的驱动器类型。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要删除的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要删除的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要删除的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共享驱动器]</td> 
   <td> <p>选择包含要下载的文档的驱动器，然后选择文档。 如果您在[！UICONTROL选择驱动器]字段中选择了[!DNL Google Docs]，则此选项可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文档ID]</td> 
   <td> <p> 选择或映射要替换其中一个或多个图像的文档。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 进行API调用]](#make-an-api-call)
* [[!UICONTROL 使文档中的所有链接都可点击]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL 进行API调用]

此操作模块允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection] </td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>输入相对于<code>https://docs.googleapis.com/</code>的路径。 示例： <code>/v1/documents/{presentationID}</code>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP请求方法。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。例如，<code>{"Content-type":"application/json"}</code>。 [!DNL Workfront Fusion]为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p> 输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：**&#x200B;以下API调用检索Google Docs中指定文档的详细信息：

**URL：**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**方法：**

[!UICONTROL GET]

![](assets/api-call-example.png)

在[!UICONTROL 包] > [!UICONTROL 正文]下的模块输出中可找到检索文档的详细信息。

![](assets/api-output.png)

#### [!UICONTROL 使文档中的所有链接都可点击]

此操作模块查找文档中的所有链接并使它们可点击。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Google]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!DNL Adobe Workfront Fusion]</a>中创建方案一文中的<a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">将模块的应用或Web服务连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL Make All Links in a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL By Mapping]</strong> <br>选择此选项以映射文档模板。</li> 
     <li><strong>[！UICONTROL By Dropdown]</strong> <br>选择此选项可从下拉菜单中选择文档。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择要使链接可点击的文档所在的驱动器类型。 如果您在上一个字段中选择了[！UICONTROL By Dropdown] ，则此选项可用。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL我的驱动器]</strong> </p> <p>选择要使链接可点击的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL已与我共享]</strong> </p> <p>选择要使链接可点击的文档所在的文件夹，然后选择该文档。</p> </li> 
     <li> <p><strong>[！UICONTROL [!DNL Google]共享驱动器]</strong> （仅适用于[!DNL Google Workspace]用户）</p> <p>选择是否希望[！UICONTROL使用域管理员访问权限]。 选择[！UICONTROL是]会以域管理员身份发出请求，并且会返回请求者是管理员的所有共享驱动器。</p> <p>选择要使链接可点击的文档所在的共享驱动器，然后选择该文档。</p> <p>注意：如果您在此字段中选择了[!DNL Google Docs]选项，并且您不是[!DNL Google Workspace]用户，则会返回错误<code>[400] Invalid Value</code>。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL共享驱动器]</td> 
   <td> <p>选择包含要更新链接的文档的驱动器，然后选择文档。 如果您在[！UICONTROL选择驱动器字段]中选择了[!DNL Google Docs]，则此选项可用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文档ID]</td> 
   <td> <p> 选择或映射要更新链接的文档。</p> </td> 
  </tr> 
 </tbody> 
</table>
