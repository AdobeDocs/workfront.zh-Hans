---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP模块
description: 使用 [!DNL Adobe Workfront Fusion SFTP] 模块可以监视所选文件夹/子文件夹中的文件更改，将新文件上传到所需文件夹，修改或删除文件夹中已存在的文件，或者更改文件权限。
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1920'
ht-degree: 0%

---

# SFTP模块

[!DNL Adobe Workfront Fusion] SFTP模块允许您监视选定文件夹/子文件夹中的文件更改，将新文件上传到所需的文件夹，修改或删除文件夹中已存在的文件，或者更改文件权限。

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

要将SFTP与[!DNL Workfront Fusion]一起使用，需要具有SFTP帐户（如[!DNL GoDaddy] Web托管）。

## 将SFTP连接到[!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

要将SFTP帐户连接到[!DNL Workfront Fusion]，您需要输入目标主机以及模块[!UICONTROL 创建连接]对话框的SFTP凭据（用户名和密码或用户名和密钥）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接名称]</td> 
   <td> <p> 输入SFTP连接的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL主机]</p> </td> 
   <td> <p>输入要连接的SFTP服务器的主机名。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL端口] </td> 
   <td> <p>输入SFTP服务器端口。 例如，22。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL身份验证类型]</p> </td> 
   <td> <p>选择要用于连接到SFTP服务器的授权方法。</p> 
    <ul> 
     <li><strong>[！UICONTROL用户名和密码]</strong>：输入您的凭据。</li> 
     <li> <p><strong>[！UICONTROL用户名和密钥]</strong>：输入您的用户名和私钥/证书</p> <p>如果要使用自签名证书的TLS，请上载私钥以使用客户端授权，或上载证书（P12或PFX文件）。 如果您使用的是客户端证书授权，可以在此处输入您的CA证书。</p> <p>[!DNL Workfront Fusion] 不保留或存储您在此处提供的任何数据（文件、密码）。 文件和密码仅用于提取私钥/证书。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

输入连接信息后，单击&#x200B;**[!UICONTROL 继续]**&#x200B;建立连接。

## [!UICONTROL SFTP]模块及其字段

配置[!UICONTROL SFTP]模块时，[!DNL Workfront Fusion]显示以下列出的字段。 此外，可能还会显示其他[!UICONTROL SFTP]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

### 触发器

#### [!UICONTROL 监视文件夹中的文件]

在指定文件夹中创建或更改文件时，返回包含详细信息的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>输入或映射要监视的文件夹。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>缓冲区大小[B]</td> 
   <td> <p> 输入缓冲区大小（字节）。 该值定义从服务器传送的块的大小。 当值过高时，某些服务器可能会导致问题或文件损坏。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回的最大文件数]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内处理的最大文件数</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 监视文件夹中的子文件夹]

在指定文件夹中创建或更改文件夹时，返回包含详细信息的文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td> 
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>输入或映射要监视的文件夹。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回的最大文件数]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内返回的最大文件夹数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

#### [!UICONTROL 列出文件夹的内容]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Show] </td> 
   <td> <p>选择是要检索文件、文件夹还是两者。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>输入或映射包含要列出的文件或文件夹的文件夹。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索] </td> 
   <td> <p>输入或映射搜索词。 例如，如果要搜索文件扩展名为.txt的文件，请输入<code>.txt</code>。您还可以输入或映射要搜索的文件名。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序方式]</td> 
   <td> <p> 选择是否要按文件名、大小、上次访问日期或上次修改日期对结果进行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序顺序] </td> 
   <td> <p>选择应按升序还是降序返回结果。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL即使模块未返回任何结果，仍继续执行路由]</p> </td> 
   <td>启用此选项以确保此模块在未返回任何结果时不会停止方案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回结果的最大数目]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内返回的结果的最大数目。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此模块列出指定文件夹中的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL缓冲区大小[B]]</td> 
   <td> <p> 输入缓冲区大小（字节）。 该值定义从服务器传送的块的大小。 当值过高时，某些服务器可能会导致问题或文件损坏。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>输入或映射包含要列出的文件或文件夹的文件夹。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL搜索] </td> 
   <td> <p>输入或映射搜索词。 例如，如果要搜索文件扩展名为.txt的文件，请输入<code>.txt</code>。您还可以输入或映射要搜索的文件名。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序方式]</td> 
   <td> <p> 选择是否要按文件名、大小、上次访问日期或上次修改日期对结果进行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL排序顺序]</td> 
   <td> <p> 选择应按升序还是降序返回结果。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL即使模块未返回任何结果，仍继续执行路由]</p> </td> 
   <td>启用此选项以确保此模块在未返回任何结果时不会停止方案。</td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL返回结果的最大数目]</td> 
   <td> <p> 设置[!DNL Workfront Fusion]在一个周期内返回的最大文件数。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此模块可检索文件详细信息，包括文件数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL缓冲区大小[B]]</td> 
   <td> <p> 输入缓冲区大小（字节）。 该值定义从服务器传送的块的大小。 当值过高时，某些服务器可能会导致问题或文件损坏。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件路径] </td> 
   <td> <p>输入文件的路径。 您可以指定绝对路径，如<code>/home/user/file.txt</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，如<code>./file.txt</code>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上载文件]

此模块允许您将文件上传到SFTP服务器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>指定现有文件夹作为文件的存储位置。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL Source File]</td> 
   <td> <p> 映射来自前一模块的源文件，如[！UICONTROLDropbox] &gt; [！UICONTROL获取文件]。 您还可以输入或映射文件名和文件数据。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Permissions]</p> </td> 
   <td> <p>为文件或文件夹设置所需的权限。 使用chmod参数。 例如： <code>777 </code>或<code>-rwxrwxrwx</code>。</p> <p>有关chmod的详细信息，请参阅<a href="https://ss64.com/bash/chmod.html">chmod文档</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 重命名文件]

重命名文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件路径]</td> 
   <td> <p> 输入要重命名的文件的路径。 您可以指定绝对路径，如<code>/home/user/file.txt</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，如<code>./file.txt</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新文件名]</td> 
   <td> <p> 输入文件的新名称，包括文件扩展名。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 移动文件]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件路径]</td> 
   <td> <p> 输入要移动文件的路径。 您可以指定绝对路径，如<code>/home/user/file.txt</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，如<code>./file.txt</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL新文件夹]</td> 
   <td> <p> 输入文件新位置的路径。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件路径]</td> 
   <td> <p> 输入要删除的文件的路径。 您可以指定绝对路径，如<code>/home/user/file.txt</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，如<code>./file.txt</code>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新文件权限]

允许您更改文件的权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件路径]</td> 
   <td> <p> 输入要移动文件的路径。 您可以指定绝对路径，如<code>/home/user/file.txt</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，如<code>./file.txt</code>。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Permissions]</p> </td> 
   <td> <p>设置所需的文件权限。 使用chmod参数。 例如，<code>777 </code>或<code>-rwxrwxrwx</code>。</p> <p>必须符合模式 <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>有关chmod的详细信息，请参阅<a href="https://ss64.com/bash/chmod.html">chmod文档</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

在指定位置创建新文件夹。

>[!NOTE]
>
>如果该文件夹已存在，则模块将引发错误。 若要继续流而不中断，请将错误处理程序路由附加到模块以捕获错误，并使用[!UICONTROL Resume]指令继续流。 有关附加错误处理程序路由的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md)中的[错误处理。 有关错误处理程序路由的信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)中用于错误处理的[指令。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹] </td> 
   <td> <p>指定现有文件夹作为新文件夹的存储位置。 您可以指定绝对路径，如<code>/home/user/file.txt</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，如<code>./</code>。</p> </td> 
  </tr> 
  <tr> 
   <td>[！UICONTROL文件夹名称]</td> 
   <td> <p> 输入文件夹名称。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[！UICONTROL Permissions]</p> </td> 
   <td> <p>设置所需的文件夹权限。 使用chmod参数。 例如，<code>777 </code>或<code>-rwxrwxrwx</code>。</p> <p>必须符合模式 <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>有关chmod的详细信息，请参阅<a href="https://ss64.com/bash/chmod.html">chmod手册页</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件夹]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[！UICONTROL Connection] </td>
   <td> <p>有关将SFTP帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> 指定要删除的文件夹的路径。 您可以指定绝对路径，如<code>/home/user/</code>。 或者，您可以指定指向登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
