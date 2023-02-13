---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP模块
description: 的 [!DNL Adobe Workfront Fusion SFTP] 利用模块，可监视选定文件夹/子文件夹中的文件更改、将新文件上传到所需文件夹、修改或删除文件夹中已存在的现有文件，或更改文件权限。
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# SFTP模块

的 [!DNL Adobe Workfront Fusion] SFTP模块允许您监视选定文件夹/子文件夹中的文件更改、将新文件上传到所需文件夹、修改或删除文件夹中已有的现有文件，或更改文件权限。

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

要将SFTP与 [!DNL Workfront Fusion]，则需要具有SFTP帐户(例如 [!DNL GoDaddy] Web托管)。

## 将SFTP连接到 [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

将您的SFTP帐户连接到 [!DNL Workfront Fusion] 您需要在模块中输入目标主机和SFTP凭据（用户名和密码或用户名和密钥） [!UICONTROL 创建连接] 对话框。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接名称]</td> 
   <td> <p> 输入SFTP连接的名称。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL主机]</p> </td> 
   <td> <p>输入要连接的SFTP服务器的主机名。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL端口] </td> 
   <td> <p>输入SFTP服务器端口。 例如，22。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Auth类型]</p> </td> 
   <td> <p>选择要用于连接到SFTP服务器的授权方法。</p> 
    <ul> 
     <li><strong>[!UICONTROL用户名和密码]</strong>:输入您的凭据。</li> 
     <li> <p><strong>[!UICONTROL用户名和密钥]</strong>:输入您的用户名和私钥/证书</p> <p>如果要使用自签名证书的TLS，请上传私钥以使用客户端授权，或上传您的证书（P12或PFX文件）。 如果您使用的是客户端证书授权，则可以在此处输入您的CA证书。</p> <p>[!DNL Workfront Fusion] 不会保留或存储您在此处提供的任何数据（文件、密码）。 文件和密码仅用于提取私钥/证书。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

输入连接信息后，单击 **[!UICONTROL 继续]** 建立连接。

## [!UICONTROL SFTP] 模块及其字段

配置 [!UICONTROL SFTP] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!UICONTROL SFTP] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### 触发器

#### [!UICONTROL 文件夹中的监视文件]

在指定的文件夹中创建或更改文件时，返回包含详细信息的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>输入或映射要监视的文件夹。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>缓冲区大小[B]</td> 
   <td> <p> 输入缓冲区大小（以字节为单位）。 值定义从服务器传输的块的大小。 当值过高时，某些服务器可能会导致问题或损坏文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回文件的最大数量]</td> 
   <td> <p> 设置文件的最大数量 [!DNL Workfront Fusion] 在一个周期内可用</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 文件夹中的监视子文件夹]

在指定的文件夹中创建或更改文件夹时，返回包含详细信息的文件夹。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td> 
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>输入或映射要监视的文件夹。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回文件的最大数量]</td> 
   <td> <p> 设置文件夹的最大数量 [!DNL Workfront Fusion] 将在一个周期中返回。</p> </td> 
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
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>选择是要检索文件、文件夹，还是同时检索两者。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>输入或映射包含要列出的文件或文件夹的文件夹。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>输入或映射搜索词。 例如，如果要搜索文件扩展名为.txt的文件，请输入 <code>.txt</code>。您还可以输入或映射要搜索的文件的名称。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序依据]</td> 
   <td> <p> 选择要按文件名、大小、上次访问日期还是上次修改日期对结果进行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序顺序] </td> 
   <td> <p>选择结果应按升序还是降序返回。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL即使模块未返回任何结果，仍继续执行路由]</p> </td> 
   <td>启用此选项可确保此模块在未返回任何结果时不会停止方案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回结果的最大数]</td> 
   <td> <p> 设置 [!DNL Workfront Fusion] 将在一个周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此模块会列出指定文件夹中的文件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL缓冲区大小[B]]</td> 
   <td> <p> 输入缓冲区大小（以字节为单位）。 值定义从服务器传输的块的大小。 当值过高时，某些服务器可能会导致问题或损坏文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>输入或映射包含要列出的文件或文件夹的文件夹。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL搜索] </td> 
   <td> <p>输入或映射搜索词。 例如，如果要搜索文件扩展名为.txt的文件，请输入 <code>.txt</code>。您还可以输入或映射要搜索的文件的名称。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序依据]</td> 
   <td> <p> 选择要按文件名、大小、上次访问日期还是上次修改日期对结果进行排序。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL排序顺序]</td> 
   <td> <p> 选择结果应按升序还是降序返回。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL即使模块未返回任何结果，仍继续执行路由]</p> </td> 
   <td>启用此选项可确保此模块在未返回任何结果时不会停止方案。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL返回结果的最大数]</td> 
   <td> <p> 设置文件的最大数量 [!DNL Workfront Fusion] 将在一个周期中返回。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 获取文件]

此模块可检索文件详细信息，包括文件的数据。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL缓冲区大小[B]]</td> 
   <td> <p> 输入缓冲区大小（以字节为单位）。 值定义从服务器传输的块的大小。 当值过高时，某些服务器可能会导致问题或损坏文件。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件路径] </td> 
   <td> <p>输入文件的路径。 您可以指定绝对路径，例如 <code>/home/user/file.txt</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此模块允许您将文件上传到SFTP服务器。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>指定现有文件夹作为文件的存储位置。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL源文件]</td> 
   <td> <p> 映射来自前一模块的源文件，如[!UICONTROLDropbox] &gt; [!UICONTROL获取文件]。 您还可以输入或映射文件名和文件数据。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL权限]</p> </td> 
   <td> <p>为文件或文件夹设置所需的权限。 使用chmod参数。 例如： <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>有关chmod的更多详细信息，请参阅 <a href="https://ss64.com/bash/chmod.html">chmod文档</a>.</p> </td> 
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
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件路径]</td> 
   <td> <p> 输入要重命名的文件的路径。 您可以指定绝对路径，例如 <code>/home/user/file.txt</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL新文件名]</td> 
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
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件路径]</td> 
   <td> <p> 输入要移动的文件的路径。 您可以指定绝对路径，例如 <code>/home/user/file.txt</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New Folder]</td> 
   <td> <p> 输入文件新位置的路径。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件路径]</td> 
   <td> <p> 输入要删除的文件的路径。 您可以指定绝对路径，例如 <code>/home/user/file.txt</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新文件权限]

用于更改文件的权限。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件路径]</td> 
   <td> <p> 输入要移动的文件的路径。 您可以指定绝对路径，例如 <code>/home/user/file.txt</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL权限]</p> </td> 
   <td> <p>设置所需的文件权限。 使用chmod参数。 例如， <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>必须匹配模式 <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>有关chmod的更多详细信息，请参阅 <a href="https://ss64.com/bash/chmod.html">chmod文档</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 创建文件夹]

在指定位置创建新文件夹。

>[!NOTE]
>
>如果文件夹已存在，则模块将引发错误。 要不中断地继续流，请将错误处理程序路由附加到模块以捕获错误并使用 [!UICONTROL 恢复] 指令继续流程。 有关附加错误处理程序路由的信息，请参阅 [在中处理错误 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). 有关错误处理程序路由的信息，请参阅 [中错误处理的指令 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹] </td> 
   <td> <p>指定现有文件夹作为新文件夹的存储位置。 您可以指定绝对路径，例如 <code>/home/user/file.txt</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL文件夹名称]</td> 
   <td> <p> 输入文件夹名称。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL权限]</p> </td> 
   <td> <p>设置所需的文件夹权限。 使用chmod参数。 例如， <code>777 </code>或 <code>-rwxrwxrwx</code>.</p> <p>必须匹配模式 <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>有关chmod的更多详细信息，请参阅 <a href="https://ss64.com/bash/chmod.html">chmod手册页</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除文件夹]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL连接] </td>
   <td> <p>有关将SFTP帐户连接到 [!DNL Workfront Fusion]，请参阅 <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">将SFTP连接到 [!DNL Workfront Fusion]</a> 在本文中。</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> 指定要删除的文件夹的路径。 您可以指定绝对路径，例如 <code>/home/user/</code>. 或者，您也可以指定指向已登录用户的特定文件夹的相对路径，例如 <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
