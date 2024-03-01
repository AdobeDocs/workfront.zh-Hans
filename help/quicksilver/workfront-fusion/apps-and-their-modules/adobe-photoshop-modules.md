---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Photoshop模块
description: 借助Adobe Photoshop模块，您可以根据Adobe Photoshop帐户中的事件启动Adobe Workfront Fusion方案，创建、读取或更新协议和其他记录，使用您设置的标准搜索记录以及上传文档。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: 0ea4ac4c4579d09dafeed47946ae9c7caf906cfe
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 0%

---

# [!DNL Adobe Photoshop] 模块

在 [!DNL Adobe Workfront Fusion] 方案，您可以自动执行使用 [!DNL Adobe Photoshop]，并将其连接到多个第三方应用程序和服务。 [!DNL Adobe Photoshop] 通过模块，您可以创建、读取、更新或删除记录，列出给定类型的所有记录，根据您指定的条件搜索记录，或者对 [!DNL Adobe Photoshop] API。


如果您需要有关创建方案的说明，请参阅 [创建方案](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划*</td>
      <td>
        <p>[！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td>
      <td>
        <p>[！UICONTROL计划]，[！UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td>
      <td >
        <p>[！UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">产品</td>
      <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

&#42;&#42;有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 先决条件

在使用 [!DNL Adobe Photoshop] 连接器时，必须确保满足以下先决条件：

* 您必须拥有有效的 [!DNL Adobe Photoshop] 帐户。

## 创建与的连接 [!DNL Adobe Photoshop]

要为创建连接，请执行以下操作 [!DNL Adobe Photoshop] 模块：

1. 单击 **[!UICONTROL 添加]** ，位于“Connection（连接）”框旁。

1. 填写以下字段：

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[！UICONTROL连接名称]</td>
        <td>
          <p>输入此连接的名称。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL客户端ID]</td>
        <td>输入您的[！UICONTROLAdobe] [！UICONTROL客户端ID]。 可在[！UICONTROL Credentials]的 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL客户端密钥]</td>
        <td>输入您的 [!DNL Adobe] [！UICONTROL客户端密钥]。 可在[！UICONTROL Credentials]的 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL技术帐户ID]</td>
        <td>输入您的 [!DNL Adobe] [！UICONTROL技术帐户ID]。 可在[！UICONTROL Credentials]的 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL组织ID]</td>
        <td>输入您的 [!DNL Adobe] [！UICONTROL组织ID]。 可在[！UICONTROL Credentials]的 [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[！UICONTROL私钥]</td>
        <td>
          <p>输入在中创建凭据时生成的私钥 [!DNL Adobe Developer Console]. </p>
          <p>要提取您的私钥或证书，请执行以下操作：</p>
          <ol>
            <li value="1">
              <p>单击 <b>[！UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>选择要提取的文件类型。</p>
            </li>
            <li value="3">
              <p>选择包含私钥或证书的文件。</p>
            </li>
            <li value="4">
              <p>输入文件的密码。</p>
            </li>
            <li value="5">
              <p>单击 <b>保存</b> 以提取文件并返回到[！UICONTROL ]e连接设置。</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

## [!DNL Adobe Photoshop] 模块及其字段

配置时 [!DNL Adobe Photoshop] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Adobe Photoshop] 字段可能会显示，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### 操作

* [创建新PSD](#create-a-new-psd)
* [编辑文本图层](#edit-text-layers)
* [执行深度模糊](#execute-depth-blur)
* [执行Photoshop操作](#execute-photoshop-actions)
* [执行产品裁切](#execute-product-crop)
* [获取图层信息](#get-layer-info)
* [进行自定义API调用](#make-a-custom-api-call)

#### 创建新PSD

该操作模块会创建一个带有可选层的新PSD，并生成演绎版或另存为PSD。

有关与此模块相关的字段，请参阅 [创建新PSD](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) 请参阅Adobe Photoshop文档中的。

#### 编辑文本图层

此操作模块可编辑Photoshop文件中的文本图层。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Photoshop]，请参见 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >创建与的连接 [!DNL Adobe Photoshop]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入文件存储]</td>
      <td>
        <p>选择存储要编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输入文件URL]</p>
      </td>
   <td> 输入或映射要编辑的文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Manage missing fonts]</td>
      <td>
        <p>选择文档中存在一个或多个缺少的字体时要执行的操作。 如果未提供该字体，模块将使用默认字体。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL默认字体]  </td>
      <td>
        <p>输入要用作文档全局默认字体的完整postscript名称。 此字体将用于缺少字体且没有专门为该图层提供其他字体的任何文本图层。 如果缺少此字体，则在“管理缺少的字体”中指定的选项将生效。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL层]</td>
   <td> <p>有关图层选项的详细信息，请参阅 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">编辑文本图层</a> 请参阅Adobe Photoshop文档。</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输出文件存储]</td>
      <td>
        <p>选择要存储编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件URL]</p>
      </td>
   <td> 输入或映射将存储编辑文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件类型]</p>
      </td>
   <td> 为编辑的文件选择文件类型。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆盖]</td>
      <td>
        <p>选择新编辑的文件是否会覆盖任何已存在的输出文件。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL压缩]</p>
      </td>
   <td> 选择输出文件的压缩级别。 </td> 
    </tr>
  </tbody>
</table>

#### 执行深度模糊

此操作模块对所选文件执行“深度模糊”。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Photoshop]，请参见 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >创建与的连接 [!DNL Adobe Photoshop]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入文件存储]</td>
      <td>
        <p>选择存储要编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输入文件URL]</p>
      </td>
   <td> 输入或映射要编辑的文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输出文件存储]</td>
      <td>
        <p>选择要存储编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件URL]</p>
      </td>
   <td> 输入或映射将存储编辑文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件类型]</p>
      </td>
   <td> 为编辑的文件选择文件类型。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL其他字段]</td>
      <td>
        <p>有关其他“深度模糊”选项的详细信息，请参阅 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">执行深度模糊 </a>在Adobe Photoshop API文档中。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆盖]</td>
      <td>
        <p>选择新编辑的文件是否会覆盖任何已存在的输出文件。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL压缩]</p>
      </td>
   <td> 选择输出文件的压缩级别。 </td> 
    </tr>
  </tbody>
</table>

#### 执行Photoshop操作

此操作模块对所选图像执行Photoshop操作。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Photoshop]，请参见 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >创建与的连接 [!DNL Adobe Photoshop]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入文件存储]</td>
      <td>
        <p>选择存储要编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输入文件URL]</p>
      </td>
   <td> 输入或映射要编辑的文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Actions文件存储]</td>
      <td>
        <p>选择存储操作文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL操作文件URL]</p>
      </td>
   <td> 输入或映射操作文件的URL或路径。 </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL操作名称]</p>
      </td>
   <td> 如果只想执行特定操作，则可以从ActionSet中指定要播放的操作。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL字体/图案/画笔存储]</td>
      <td>
        <p>选择存储要使用的文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL字体/模式/画笔文件URL]</p>
      </td>
   <td> 输入或映射要使用的文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输出文件存储]</td>
      <td>
        <p>选择要存储编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件URL]</p>
      </td>
   <td> 输入或映射将存储编辑文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件类型]</p>
      </td>
   <td> 为编辑的文件选择文件类型。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆盖]</td>
      <td>
        <p>选择新编辑的文件是否会覆盖任何已存在的输出文件。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL压缩]</p>
      </td>
   <td> 选择输出文件的压缩级别。 </td> 
    </tr>
  </tbody>
</table>

#### 执行产品裁切

此操作模块对所选图像执行产品裁切。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Photoshop]，请参见 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >创建与的连接 [!DNL Adobe Photoshop]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入文件存储]</td>
      <td>
        <p>选择存储要裁切文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输入文件URL]</p>
      </td>
   <td> 输入或映射要裁切的文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL单元]</p>
      </td>
   <td> 选择您要以像素还是以百分比描述高度和宽度调整。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL宽度]</p>
      </td>
   <td> 输入或映射要添加宽度边距的量。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL Height]</p>
      </td>
   <td> 输入或映射要添加的高度边距量。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输出文件存储]</td>
      <td>
        <p>选择要存储编辑文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件URL]</p>
      </td>
   <td> 输入或映射将存储编辑文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输出文件类型]</p>
      </td>
   <td> 为编辑的文件选择文件类型。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL覆盖]</td>
      <td>
        <p>选择新编辑的文件是否会覆盖任何已存在的输出文件。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL压缩]</p>
      </td>
   <td> 选择输出文件的压缩级别。 </td> 
    </tr>
  </tbody>
</table>

#### 获取图层信息

此操作模块从指定的PSD文件中检索层信息。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Photoshop]，请参见 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >创建与的连接 [!DNL Adobe Photoshop]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入文件存储]</td>
      <td>
        <p>选择要从中检索层信息的文件的文件服务。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL输入文件URL]</p>
      </td>
   <td> 输入或映射要从中检索图层信息的文件的URL或路径。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL缩略图]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### 进行自定义API调用

此操作模块对Photoshop API进行自定义调用。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Photoshop]，请参见 <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >创建与的连接 [!DNL Adobe Photoshop]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]</td>
      <td>
        <p>输入相对路径 <code>https://image.adobe.io/pie/psdService</code>. 示例： <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加授权标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL查询字符串]  </td>
      <td>
        <p>输入请求查询字符串。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

