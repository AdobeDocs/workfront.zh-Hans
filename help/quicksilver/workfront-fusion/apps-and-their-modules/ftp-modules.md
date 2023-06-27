---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP模块
description: FTP模块允许您监视选定文件夹中的文件更改，将新文件上传到所需文件夹，以及修改或删除文件夹中已有的现有文件。
author: Becky
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1343'
ht-degree: 0%

---

# FTP模块

FTP模块允许您监视选定文件夹中的文件更改，将新文件上传到所需文件夹，以及修改或删除文件夹中已有的现有文件。

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

要使用 [Fusion应用程序] 替换为 [!DNL Workfront Fusion]，您必须拥有FTP帐户。

## 在FTP模块中创建连接 {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接名称]</td> 
   <td> <p> 输入FTP连接的名称。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL主机] </td> 
   <td> <p>输入FTP服务器主机名。 E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL端口] </td> 
   <td> <p>输入FTP服务器端口号。 E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL用户名] </td> 
   <td> <p>输入您的FTP帐户用户名。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL密码] </td> 
   <td> <p>输入您的FTP帐户密码。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>使用安全连接(TLS)</p> </td> 
   <td> <p>选择是否要使用安全连接。</p> <p style="font-weight: bold;">[！UICONTROL否]</p> <p>连接不安全。</p> <p style="font-weight: bold;">[！UICONTROL显式加密或隐式加密]</p> <p>使用SSL保护连接。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL拒绝未经授权的证书]</p> </td> 
   <td> <p>启用此选项以验证FTP服务器证书。 如果验证失败，则不会创建连接。 要通过验证，证书必须满足以下条件之一：</p> 
    <ul> 
     <li>由根用户签名 <a href="https://en.wikipedia.org/wiki/Certificate_authority">证书颁发机构</a></li> 
     <li>由中间认证机构签名(参见 <a href="https://knowledge.digicert.com/solution/SO16297.html">证书链的工作方式</a> 以取得进一步说明)。 在这种情况下，所有中间证书都应安装在FTP服务器上。</li> 
     <li>是[！UICONTROL Self-signed certificate]字段中提供的自签名证书（见下文）</li> </ul>

如果禁用此选项，则不会验证FTP服务器证书。 我们强烈建议不要禁用此选项，因为它会导致连接不安全，并带来严重的安全风险。</td>
</tr> 
  <tr> 
   <td> <p>[！UICONTROL自签名证书]</p> </td> 
   <td> <p>单击 <b>[！UICONTROL Extract]</b> 按钮打开上传对话框。</p> <p>上载证书以将TLS与您的自签名证书一起使用。 [!DNL Workfront Fusion] 不会保留或存储您提供的任何数据，例如文件和密码。 文件和密码仅用于提取证书。</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP模块及其字段

* [触发器](#triggers)
* [操作](#actions)

### 触发器

#### [!UICONTROL 关注文件]

[!UICONTROL 关注文件] 是FTP的唯一触发器模块。 它监视所选文件夹的文件内容。 将新文件插入到指定文件夹时，将执行触发器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关建立与FTP帐户的连接的说明，请参阅 <a href="#create-a-connection" class="MCXref xref">在FTP模块中[！UICONTROL创建连接]</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL文件夹]</p> </td> 
   <td> <p>选择要监视的文件夹。</p> <p><b>注意：</b> 每个方案只允许一个文件夹。 子文件夹将被忽略。</p> <p><b>提示：</b> 要跟踪多个文件夹，请为每个文件夹创建一个独立的方案。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回文件的最大数目] </td> 
   <td> <p>设置满足以下条件的最大结果数 [!DNL Workfront Fusion] 在一个周期内使用。 如果该值设置得过高，则可能会中断给定第三方服务端的连接（超时）。 [!DNL Workfront Fusion] 对此没有任何影响。 我们建议您设置较低的值，并为最大循环数定义较高的值，或者更频繁地运行该方案。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 更改权限]](#change-permissions)
* [[!UICONTROL 创建文件夹]](#create-a-folder)
* [[!UICONTROL 删除文件]](#delete-a-file)
* [[!UICONTROL 删除文件夹]](#delete-a-folder)
* [[!UICONTROL 获取文件]](#get-a-file)
* [[!UICONTROL 文件夹中的文件列表]](#list-of-files-in-a-folder)
* [[!UICONTROL 移动文件或文件夹]](#move-a-file-or-folder)
* [[!UICONTROL 上传] 文件](#upload-a-file)

#### [!UICONTROL 更改权限]

此操作模块更改文件或文件夹的权限设置。

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[！UICONTROL连接]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">有关建立与FTP帐户的连接的说明，请参阅 <a href="#Create" class="MCXref xref" >在FTP模块中[！UICONTROL创建连接]</a> 本文章中。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[！UICONTROL更改权限设置]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>选择是否要更改文件或文件夹的设置。</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[！UICONTROL文件路径]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">输入或映射文件路径到文件夹或文件。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[！UICONTROL Permissions]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>设置所需的文件或文件夹权限。 使用chmod参数。 例如： <code>777 </code>或 <code>-rwxrwxrwx</code>.</p>
               <p>权限必须匹配模式 <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 创建文件夹]

此操作模块将创建新文件夹。

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[！UICONTROL连接]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">有关建立与FTP帐户的连接的说明，请参阅 <a href="#Create" class="MCXref xref" >在FTP模块中[！UICONTROL创建连接]</a> 本文章中。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[！UICONTROL文件夹路径]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">输入或映射文件路径到新文件夹。</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[！UICONTROL新文件夹名称]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>输入或映射新文件夹的名称。</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 删除文件]

从指定的文件夹中删除文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">有关建立与FTP帐户的连接的说明，请参阅 <a href="#Create" class="MCXref xref" >在FTP模块中[！UICONTROL创建连接]</a> 本文章中。</td>
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要从中删除文件的FTP文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件名]</td> 
   <td> <p> 输入文件名，包括文件扩展名。 示例: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件夹]

此操作模块将永久删除指定的文件夹。

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[！UICONTROL连接]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">有关建立与FTP帐户的连接的说明，请参阅 <a href="#Create" class="MCXref xref" >在FTP模块中[！UICONTROL创建连接]</a> 本文章中。</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[！UICONTROL文件夹]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>选择要从中删除文件的FTP文件夹。</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL 获取文件]

从FTP服务器检索可进一步处理的文件，例如上传到 [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关建立与FTP帐户的连接的说明，请参阅 <a href="#creating-the-ftp-connection" class="MCXref xref">创建FTP连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件路径]</td> 
   <td> <p> 输入要获取的文件的路径。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文件夹中的文件列表]

检索文件和/或文件夹信息。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td> <p>有关建立与FTP帐户的连接的说明，请参阅 <a href="#creating-the-ftp-connection" class="MCXref xref">创建FTP连接</a> 本文章中。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要搜索的FTP文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Show] </td> 
   <td> <p>选择是要检索有关文件或文件夹的信息，还是要检索这两者。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索] </td> 
   <td> <p>输入搜索词。 如果未输入搜索词，则将检索指定文件夹中的所有文件和文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回文件的最大数目]</td> 
   <td> <p> 设置此模块检索的文件的最大数目。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动文件或文件夹]

此操作模块会将文件或文件夹移动到其他位置。

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[！UICONTROL连接]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">有关建立与FTP帐户的连接的说明，请参阅 <a href="#Create" class="MCXref xref" >在FTP模块中[！UICONTROL创建连接]</a> 本文章中。</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[！UICONTROL旧文件路径]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>输入要从中移动文件的路径。 示例: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[！UICONTROL新文件路径]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>输入要将该文件移动到的路径。 示例: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL 上传文件]

将文件上传到FTP服务器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL连接] </td> 
   <td>有关建立与FTP帐户的连接的说明，请参阅 <a href="#creating-the-ftp-connection" class="MCXref xref">创建FTP连接</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>选择要将文件上传到的FTP文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL源文件] </td> 
   <td> <p>从上一个模块中选择一个源文件，或映射源文件的名称和数据。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL附加到现有文件]</td> 
   <td> <p>如果启用了此选项，并且FTP服务器上已存在文件，则文件的内容将附加到现有文件。 如果未启用此选项，则将覆盖文件的内容。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL创建文件夹（如果不存在）] </td> 
   <td> <p>如果启用了此选项，并且FTP服务器上不存在您输入到“文件夹”字段的文件夹，则模块将创建该文件夹</p> </td> 
  </tr> 
 </tbody> 
</table>

## 故障排除 {#troubleshooting}

如果在创建连接期间或模块操作期间FTP应用程序遇到问题，请尝试使用某个常用FTP客户端，并尝试执行相同的操作（例如，创建连接或在文件夹中列出文件）。 FTP客户端。 如果您也遇到与FTP客户端相同的问题，原因可能是FTP服务器的配置错误。
