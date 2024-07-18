---
title: CloudConvert模块
description: CloudConvert模块
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3008'
ht-degree: 0%

---

# [!DNL CloudConvert]模块

在Adobe Workfront Fusion场景中，您可以自动使用CloudConvert的工作流，并将其连接到多个第三方应用程序和服务。 [!DNL CloudConvert]模块允许您监视和管理[!DNL CloudConvert]帐户中的作业、任务以及导入和导出文件。

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

## 将[!DNL CloudConvert]连接到[!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

若要将您的[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]，您需要从您的[!DNL CloudConvert]帐户获取API密钥。

1. 登录到您的[!DNL CloudConvert]帐户并打开您的[!UICONTROL 仪表板]。
1. 打开&#x200B;**[!UICONTROL 授权] > [!UICONTROL API密钥]**&#x200B;部分。
1. 单击&#x200B;**[!UICONTROL 创建新API密钥]**。
1. 输入API密钥的名称，启用要使用的范围，然后单击&#x200B;**[!UICONTROL 创建]**。
1. 复制提供的令牌并将其存储在安全位置。
1. 在[!DNL Workfront Fusion]中，开始创建方案并打开[!DNL CloudConvert]模块的&#x200B;**[!UICONTROL 创建连接]**&#x200B;对话框。

   有关说明，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md)中创建方案。

1. 输入您在步骤5中保存的令牌，然后单击&#x200B;**[!UICONTROL 继续]**&#x200B;以建立连接。

## [!DNL CloudConvert]模块及其字段 {#cloudconvert-modules-and-their-fields}

配置[!DNL CloudConvert]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL CloudConvert]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [常见任务](#common-tasks)
* [个作业](#jobs)
* [任务](#tasks)
* [其他](#other)

### 常见任务

* [捕获网站](#capture-a-website)
* [[!UICONTROL 转换文件]](#convert-a-file)
* [创建存档](#create-an-archive)
* [合并文件](#merge-files)
* [优化文件](#optimize-a-file)

#### [!UICONTROL 捕获网站]

此操作模块可捕获指定的网站并将其保存为PDF、JPG或PNG格式。

您可以指定网站的URL和其他信息，例如要将信息存储在何处。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td>输入要捕获的网站的URL。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式] </td> 
   <td>选择您希望以PNG、JPG还是PDF格式保存捕获的网站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名] </td> 
   <td>为目标输出文件输入文件名（包括扩展名）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers] </td> 
   <td> <p>（可选）定义请求标头。 </p> <p>这很有用，例如，当指定的URL需要授权时。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL转换和特定于引擎的选项] </p> </td> 
   <td>指定转化和特定于引擎的选项。 要查看可用选项，请参阅有关<code>input_format</code>和<code>output_format</code>的<a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a>文档。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下载文件] </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入文件]</td> 
   <td>选择是要使用[!DNL Workfront Fusion]上载文件，还是提供将从中上载文件的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上传文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL从URL导入文件]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[！UICONTROL URL]</strong> </p> <p>输入要转换的文件的URL。</p> </li> 
     <li> <p><strong>[！UICONTROL Headers]</strong></p> <p>定义请求标头（可选）。 这很有用，例如，当指定的URL需要授权时。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL格式]</td> 
   <td>选择是否要指定要转换的文件的输入格式。 如果未指定，则使用输入文件的扩展名作为输入格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>选择文件的当前格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td>选择要将文件转换到的目标文件格式。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td>选择目标输出文件的文件名（包括扩展名）。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[！UICONTROL转换和特定于引擎的选项] </p> </td> 
   <td>指定转化和特定于引擎的选项。 要查看可用选项，请参阅有关<code>input_format</code>和<code>output_format</code>的<a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a>文档。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[！UICONTROL下载文件] </td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建存档]

使您能够将一个或多个文件添加到ZIP、RAR、7Z、TAR、TAR.GZ或TAR.BZ2存档中。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输入文件]</p> </td> 
   <td> <p>指定要添加到存档中的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上传文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL从URL导入文件]</p> </td> 
   <td> <p><strong>[！UICONTROL URL]</strong> </p> <p>输入要存档的文件的URL。</p> <p><strong>[！UICONTROL标头]</strong> </p> <p>定义请求标头（可选）。 这很有用，例如，当指定的URL需要授权时。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td> <p> 选择存档文件的目标格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td> <p> 输入目标输出文件的文件名（包括扩展名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL转换和特定于引擎的选项] </td> 
   <td> <p>指定转化和特定于引擎的选项。 要查看可用选项，请参阅有关<code>input_format</code>和<code>output_format</code>的<a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a>文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下载文件]</td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 合并文件]

至少将两个文件合并到一个PDF中。 如果输入文件不是PDF，则它们会自动转换为PDF。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL输入文件]</p> </td> 
   <td> <p>指定要合并的文件。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上传文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL从URL导入文件]</p> </td> 
   <td> <p><strong>[！UICONTROL URL]</strong> </p> <p>输入要存档的文件的URL。</p> <p><strong>[！UICONTROL标头]</strong> </p> <p>定义请求标头（可选）。 这很有用，例如，当指定的URL需要授权时。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式]</td> 
   <td> <p> 选择合并文件的目标格式。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td> <p> 输入目标输出文件的文件名（包括扩展名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL转换和特定于引擎的选项] </td> 
   <td> <p>指定转化和特定于引擎的选项。 要查看可用选项，请参阅有关<code>input_format</code>和<code>output_format</code>的<a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a>文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下载文件]</td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 优化文件]

该操作模块可优化和压缩PDF、PNG或JPG格式的文件。

指定文件以及用于优化和存储文件的参数。

模块会返回文件的ID和任何关联字段，以及连接访问的任何自定义字段和值。 您可以在场景的后续模块中映射此信息。

配置此模块时，会显示以下字段。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入文件]</td> 
   <td>选择是要使用Workfront Fusion上载文件，还是提供用于上载文件的URL。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL上传文件]</p> </td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL从URL导入文件] </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL URL]</strong>：输入要转换的文件的URL。</li> 
     <li><strong>[！UICONTROL标头]</strong>： （可选）定义请求标头。 这很有用，例如，当指定的URL需要授权时。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Optimization for] </td> 
   <td> <p>为特定目标需求选择优化配置文件。</p> 
    <ul> 
     <li> <p><strong>[！UICONTROL Web]</strong>：针对Web进行优化（默认）</p> 
      <ul> 
       <li>为Web删除冗余和不必要的数据</li> 
       <li>缩减像素采样、剪辑和智能压缩图像</li> 
       <li>合并字体和子集字体</li> 
       <li>将颜色转换为RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL打印]</strong>：优化打印</p> 
      <ul> 
       <li> <p>删除冗余和不必要的打印数据</p> </li> 
       <li> <p>缩减像素采样、剪辑和智能压缩图像</p> </li> 
       <li> <p>合并字体和子集字体</p> </li> 
       <li> <p>将颜色转换为CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL存档]</strong>：针对存档目的进行优化</p> 
      <ul> 
       <li> <p>删除冗余和不必要的数据以进行存档</p> </li> 
       <li> <p>智能压缩图像</p> </li> 
       <li> <p>合并字体和子集字体</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL扫描的图像]</strong>：优化扫描的图像</p> 
      <ul> 
       <li> <p>为主要包含光栅图像的PDF优化的配置文件</p> </li> 
       <li> <p>在不显着降低视觉质量的情况下压缩图像</p> </li> 
      </ul> </li> 
     <li> <p><strong>[！UICONTROL最大尺寸缩减]</strong>：针对最大尺寸缩减进行优化</p> 
      <ul> 
       <li> <p>使用最大可能的压缩</p> </li> 
       <li> <p>可能会降低视觉质量</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入格式] </td> 
   <td>选择要优化的输入文件格式。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件名]</td> 
   <td> <p>为目标输出文件输入文件名（包括扩展名）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL转换和特定于引擎的选项]</td> 
   <td> <p>指定转化和特定于引擎的选项。 要查看可用选项，请参阅有关<code>input_format</code>和<code>output_format</code>的<a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a>文档。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL下载文件]</td> 
   <td> <p>如果还希望在模块的输出中包含文件数据，则启用此选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 任务

* [[!UICONTROL 创建作业（高级）]](#create-a-job-advanced)
* [[!UICONTROL 新作业事件]](#new-job-event)
* [[!UICONTROL 列出作业]](#list-jobs)
* [[!UICONTROL 获取作业]](#get-a-job)
* [[!UICONTROL 删除作业]](#delete-a-job)

#### [!UICONTROL 创建作业（高级）]

此模块将创建一个作业。 作业可以是[!UICONTROL 名称]字段中标识并使用[!UICONTROL 输入]字段相互链接的一个或多个任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输入文件]</td> 
   <td> <p>选择是要使用[!DNL Workfront Fusion]上载文件，还是提供上载文件的URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL上传文件]</td> 
   <td> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL从URL导入文件]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[！UICONTROL URL]</strong>：输入要处理的文件的URL。</li> 
     <li><strong>[！UICONTROL标头]</strong>： （可选）定义请求标头。 这很有用，例如，当指定的URL需要授权时。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL任务]</p> </td> 
   <td> <p>添加将在作业中执行的任务。</p> <p>请在相应的部分中找到操作字段的说明。</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[！UICONTROL转换文件]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[！UICONTROL捕获网站]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[！UICONTROL优化文件]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[！UICONTROL创建存档]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[！UICONTROL合并文件]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[！UICONTROL执行命令]</strong> </p> <p>有关执行命令的详细信息，请参阅<a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] API文档</a>。</p> </li> 
     <li> <p><strong>[！UICONTROL将文件导出到临时URL]</strong> </p> <p> 指定任务名称和输入任务名称（例如，转换）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标记] </td> 
   <td> <p>输入标记。 标记是用于标识作业的任意字符串。 它们没有任何效果，可用于将作业与ID相关联。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除作业]

此模块会删除作业，包括所有任务和数据。

>[!NOTE]
>
>作业在结束的24小时后自动删除。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL作业ID]</td> 
   <td> <p>输入或映射要删除的作业的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取作业]

此模块可检索作业详细信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL作业ID]</td> 
   <td> <p>输入或映射要检索其详细信息的作业的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出作业]

此模块可检索已在您的帐户中运行的所有作业。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL状态] </td> 
   <td> <p>选择作业状态，以筛选返回的作业。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>设置Workfront Fusion 2.0在一个执行周期中返回的作业数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新作业事件]

在帐户或任务中的作业创建、完成或失败时触发。

>[!NOTE]
>
>* 由[!UICONTROL 创建作业（高级）]模块创建的作业包含&#x200B;*多个*&#x200B;任务。
>* 创建、完成或失败的&#x200B;*单个*&#x200B;任务时，也会触发[!UICONTROL 新作业事件]触发器。
>

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称]</td> 
   <td>输入webhook名称。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL输出格式] </td> 
   <td>选择您希望以PNG、JPG还是PDF格式保存捕获的网站。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL事件]</td> 
   <td>选择在创建、完成或失败作业或任务时是否触发该模块。</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 如果使用数组聚合器（例如，您有许多不同格式的文件要转换），请使用[!UICONTROL 添加任务]对话框中的&#x200B;**[!UICONTROL 我不知道输入格式]**&#x200B;选项。 否则，将返回错误。
>* 链接作业中的任务（名称>输入，名称>输入，...）：
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### 任务

* [[!UICONTROL 获取任务]](#get-a-task)
* [[!UICONTROL 下载文件]](#download-a-file)
* [[!UICONTROL 列出任务]](#list-tasks)
* [[!UICONTROL 重试任务]](#retry-a-task)
* [[!UICONTROL 取消任务]](#cancel-a-task)
* [[!UICONTROL 删除任务]](#delete-a-task)

#### [!UICONTROL 取消任务]

此模块可取消处于等待或处理状态的任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任务ID]</td> 
   <td> <p> 输入或映射要取消的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除任务]

删除任务，包括所有数据。

>[!NOTE]
>
>任务结束后24小时后会自动删除。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任务ID]</td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任务ID]</td> 
   <td> <p> 输入或映射要从中下载文件的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取任务]

此模块可检索任务详细信息。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任务ID]</td> 
   <td> <p>输入或映射要检索其详细信息的任务的ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 列出任务]

此模块根据筛选器设置检索您帐户中的所有任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL状态] </td> 
   <td> <p>选择任务状态以作为返回任务筛选依据。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL作业ID] </td> 
   <td> <p>输入或映射作业ID以仅返回指定作业内的任务。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作] </td> 
   <td> <p>输入工序类型以仅返回具有指定工序的任务。 </p> <p>注意：使用[！UICONTROL List Possible Operations]模块检索操作。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td> <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重试任务]

此模块根据其他任务的设置（有效负荷）创建新任务。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL任务ID]</td> 
   <td> <p> 输入或映射要从中创建新任务的任务ID。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL CloudConvert]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">将[!DNL CloudConvert]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[Fusion App]帐户连接到Workfront Fusion的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe Workfront Fusion的连接 — 基本说明</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL URL]</td> 
   <td> <p>输入相对于<code>https://api.cloudconvert.com/</code>的路径。 例如： <code>/v2/tasks</code></p> <p>有关可用端点的列表，请参阅<a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] API v2文档</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL方法]</td> 
   td&gt; <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Body]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**示例：**&#x200B;列表任务

以下API调用返回您CloudFront帐户中的所有任务：

URL： `/v2/tasks`

方法： `GET`

![](assets/cloudconvert-api-example-input.png)

在[!UICONTROL 包] > [!UICONTROL 正文] > [!UICONTROL 数据]下的模块输出中可以找到搜索匹配项。

在我们的示例中，返回了6个任务：

![](assets/cloudconvert-api-example-output.png)

## 故障排除 {#troubleshooting}

请参阅下表以了解可能出现的错误及其解决方案：

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
   <td role="rowheader"> <p><span style="font-weight: normal;">[！UICONTROL输出文件大小超出方案所允许的限制。]</span> </p> </td> 
   <td> <p>请参阅文件大小限制。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[！UICONTROL您已超过最大转化时间。]</span> </p> </td> 
   <td> <p>免费的[!DNL CloudConvert]计划每天提供25分钟的转化时间。 如果您的使用情况超过了免费计划的限制，则可以切换到（预付）程序包或订阅。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[！UICONTROL无法读取帧大小：无法搜寻到1508。 /output/JLIADSA00137P0.mp3�：参数无效。]</span> </p> </td> 
   <td> <p>例如，将文件从MP3转换为WAV时会引发此错误。 请确保选择了正确的区域，因为它将查找文件的引用，而不仅仅是正确文件的引用。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL RuntimeError：] </p> <p><span style="font-weight: normal;">[！UICONTROL超出最大重复数。]</span> </p> </td> 
   <td> <p>在[!DNL CloudConvert]仪表板的作业列表中找到相应的[!DNL CloudConvert]作业，并检查该作业的持续时间：</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>[!DNL CloudConvert] &gt; [！UICONTROL Convert a File]模块的超时设置为3分钟。 如果作业持续时间超过3分钟（可能由于[!DNL CloudConvert]服务临时过载），则模块会引发上述错误。</p> <p>在这种情况下，请考虑以下选项之一：</p> 
    <ul> 
     <li>在场景设置中启用<strong>[！UICONTROL允许存储未完成的执行]</strong>选项以存储未完成的执行，以供以后手动解析。 或者，您可以附加一个错误处理路由到[!DNL CloudConvert]模块，并使用[！UICONTROL Break]指令自动解决未完成的执行。</li> 
     <li>禁用[!DNL CloudConvert] &gt; [！UICONTROL转换文件]模块中的<strong>[！UICONTROL下载文件]选项</strong>。 在这种情况下，模块将不会等待转换结果。 要获得转换结果，请创建一个新方案并使用[!DNL CloudConvert] &gt; [！UICONTROL新建作业事件]触发器。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## [!DNL CloudConvert]连接器的工作流示例

>[!INFO]
>
>**示例：**&#x200B;将视频从MOV转换为MP4格式
>
>1. 访问[https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. 单击&#x200B;**[!UICONTROL 选择文件]**&#x200B;并选择您的示例MOV文件。
>1. 单击&#x200B;**[!UICONTROL 转换为]**&#x200B;旁边的下拉菜单并选择&#x200B;**[!UICONTROL MP4]**。
>
>1. 单击&#x200B;**[!UICONTROL 扳手]**&#x200B;图标。
>1. 根据需要配置MP4压缩设置。
>1. 单击&#x200B;**[!UICONTROL 转换]**。
>1. 转换完成后，单击&#x200B;**[!UICONTROL 下载]**。
>1. 查看转换后的视频。
>1. 重复步骤1至8，直到找到步骤5的最佳转化设置。
>1. 访问[https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. 为&#x200B;**[!UICONTROL input_format]**&#x200B;字段选择&#x200B;**[!UICONTROL mov]**。
>
>1. 为&#x200B;**[!UICONTROL output_format]**&#x200B;字段选择&#x200B;**[!UICONTROL mp4]**。
>
>1. 所有可能参数（如video_codec、crf等）的列表。 将会出现。
>1. 在Workfront Fusion 2.0中，在您的方案中插入&#x200B;**[!UICONTROL CloudConvert]** > **[!UICONTROL 转换文件]**&#x200B;模块。
>
>1. 打开模块的设置。
>1. 按如下所示配置模块：
>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. 确保在“转换和引擎特定选项”字段中包括所有设置：对于步骤5中的每个设置，请找到步骤13中的相应参数及其相应值。
