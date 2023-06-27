---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Google幻灯片模块
description: Adobe Workfront Fusion Google幻灯片模块允许您创建、更新、列出和/或删除演示文稿，并将图像上传到Google幻灯片帐户中的演示文稿。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 680a5328-1d50-4434-beda-7a4670a6e458
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# [!DNL Google Slides] 模块

此 [!DNL Adobe Workfront Fusion] [!DNL Google Slides] 通过模块，您可以创建、更新、列出和/或删除演示文稿，并将图像上传到中的演示文稿 [!DNL Google Slides] 帐户。

要使用 [!DNL Google Slides] 替换为 [!DNL Workfront Fusion]，则必须拥有 [!DNL Google] 帐户。 如果您没有 [!DNL Google] 帐户，则可以在以下位置创建一个 [!DNL Google] 帐户帮助页面。

您还需要 [!DNL Google Slides] 在您的 [!DNL Google Drive].

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

使用 [!DNL Google Slides] 模块，您必须具有 [!DNL Google] 帐户。

## [!DNL Google Slides] 模块及其字段

配置时 [!DNL Google Slides] 模块， Workfront Fusion将显示下面列出的字段。 除此以外，还有 [!DNL Google Slides] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [演示文稿](#presentation)
* [其他](#other)

### 演示文稿

* [[!UICONTROL 观看Presentations]](#watch-presentations)
* [[!UICONTROL 列出Presentations]](#list-presentations)
* [[!UICONTROL 获取演示]](#get-a-presentation)
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
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL监视] </td> 
   <td> <p>选择观看演示的选项：</p> 
    <ul> 
     <li> <p>[！UICONTROL创建日期]</p> </li> 
     <li> <p>[！UICONTROL修改日期]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>在一个场景执行周期内，Workfront Fusion应返回的最大演示文稿数。</p> </td> 
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
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器位置]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
     <li>[！UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹ID]</td> 
   <td> <p>选择要列出的演示文稿的文件夹位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制]</td> 
   <td> <p>演示文稿的最大数量 [!DNL Workfront Fusion] 应在一个场景执行周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取演示]

获取指定演示文稿的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
     <li>[！UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL演示文稿ID]</td> 
   <td> <p> 选择要检索的演示文稿。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取页面/缩略图]

获取指定页面或演示文稿中页面缩略图的最新版本。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL演示文稿ID]</td> 
   <td> <p> 选择要检索的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL页面对象ID]</td> 
   <td> <p> 选择要查看其页面对象详细信息的幻灯片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL显示页面缩略图]</td> 
   <td> <p> 如果要查看页面缩略图信息，请选中复选框。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 从模板创建演示]

通过替换所有标记（如）创建新演示文稿 `{{Name}}`， `{{Email}}` 在模板中提供数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标题] </td> 
   <td> <p>输入新演示文稿的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL复制演示]</td> 
   <td> <p> 如果要复制现有演示文稿，请选择选项：</p> 
    <ul> 
     <li>[！UICONTROL By Mapping]</li> 
     <li>[！UICONTROL By下拉列表]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL现有演示文稿ID的副本]</td> 
   <td> <p> 输入要复制的现有演示文稿的路径或演示文稿ID。 如果您正在通过映射创建演示文稿[！UICONTROL]，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
     <li>[！UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> <p>如果您正在创建演示文稿[！UICONTROL By Dropdown] ，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL演示文稿ID]</td> 
   <td> <p> 选择要用作模板的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值] </td> 
   <td> <p>添加值：</p> 
    <ul> 
     <li><strong>[！UICONTROL标记]</strong>：在演示文稿中输入要替换的标记。 例如， <code>&#123;&#123;Name&#125;&#125;</code></li> 
     <li><strong>[！UICONTROL替换值]</strong>：输入要替换现有标记的值。 例如，如果字符串 <tr><ul><tr><tr><tr><code>&#123;&#123;Name&#125;&#125;/code> in the presentation and the replaced value is Sample, then the <code>&#123;&#123;Name}}</code> will be replaced by <code>Sample</code>.</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL New Drive Location]</td> 
   <td> <p>Select the [!DNL Google Drive] where you want to store or add the new presentation:</p> 
     
     <li>[!UICONTROL My Drive]</li> 
     <li>[!UICONTROL Shared With Me]</li> 
     <li>[!UICONTROL [!DNL Google] Shared Drive]</li> 
    </ul> </td> 
  </tr> 
   
   <td role="rowheader"> <p>[!UICONTROL New Document's Location]</p> </td> 
   <td> <p>Select the folder where you want to store or add the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Shared] </td> 
   <td> <p>Select if you want to share the presentation.</p> </td> 
  </tr> 
   
   <td role="rowheader">[!UICONTROL Sharing with Other's Email Address]</td> 
   <td> <p> Enter the email address with whom you want to share the presentation. If you are not entering an email address and selecting only shared field, the presentation is shareable to anyone.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 将图像上传到演示文稿]

上传包含所提供数据的图像。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择演示]</td> 
   <td> <p>选择您希望如何选择将图像上传到的演示文稿。</p> 
    <ul> 
     <li>[！UICONTROL By Mapping]</li> 
     <li>[!DNL By Dropdown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
     <li>[！UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> <p>如果您正在创建演示文稿[！UICONTROL By Dropdown] ，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL演示文稿ID]</td> 
   <td> <p> 选择要将图像上传到的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL值]</td> 
   <td> <p>值添加值：</p> 
    <ul> 
     <li><strong>[！UICONTROL标记]</strong>：输入要将URL添加到其中的标记。</li> 
     <li><strong>[！UICONTROL图像URL]</strong>：输入要上传的图像的路径或URL。</li> 
    </ul> <p>注意：图像大小必须小于50MB，不能超过2500万像素，且必须采用PNG、JPEG或GIF格式。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 刷新图表]

刷新存储在ID指定的演示文稿中的图表数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
     <li>[！UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL演示文稿ID]</td> 
   <td> <p>选择包含要刷新图表的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL图表对象ID]</td> 
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
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择方法]</td> 
   <td> <p>选择要添加新幻灯片还是删除幻灯片。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Presentation ID]</td> 
   <td> <p>选择要为其添加或删除幻灯片的演示文稿的演示文稿ID。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL预定义的布局类型]</td> 
   <td> <p> 选择您希望添加的幻灯片使用的预定义幻灯片布局。 指定任何其他字段的值（如[！UICONTROL Title]）。</p> 
    <ul> 
     <li>[！UICONTROL空白布局，无占位符]</li> 
     <li>[！UICONTROL布局，底部有标题]</li> 
     <li>带有标题和子标题的[！UICONTROL布局]</li> 
     <li>带有标题和正文的[！UICONTROL布局]</li> 
     <li>[！UICONTROL布局，带标题和两列]</li> 
     <li>[！UICONTROL布局，仅带标题]</li> 
     <li>带有分区标题的[！UICONTROL布局]</li> 
     <li>[！UICONTROL布局，标题和副标题位于一侧，描述位于另一侧]</li> 
     <li>[！UICONTROL布局，有一个标题和一个正文，排列在一列中]</li> 
     <li>带主点的[！UICONTROL布局]</li> 
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
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>输入相对于https://developers.google.com/slides/的路径。 例如，演示文稿。</p> <p>有关可用端点的列表，请参阅 <a href="https://developers.google.com/slides/reference/rest">[!DNL Google Slides] API文档</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>输入所需的请求标头。 您无需添加授权标头。</p> </td> 
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

>[!INFO]
>
>**示例：** 使用API调用，您可以获取已输入演示文稿ID的演示详细信息。 在中打开演示文稿时，可以在URL中找到该演示文稿ID [!DNL Google Slides].
>
>![](assets/api-call-350x13.png)
>
>以下API调用返回演示详细信息：
>
>![](assets/presentation-details.png)
>
>搜索匹配项可在模块的输出中找到，位于 [!UICONTROL 捆绑] > [!UICONTROL 正文] > [!UICONTROL presentationId].
>
>在我们的示例中，返回了请求的演示详细信息：
>
>![](assets/presentation-details-2.png)

#### [!UICONTROL 在演示文稿中插入链接]

此模块使演示文稿中的所有链接都可点击，或将链接插入到所有匹配的输入文本中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接] </td> 
   <td> <p>有关连接 [!DNL Google Slides] 目标帐户 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择演示]</td> 
   <td> <p>选择您希望如何选择将图像上传到的演示文稿。</p> 
    <ul> 
     <li>[！UICONTROL By Mapping]</li> 
     <li>[！UICONTROL By下拉列表]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择驱动器]</td> 
   <td> <p>选择 [!DNL Google Drive] 要列出的演示文稿所在的位置：</p> 
    <ul> 
     <li>[！UICONTROL我的驱动器]</li> 
     <li>[！UICONTROL与我共享]</li> 
     <li>[！UICONTROL [!DNL Google] 共享驱动器]</li> 
    </ul> <p>如果您正在创建演示文稿[！UICONTROL By Dropdown] ，则会显示此字段。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL演示文稿ID]</td> 
   <td> <p>选择要列出的演示文稿的文件夹位置。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL选择]</td> 
   <td> <p>选择是要使演示文稿中的所有链接都可点击，还是要将链接插入到所有匹配的输入文本中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文本输入]</td> 
   <td>对于要为其添加链接的每个文本项，将项及其关联的链接添加到列表。 每次在演示文稿中显示项目时，它都会自动链接到指定的站点。</td> 
  </tr> 
 </tbody> 
</table>
