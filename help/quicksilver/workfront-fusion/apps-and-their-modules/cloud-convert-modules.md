---
title: CloudConvert模块
description: CloudConvert模块
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2993'
ht-degree: 0%

---

# [!DNL CloudConvert] 模块

在Adobe Workfront Fusion方案中，您可以自动执行使用CloudConvert的工作流，并将其连接到多个第三方应用程序和服务。 的 [!DNL CloudConvert] 模块允许您监视和管理作业、任务，以及导入和导出文件 [!DNL CloudConvert] 帐户。

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

## 连接 [!DNL CloudConvert] to [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，您需要从 [!DNL CloudConvert] 帐户。

1. 登录到 [!DNL CloudConvert] 帐户，打开 [!UICONTROL 功能板].
1. 打开 **[!UICONTROL 授权] > [!UICONTROL API密钥]** 中。
1. 单击 **[!UICONTROL 创建新API密钥]**.
1. 输入API密钥的名称，启用要使用的作用域，然后单击 **[!UICONTROL 创建]**.
1. 复制提供的令牌并将其存储在安全位置。
1. 在 [!DNL Workfront Fusion]，开始创建方案并打开 [!DNL CloudConvert] 模块 **[!UICONTROL 创建连接]** 对话框。

   有关说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 输入您在步骤5中保存的令牌，然后单击 **[!UICONTROL 继续]** 建立连接。

## [!DNL CloudConvert] 模块及其字段 {#cloudconvert-modules-and-their-fields}

配置 [!DNL CloudConvert] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL CloudConvert] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [常见任务](#common-tasks)
* [任务](#jobs)
* [任务](#tasks)
* [其他](#other)

### 常见任务

* [捕获网站](#capture-a-website)
* [[!UICONTROL 转换文件]](#convert-a-file)
* [创建存档](#create-an-archive)
* [合并文件](#merge-files)
* [优化文件](#optimize-a-file)

#### [!UICONTROL 捕获网站]

此操作模块会捕获指定的网站，并将其保存为PDF、JPG或PNG格式。

您可以指定网站的URL和其他信息，例如您希望将信息存储到的位置。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入要捕获的网站的URL。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式] </td> 
   <td>选择是要以PNG、JPG还是PDF格式保存捕获的网站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名] </td> 
   <td>输入目标输出文件的文件名（包括扩展名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头] </td> 
   <td> <p>（可选）定义请求标头。 </p> <p>这非常有用，例如，当指定的URL需要授权时。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL转化和引擎特定选项] </p> </td> 
   <td>指定转化和引擎特定选项。 要查看可用选项，请参阅 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 文档 <code>input_format</code> 和 <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下载文件] </td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 转换文件]

将文件转换为选定的输出格式。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件]</td> 
   <td>选择是否要使用 [!DNL Workfront Fusion] 或者提供将从中上传文件的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上传文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL从URL导入文件]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>输入要转换的文件的URL。</p> </li> 
     <li> <p><strong>[!UICONTROL标头]</strong></p> <p>定义请求标头（可选）。 这非常有用，例如，当指定的URL需要授权时。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Format]</td> 
   <td>选择是否要指定要转换的文件的输入格式。 如果未指定，则使用输入文件的扩展名作为输入格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>选择文件的当前格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL输出格式]</td> 
   <td>选择要将文件转换为的目标文件格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td>为目标输出文件选择文件名（包括扩展名）。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL转化和引擎特定选项] </p> </td> 
   <td>指定转化和引擎特定选项。 要查看可用选项，请参阅 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 文档 <code>input_format</code> 和 <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL下载文件] </td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建存档]

允许您向ZIP、RAR、7Z、TAR、TAR.GZ或TAR.BZ2存档添加一个或多个文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL输入文件]</p> </td> 
   <td> <p>指定要添加到存档的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上传文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL从URL导入文件]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>输入要存档的文件的URL。</p> <p><strong>[!UICONTROL标头]</strong> </p> <p>定义请求标头（可选）。 这非常有用，例如，当指定的URL需要授权时。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式]</td> 
   <td> <p> 选择存档文件的目标格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td> <p> 输入目标输出文件的文件名（包括扩展名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL转化和引擎特定选项] </td> 
   <td> <p>指定转化和引擎特定选项。 要查看可用选项，请参阅 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 文档 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下载文件]</td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 合并文件]

将至少两个文件合并到一个PDF中。 如果输入文件不是PDF，则会自动将它们转换为PDF。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL输入文件]</p> </td> 
   <td> <p>指定要合并的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上传文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL从URL导入文件]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>输入要存档的文件的URL。</p> <p><strong>[!UICONTROL标头]</strong> </p> <p>定义请求标头（可选）。 这非常有用，例如，当指定的URL需要授权时。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式]</td> 
   <td> <p> 选择合并文件的目标格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td> <p> 输入目标输出文件的文件名（包括扩展名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL转化和引擎特定选项] </td> 
   <td> <p>指定转化和引擎特定选项。 要查看可用选项，请参阅 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 文档 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下载文件]</td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 优化文件]

此操作模块会优化和压缩PDF、PNG或JPG格式的文件。

您可以指定文件以及用于优化和存储该文件的参数。

模块会返回文件的ID和任何关联的字段，以及连接访问的任何自定义字段和值。 您可以在方案的后续模块中映射此信息。

配置此模块时，将显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件]</td> 
   <td>选择您是要使用Workfront Fusion上传文件，还是提供将从中上传文件的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL上传文件]</p> </td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL从URL导入文件] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>:输入要转换的文件的URL。</li> 
     <li><strong>[!UICONTROL标头]</strong>:（可选）定义请求标头。 这非常有用，例如，当指定的URL需要授权时。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optimization for] </td> 
   <td> <p>根据特定目标需求选择优化配置文件。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong>:Web优化（默认）</p> 
      <ul> 
       <li>为Web删除冗余和不必要的数据</li> 
       <li>对图像进行下采样、剪辑和智能压缩</li> 
       <li>合并和子集化字体</li> 
       <li>将颜色转换为RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Print]</strong>:打印优化</p> 
      <ul> 
       <li> <p>删除用于打印的冗余和不必要的数据</p> </li> 
       <li> <p>对图像进行下采样、剪辑和智能压缩</p> </li> 
       <li> <p>合并和子集化字体</p> </li> 
       <li> <p>将颜色转换为CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL存档]</strong>:针对归档目的进行优化</p> 
      <ul> 
       <li> <p>为归档删除冗余和不必要的数据</p> </li> 
       <li> <p>智能地压缩图像</p> </li> 
       <li> <p>合并和子集化字体</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL扫描的图像]</strong>:优化扫描的图像</p> 
      <ul> 
       <li> <p>针对主要由光栅图像组成的PDF优化的配置文件</p> </li> 
       <li> <p>压缩图像，而不会显着降低视觉质量</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL最大尺寸缩减]</strong>:最大尺寸减小的优化</p> 
      <ul> 
       <li> <p>使用最大可能的压缩</p> </li> 
       <li> <p>可能会降低视觉质量</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入格式] </td> 
   <td>选择要优化的输入文件的格式。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL文件名]</td> 
   <td> <p>输入目标输出文件的文件名（包括扩展名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL转化和引擎特定选项]</td> 
   <td> <p>指定转化和引擎特定选项。 要查看可用选项，请参阅 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> 文档 <code>input_format</code> 和 <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL下载文件]</td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 任务

* [[!UICONTROL 创建作业（高级）]](#create-a-job-advanced)
* [[!UICONTROL 新建作业事件]](#new-job-event)
* [[!UICONTROL 列表作业]](#list-jobs)
* [[!UICONTROL 找工作]](#get-a-job)
* [[!UICONTROL 删除作业]](#delete-a-job)

#### [!UICONTROL 创建作业（高级）]

此模块会创建一个作业。 作业可以是在 [!UICONTROL 名称] 字段并使用 [!UICONTROL 输入] 字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输入文件]</td> 
   <td> <p>选择是否要使用 [!DNL Workfront Fusion]，或提供将从中上传文件的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL上传文件]</td> 
   <td> <p>从前一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL从URL导入文件]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>:输入要处理的文件的URL。</li> 
     <li><strong>[!UICONTROL标头]</strong>:（可选）定义请求标头。 这非常有用，例如，当指定的URL需要授权时。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL任务]</p> </td> 
   <td> <p>添加将在作业中执行的任务。</p> <p>有关操作字段的说明，请参阅相应章节。</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL转换文件]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL捕获网站]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL优化文件]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL创建存档]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL合并文件]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL执行命令]</strong> </p> <p>有关执行命令的更多信息，请参阅 <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] API文档</a>.</p> </li> 
     <li> <p><strong>[!UICONTROL将文件导出到临时URL]</strong> </p> <p> 指定任务名称和输入任务名称（例如，转化）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标记] </td> 
   <td> <p>输入标记。 标记是用于标识作业的任意字符串。 它们没有任何效果，可用于将作业与ID关联。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除作业]

此模块会删除作业，包括所有任务和数据。

>[!NOTE]
>
>作业结束后24小时自动删除。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作业ID]</td> 
   <td> <p>输入或映射要删除的作业的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 找工作]

此模块检索作业详细信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作业ID]</td> 
   <td> <p>输入或映射要检索有关详细信息的作业的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表作业]

此模块可检索您的帐户中已运行的所有作业。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL状态] </td> 
   <td> <p>选择作业状态以筛选返回的作业。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>设置在一个执行周期中返回的Workfront Fusion 2.0作业数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新建作业事件]

在帐户或任务中创建、完成或失败的作业时触发。

>[!NOTE]
>
>* 由 [!UICONTROL 创建作业（高级）] 模块由 *多个* 任务。
>* 的 [!UICONTROL 新建作业事件] 触发器还会在 *个人* 任务已创建、已完成或失败。
>


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td>输入Webhook名称。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL输出格式] </td> 
   <td>选择是要以PNG、JPG还是PDF格式保存捕获的网站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event]</td> 
   <td>选择是在创建、完成还是失败作业或任务时触发模块。</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 如果使用阵列聚合器（例如，您有许多不同格式的文件要转换），请使用 **[!UICONTROL 我不知道输入格式]** 选项 [!UICONTROL 添加任务] 对话框。 否则，返回错误。
>* 正在链接作业中的任务（名称>输入、名称>输入……）：
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### 任务

* [[!UICONTROL 获取任务]](#get-a-task)
* [[!UICONTROL 下载文件]](#download-a-file)
* [[!UICONTROL 列表任务]](#list-tasks)
* [[!UICONTROL 重试任务]](#retry-a-task)
* [[!UICONTROL 取消任务]](#cancel-a-task)
* [[!UICONTROL 删除任务]](#delete-a-task)

#### [!UICONTROL 取消任务]

此模块会取消具有等待或处理状态的任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任务ID]</td> 
   <td> <p> 输入或映射要取消的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除任务]

删除任务，包括所有数据。

>[!NOTE]
>
>任务结束后24小时，系统会自动删除这些任务。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任务ID]</td> 
   <td> <p> 输入（映射）要删除的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下载文件]

此模块从指定任务中检索文件名和文件数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任务ID]</td> 
   <td> <p> 输入或映射要从中下载文件的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取任务]

此模块检索任务详细信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任务ID]</td> 
   <td> <p>输入或映射要检索相关详细信息的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列表任务]

此模块会根据过滤器设置检索帐户中的所有任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL状态] </td> 
   <td> <p>选择任务状态以筛选返回的任务。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL作业ID] </td> 
   <td> <p>输入或映射作业ID以仅返回指定作业内的任务。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL操作] </td> 
   <td> <p>输入操作类型，以便仅返回具有指定操作的任务。 </p> <p>注意：使用[!UICONTROL List Possible Operations]模块检索操作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重试任务]

此模块会根据其他任务的设置（负载）创建新任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL任务ID]</td> 
   <td> <p> 输入或映射要从中创建新任务的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 其他

* [[!UICONTROL 获取我的信息]](#get-my-info)
* [[!UICONTROL 进行API调用]](#make-an-api-call)

#### [!UICONTROL 获取我的信息]

检索有关当前用户的经过身份验证的帐户详细信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关连接 [!DNL CloudConvert] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">连接 [!DNL CloudConvert] to [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行API调用]

允许您执行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td> <p>有关将[Fusion App]帐户连接到Workfront Fusion的说明，请参阅 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>输入相对于 <code>https://api.cloudconvert.com/</code>. 例如： <code>/v2/tasks</code></p> <p>有关可用端点的列表，请参阅 <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] API v2文档</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。使用条件语句(例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：** 列表任务

以下API调用会从您的CloudFront帐户返回所有任务：

URL: `/v2/tasks`

方法: `GET`

![](assets/cloudconvert-api-example-input.png)

搜索的匹配项可在模块的输出下找到 [!UICONTROL 捆绑] > [!UICONTROL 正文] > [!UICONTROL 数据].

在本例中，返回了6项任务：

![](assets/cloudconvert-api-example-output.png)

## 疑难解答 {#troubleshooting}

请参阅下表，了解可能出现的错误及其解决方案：

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>错误</p> </th> 
   <th>下面的步骤</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL输出文件大小超过了您的方案允许的限制。]</span> </p> </td> 
   <td> <p>请参阅文件大小限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL您已超过最大转化时间。]</span> </p> </td> 
   <td> <p>免费 [!DNL CloudConvert] 计划每天提供25分钟的转换。 如果您的使用超出了免费计划的限制，您可以切换到（预付）包或订阅。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL读取帧大小失败：无法寻找1508。 �/output/JLIADSA00137P0.mp3:参数无效。]</span> </p> </td> 
   <td> <p>例如，在将文件从MP3转换为WAV时，会引发此错误。 确保选择了正确的区域，因为它将找到对文件的引用，而不仅仅是正确的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL RuntimeError:] </p> <p><span style="font-weight: normal;">[!UICONTROL超出的最大重复次数。]</span> </p> </td> 
   <td> <p>找到对应的 [!DNL CloudConvert] 您的工作 [!DNL CloudConvert] 功能板的作业列表并检查作业的持续时间：</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>的 [!DNL CloudConvert] &gt; [!UICONTROL转换文件]模块的超时设置为3分钟。 如果作业的持续时间超过3分钟(可能是由于 [!DNL CloudConvert] 服务)时，模块会引发上述错误。</p> <p>在这种情况下，请考虑以下选项之一：</p> 
    <ul> 
     <li>启用 <strong>[!UICONTROL允许存储不完整的执行]</strong> 选项来存储未完成的执行，以便日后手动解决。 （可选）您可以将错误处理路由附加到 [!DNL CloudConvert] 具有[!UICONTROL Break]指令的模块，可自动解决未完成的执行。</li> 
     <li>禁用 <strong>[!UICONTROL下载文件]选项</strong> 在 [!DNL CloudConvert] &gt; [!UICONTROL转换文件]模块。 在这种情况下，模块将不会等待转换结果。 要获取转化结果，请创建新方案并使用 [!DNL CloudConvert] &gt; [!UICONTROL New Job Event]触发器。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 工作流示例 [!DNL CloudConvert] 连接器

>[!INFO]
>
>**示例：** 将视频从MOV转换为MP4格式
>
>1. 访问 [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. 单击 **[!UICONTROL 选择文件]** 并选择示例MOV文件。
>1. 单击旁边的下拉菜单 **[!UICONTROL 转换为]** 选择 **[!UICONTROL MP4]**.
>
>1. 单击 **[!UICONTROL 扳手]** 图标。
>1. 根据需要配置MP4压缩设置。
>1. 单击 **[!UICONTROL 转换]**.
>1. 转化完成后，单击 **[!UICONTROL 下载]**.
>1. 查看转换后的视频。
>1. 重复步骤1至8，直到找到步骤5的最佳转化设置。
>1. 访问 [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. 选择 **[!UICONTROL mov]** 对于 **[!UICONTROL input_format]** 字段。
>
>1. 选择 **[!UICONTROL mp4]** 对于 **[!UICONTROL output_format]** 字段。
>
>1. 所有可能的参数（如video_codec、crf等）的列表。 中。
>1. 在Workfront Fusion 2.0中，插入 **[!UICONTROL CloudConvert]** > **[!UICONTROL 转换文件]** 模块。
>
>1. 打开模块的设置。
>1. 配置模块，如下所示：

>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. 确保在“转化”和“引擎特定选项”字段中包含所有设置：对于步骤5中的每个设置，从步骤13中找到相应的参数及其相应值。

