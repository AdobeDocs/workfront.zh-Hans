---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google幻灯片模块
description: 利用Adobe Workfront Fusion Google幻灯片模块，可创建、更新、列出和/或删除演示文稿，以及将图像上传到Google幻灯片帐户中的演示文稿。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1575'
ht-degree: 0%

---

# [!DNL Google Slides] 模块

的 [!DNL Adobe Workfront Fusion] [!DNL Google Slides] 模块允许您创建、更新、列出和/或删除演示文稿，以及将图像上传到您的演示文稿 [!DNL Google Slides] 帐户。

为了使用 [!DNL Google Slides] with [!DNL Workfront Fusion]，则需要具有 [!DNL Google] 帐户。 如果你没有 [!DNL Google] 帐户，您可以在 [!DNL Google] 帐户帮助页面。

您还需要 [!DNL Google Slides] 在 [!DNL Google Drive].

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
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

使用 [!DNL Google Slides] 模块，您必须 [!DNL Google] 帐户。

## [!DNL Google Slides] 模块及其字段

配置 [!DNL Google Slides] 模块中， Workfront Fusion会显示下面列出的字段。 除了这些， [!DNL Google Slides] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [演示](#presentation)
* [其他](#other)

### 演示

* [[!UICONTROL 观看Presentations]](#watch-presentations)
* [[!UICONTROL 列出Presentations]](#list-presentations)
* [[!UICONTROL 获取演示文稿]](#get-a-presentation)
* [[!UICONTROL 获取页面/缩略图]](#get-a-pagethumbnail)
* [[!UICONTROL 从模板创建演示]](#create-a-presentation-from-a-template)
* [[!UICONTROL 将图像上传到演示文稿]](#upload-an-image-to-a-presentation)
* [[!UICONTROL 刷新图表]](#refresh-a-chart)
* [[!UICONTROL 添加/删除幻灯片]](#adddelete-a-slide)

#### [!UICONTROL 观看Presentations]

创建或更新新演示文稿时触发。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch] </td> 
   <td> <p>选择用于观看演示文稿的选项：</p> 
    <ul> 
     <li> <p>[!UICONTROL创建日期]</p> </li> 
     <li> <p>[!UICONTROL修改日期]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>在一个方案执行周期中，Workfront Fusion应返回的演示文稿数上限。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出Presentations]

检索所有演示文稿的列表。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择驱动器位置]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[！与我共享的UICONTROL]</li> 
     <li>[!UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件夹ID]</td> 
   <td> <p>选择要列出的演示文稿的文件夹位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制]</td> 
   <td> <p>演示文稿的最大数量 [!DNL Workfront Fusion] 应在一个方案执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取演示文稿]

获取指定演示文稿的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[！与我共享的UICONTROL]</li> 
     <li>[!UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 选择要检索的演示文稿。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取页面/缩略图]

获取演示文稿中指定页面或页面缩略图的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 选择要检索的演示ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL页面对象ID]</td> 
   <td> <p> 选择要查看其页面对象详细信息的幻灯片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL显示页面缩略图]</td> 
   <td> <p> 如果要查看页面缩略图信息，请选中此复选框。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从模板创建演示]

通过替换 `{{Name}}`, `{{Email}}` 模板中提供的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标题] </td> 
   <td> <p>输入新演示文稿的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL复制演示文稿]</td> 
   <td> <p> 如果要复制现有演示文稿，请选择选项：</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！现有演示ID的UICONTROL副本]</td> 
   <td> <p> 输入要复制的现有演示文稿的路径或演示文稿ID。 如果要创建演示文稿[!UICONTROL By Mapping]，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[！与我共享的UICONTROL]</li> 
     <li>[!UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> <p>如果要创建演示文稿[!UICONTROL By Dropdown]，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 选择要用作模板的演示文稿的演示ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值] </td> 
   <td> <p>添加值：</p> 
    <ul> 
     <li><strong>[!UICONTROL标记]</strong>:输入要在演示文稿中替换的标记。 例如， <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[!UICONTROL替换值]</strong>:输入替换现有标记的值。 例如，如果字符串 <code>&#123;&#123;Name}}</code><code>Sample</code></li></ul></td></tr><tr><td role="rowheader"></td><td><p></p><ul><li></li><li></li><li></li></ul></td></tr><tr><td role="rowheader"><p></p></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr><tr><td role="rowheader"></td><td><p></p></td></tr></tbody></table>

#### [!UICONTROL 将图像上传到演示文稿]

上传包含提供数据的图像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择演示文稿]</td> 
   <td> <p>选择要选择将图像上传到的演示文稿的方式。</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[！与我共享的UICONTROL]</li> 
     <li>[!UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> <p>如果要创建演示文稿[!UICONTROL By Dropdown]，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p> 选择您要将图像上传到的演示文稿的演示ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL值]</td> 
   <td> <p>值添加值：</p> 
    <ul> 
     <li><strong>[!UICONTROL标记]</strong>:输入要将URL添加到的标记。</li> 
     <li><strong>[!UICONTROL图像URL]</strong>:输入要上传图像的路径或URL。</li> 
    </ul> <p>注意：图像的大小必须小于50MB，不能超过2500万像素，且必须采用PNG、JPEG或GIF格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刷新图表]

刷新ID指定的演示文稿中存储的图表数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[！与我共享的UICONTROL]</li> 
     <li>[!UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p>选择演示文稿的演示文稿ID，其中包含要刷新的图表。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL图表对象ID]</td> 
   <td> <p> 选择要刷新的图表。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添加/删除幻灯片]

创建空幻灯片或删除指定演示文稿上的现有幻灯片。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择方法]</td> 
   <td> <p>选择要添加新幻灯片还是删除幻灯片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>选择要为其添加或删除幻灯片的演示文稿的演示ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL预定义的布局类型]</td> 
   <td> <p> 选择您希望添加的幻灯片使用的预定义幻灯片布局。 指定任何其他字段的值（如[!UICONTROL标题]）。</p> 
    <ul> 
     <li>[!UICONTROL空白布局，无占位符]</li> 
     <li>[!UICONTROL布局，底部带有标题]</li> 
     <li>[！带标题和子标题的UICONTROL布局]</li> 
     <li>[！带有标题和正文的UICONTROL布局]</li> 
     <li>[！带标题和两列的UICONTROL布局]</li> 
     <li>[!UICONTROL布局（仅带标题）]</li> 
     <li>[！带有节标题的UICONTROL布局]</li> 
     <li>[!UICONTROL布局，一侧带有标题和子标题，另一侧带有描述]</li> 
     <li>[!UICONTROL布局，具有一个标题和一个主体，排列在一列中]</li> 
     <li>[！具有主点的UICONTROL布局]</li> 
     <li>[!DNL Layout with a big number heading]</li> 
    </ul> <p>如果您选择添加幻灯片，则此字段可用。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 进行API调用]](#make-an-api-call)
* [[!UICONTROL 在演示文稿中插入链接]](#insert-links-in-a-presentation)

#### [!UICONTROL 进行API调用]

执行任意授权的API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>输入相对于https://developers.google.com/slides/的路径。 例如，演示。</p> <p>有关可用端点的列表，请参阅 <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API文档</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>输入所需的请求标头。 您无需添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p> 输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**示例：** 通过API调用，您可以获取已输入演示ID的演示详细信息。 在中打开演示文稿时，您可以在URL中找到演示文稿ID [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>以下API调用会返回演示详细信息：
>
>![](assets/presentation-details.png)
>
>搜索的匹配项可在模块的输出下找到 [!UICONTROL 捆绑] > [!UICONTROL 正文] > [!UICONTROL presentationId].
>
>在本例中，返回了请求的演示详细信息：
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL 在演示文稿中插入链接]

此模块可使演示文稿中的所有链接都可点击，或将所有匹配的输入文本中插入一个链接。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择演示文稿]</td> 
   <td> <p>选择要选择将图像上传到的演示文稿的方式。</p> 
    <ul> 
     <li>[!UICONTROL By Mapping]</li> 
     <li>[!UICONTROL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[!UICONTROL My Drive]</li> 
     <li>[！与我共享的UICONTROL]</li> 
     <li>[!UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> <p>如果要创建演示文稿[!UICONTROL By Dropdown]，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL演示ID]</td> 
   <td> <p>选择要列出的演示文稿的文件夹位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select]</td> 
   <td> <p>选择是希望演示文稿中的所有链接都可点击，还是希望将链接插入所有匹配的输入文本中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文本输入]</td> 
   <td>对于要为其添加链接的每个文本项目，添加该项目及其关联的链接到列表。 每当项目出现在演示文稿中时，它都会自动链接到指定的网站。</td> 
  </tr> 
 </tbody> 
</table>
