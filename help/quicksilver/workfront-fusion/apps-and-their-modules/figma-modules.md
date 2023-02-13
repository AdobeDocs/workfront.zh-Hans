---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Figma模块
description: 使用 [!DNL Adobe Workfront Fusion] 在图像模块中，您可以检索注释、文件、文件版本或项目列表。 您还可以发布评论或调用Figma API。
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2261'
ht-degree: 1%

---

# [!DNL Figma] 模块

使用 [!DNL Adobe Workfront Fusion] [!DNL Figma] 模块中，您可以检索注释、文件、文件版本或项目列表。 您还可以发布评论或调用 [!DNL Figma] API。

如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
      <td>
        <p>[!UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
      <td>
        <p>[!UICONTROL Plan]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成）</p>
      </td>
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

使用 [!DNL Figma] 模块，您必须 [!DNL Figma] 帐户。

## [!DNL Figma] 模块及其字段

配置 [!DNL Figma] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Figma] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [注释](#comments)

* [项目和文件](#projects-and-files)

* [组件和样式](#components-and-styles)

* [其他](#other)


### 注释

* [删除评论](#delete-a-comment)

* [列出注释](#list-comments)

* [发布评论](#post-a-comment)


#### [!UICONTROL 删除评论]

此操作模块会从文件中删除单个注释。

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL文件ID]</td>
      <td>输入或映射要从中添加注释的文件的文件ID。 </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL注释]</td>
      <td>输入要删除的评论文本。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出注释]

此搜索模块列出了 [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL文件ID]</td>
      <td>
        <p>输入或映射要为其检索注释的文件的文件ID。 </p>
        <ul>
          <li>
            <p>如果您不知道该ID，请单击 <b>[!UICONTROL查找文件]</b> 然后输入或映射与文件关联的项目ID，然后选择该文件。</p>
          </li>
          <li>
            <p>如果您不知道项目的ID，请单击 <b>[!UICONTROL查找项目]</b> 然后输入或映射该文件所关联项目的负责团队的ID，选择该项目，然后选择该文件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大注释数。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 发布评论]

此操作模块将评论发布到Figma文件。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL文件ID]</td>
      <td>
        <p>输入或映射要将评论发布到的文件的文件ID。 </p>
        <ul>
          <li>
            <p>如果您不知道文件的ID，请单击 <b>[!UICONTROL查找文件]</b> 然后输入或映射与文件关联的项目ID，然后选择该文件。</p>
          </li>
          <li>
            <p>如果您尝试查找文件的ID，但不知道项目的ID，请单击 <b>[!UICONTROL查找项目]</b> 并输入或映射该文件所关联项目的负责团队的ID。 选择项目，然后选择文件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL注释]</td>
      <td>输入评论的文本。</td>
    </tr>
  </tbody>
</table>


### 项目和文件

* [获取文件或图像](#get-a-file-or-image)

* [列出文件版本历史记录](#list-file-version-history)

* [列出项目文件](#list-project-files)

* [列出项目](#list-projects)


#### [!UICONTROL 获取文件或图像]

此操作模块从图像库中检索单个文件或图像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL对象类型]</td>
      <td>
        <p>选择要检索的对象类型。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL文件]</b>
            </p>
            <p>该模块将[!UICONTROL Key]引用的文档作为JSON对象返回。 可以从任何Figma文件URL中解析文件键。</p>
            <p>有关字段，请参阅 <a href="#Get2" class="MCXref xref" >[!UICONTROL获取文件或图像：文件]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL文件节点]</b>
            </p>
            <p>作为JSON对象返回ID引用的节点。 节点将从 [!DNL Figma] [!UICONTROL密钥]引用的文件。</p>
            <p>有关字段，请参阅 <a href="#Get3" class="MCXref xref" >[!UICONTROL获取文件或图像：文件节点]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL图像]</b>
            </p>
            <p>模块从文件中呈现图像。</p>
            <p>有关字段，请参阅 <a href="#Get4" class="MCXref xref" >[!UICONTROL获取文件或图像：图像]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL图像填充]</b>
            </p>
            <p>该模块返回文档中图像填充中存在的所有图像的下载链接。 图像填充是如何 [!DNL Figma] 表示用户提供的任何图像。 将图像拖入 [!DNL Figma], [!DNL Figma] 使用表示图像的单个填充创建一个矩形，并且用户能够转换该矩形（以及填充上的属性）。</p>
            <p>有关字段，请参阅 <a href="#Get5" class="MCXref xref" >[!UICONTROL获取文件或图像：图像填充]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL 获取文件或图像：文件]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL文件密钥]</td>
      <td>选择要从中返回JSON的文件。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL版本ID]</td>
      <td>输入或映射您希望模块返回的文件版本。 对于当前模块，将此字段留空。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL节点ID]</td>
      <td>
        <p>要仅返回文档的子集，请输入您希望模块返回的节点。 模块会返回列出的节点、其子节点，以及根节点和列出的节点之间的任何内容。</p>
        <p>对于要返回的每个节点，单击 <b>[!UICONTROL Add]</b> 并输入节点的文本。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL深度]</td>
      <td>
        <p>输入或映射一个整数，该整数表示要在文档树中返回结果的深度。 </p>
        <div class="example"><span class="autonumber"><span><b>示例: </b></span></span>
          <ul>
            <li>
              <p>要仅返回页面，请输入 <code>1</code>.</p>
            </li>
            <li>
              <p>要返回页面和顶级对象，请输入 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>要返回所有节点，请将此字段留空。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL几何]</td>
      <td>要返回矢量数据，请输入 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL插件数据]</td>
      <td>插件ID和/或字符串“[!UICONTROL shared]”的逗号分隔列表。 由这些插件编写的文档中存在的任何数据都将包含在 <code>pluginData</code> 和 <code>sharedPluginData</code> 属性。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL分支数据]</td>
      <td>启用此选项可返回请求的文件的分支元数据。 如果文件是分支，则主文件的键将包含在返回的响应中。 如果文件具有分支，则其元数据将包含在返回的响应中。 默认: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL 获取文件或图像：文件节点]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL文件密钥]</td>
      <td>选择要从中返回JSON的文件。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL节点ID]</td>
      <td>
        <p>输入您希望模块返回和转换的节点</p>
        <p>对于要返回的每个节点，单击 <b>[!UICONTROL Add]</b> 并输入节点的文本。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL版本ID]</td>
      <td>输入或映射您希望模块返回的文件版本。 对于当前模块，将此字段留空。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL深度]</td>
      <td>
        <p>输入或映射一个整数，该整数表示要在文档树中返回结果的深度。 </p>
        <div class="example"><span class="autonumber"><span><b>示例: </b></span></span>
          <ul>
            <li>
              <p>要仅返回页面，请输入 <code>1</code>.</p>
            </li>
            <li>
              <p>要返回页面和顶级对象，请输入 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>要返回所有节点，请将此字段留空。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL几何]</td>
      <td>要返回矢量数据，请输入 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL插件数据]</td>
      <td>插件ID和/或字符串“shared”的逗号分隔列表。 这些插件编写的文档中存在的任何数据都将包含在pluginData和sharedPluginData属性的结果中。</td>
    </tr>
  </tbody>
</table>


##### 获取文件或图像：图像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL文件密钥]</td>
      <td>选择要从中返回JSON的文件。</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>节点ID]</td>
      <td>
        <p>输入您希望模块呈现的节点。</p>
        <p>对于要渲染的每个节点，单击 <b>[!UICONTROL Add]</b> 并输入节点的文本。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Scale]</td>
      <td>要缩放图像，请输入或映射缩放因子。 此数字必须介于0.01到4之间。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Format]</td>
      <td>
        <p>选择图像输出的格式。</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROLSVG — 包含ID]</td>
      <td>启用此选项可包含所有SVG元素的ID属性。 默认：[!UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROLSVG — 简化描边]</td>
      <td>启用此选项可简化内部/外部描边，并尽可能使用描边属性，而不是 &lt;mask&gt;. 默认：[!UICONTROL true]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL使用绝对范围]</td>
      <td>启用此选项，无论是否裁剪了节点或其周围的空间为空，都可使用节点的完整尺寸。 使用此选项可导出文本节点，而无需裁剪。 默认：[!UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL版本ID]</td>
      <td>输入或映射您希望模块返回的文件版本。 对于当前模块，将此字段留空。</td>
    </tr>
  </tbody>
</table>

##### 获取文件或图像：图像填充

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL文件密钥]</td>
      <td>选择要从中返回JSON的文件。</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL 列出文件版本历史记录]

此搜索模块会返回 [!UICONTROL Figma].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL文件ID]</td>
      <td>
        <p>输入或映射要检索其版本历史记录的文件的文件ID。 </p>
        <ul>
          <li>
            <p>如果您不知道文件的ID，请单击 <b>[!UICONTROL查找文件]</b> 然后输入或映射与文件关联的项目ID，然后选择该文件。</p>
          </li>
          <li>
            <p>如果您尝试查找文件的ID，但不知道项目的ID，请单击 <b>[!UICONTROL查找项目]</b> 并输入或映射该文件所关联项目的负责团队的ID。 选择项目，然后选择文件。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出项目文件]

此搜索模块会返回指定项目中所有文件的列表。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL文件ID]</td>
      <td>
        <p>输入或映射要检索其文件的项目ID。 </p>
        <ul>
          <li>
            <p>如果您不知道项目的ID，请单击 <b>[!UICONTROL查找项目]</b> 然后输入或映射与项目关联的团队的ID，然后选择项目。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出项目]

此搜索模块会返回指定团队中所有项目的列表。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL团队ID]</td>
      <td>输入或映射要为其检索文件的项目ID。 团队ID可在Figma团队页面的URL中找到</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL限制]</td>
      <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td>
    </tr>
  </tbody>
</table>


### 组件和样式

#### [!UICONTROL 获取样式或组件]

此操作模块可检索单个样式或组件，或一组样式或组件。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL对象&gt;键]</td>
      <td>输入要检索的对象的键值（唯一标识符）。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL团队ID]</td>
      <td>输入或映射与记录关联的团队的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL页面大小]</td>
      <td>输入或映射每页返回的数字或结果。 默认：30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>输入或映射开始检索结果后的结果数。 这可以与[!UICONTROL Page Size]字段结合使用，以对结果进行分页。</p>
        <p>此值与对象ID不对应。</p>
        <p>此字段不能与[!UICONTROL Before]字段结合使用。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>输入或映射开始检索结果之前的结果数。 这可以与[!UICONTROL Page Size]字段结合使用，以对结果进行分页。</p>
        <p>此值与对象ID不对应。</p>
        <p>此字段不能与[!UICONTROL After]字段结合使用。</p>
      </td>
    </tr>
  </tbody>
</table>


### 其他

* [进行API调用](#make-an-api-call)

* [观看事件](#watch-events)


#### [!UICONTROL 进行API调用]

此操作模块允许您对Figma API进行经过身份验证的自定义调用，而无需考虑通过身份验证。 这样，您就可以创建数据流自动化，而其他Figma模块无法完成该操作。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
      <td> <p>有关连接 [!DNL Figma] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建连接 [!DNL Adobe Workfront Fusion]  — 基本说明。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>输入相对于 <code>https://api.figma.com/v1/</code>.</p>
        <p>例如： <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL方法]</td>
      <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL标头]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 为您添加授权标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL查询字符串]</td>
      <td>
        <p>以标准JSON对象的形式添加API调用的查询。</p>
        <p>例如： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL主体]</td>
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 观看事件]

当您的团队中的特定团队发生以下事件之一时，此触发器模块会启动一个方案 [!DNL Figma] 团队空间

* 文件更新

* 文件版本更新

* 文件删除

* 库发布

* 文件注释

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>选择模块监视的WebHook。</p>
        <p>要添加新网页挂接，请执行以下操作：</p>
        <ol>
          <li value="1">
            <p>单击 <b>[!UICONTROL Add]</b> [!UICONTROL Webhook]字段旁边。</p>
          </li>
          <li value="2">
            <p>选择要用于此WebHook的连接。 有关连接 [!DNL Figma] 帐户[!UICONTROL Workfront Fusion]，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与[!UICONTROL Adobe Workfront Fusion]的连接 — 基本说明。</a></p>
          </li>
          <li value="3">
            <p>选择您希望模块监视的事件类型。</p>
          </li>
          <li value="4">
            <p>输入您希望Webhook监视其事件的团队的ID。</p>
          </li>
          <li value="5">
            <p>输入您希望Webhook可监视的事件的[!UICONTROL Status]或[!UICONTROL Description]。</p>
          </li>
          <li value="6">
            <p>单击 <b>[!UICONTROL Save]</b> 保存webhook并返回到模块。</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
