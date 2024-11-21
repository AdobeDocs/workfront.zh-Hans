---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets模块
description: 使用 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] 帐户的 [!DNL Adobe Experience Manager Assets] 连接器，创建、上传和更新资产，以及复制或移动文件夹和资产。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1724'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets]模块

使用[!DNL Adobe Workfront Fusion]的[!DNL Adobe Experience Manager Assets]连接器，您可以基于[!DNL Adobe Experience Manager Assets]帐户中的事件启动方案，创建、上传和更新资产，以及复制或移动文件夹和资产。

有关Adobe Experience Manager Assets连接器的介绍，请参阅：

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

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

* 您必须拥有[!DNL Adobe Experience Manager Assets]帐户才能使用这些模块。
* 必须在[!DNL Adobe Developer console]中设置[!UICONTROL 服务器到服务器]流。

  有关在[!DNL Adobe Developer console]中设置[!UICONTROL 服务器到服务器]流的说明，请参阅[为服务器端API生成访问令牌](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow)。
* 您的Adobe Experience Manager技术帐户必须具有写入权限。

  有关向Adobe Experience Manager技术帐户添加写入权限的说明，请参阅Adobe Experience Manager文档中的[服务凭据](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)。

## Adobe Experience Manager Assets API信息

Adobe Experience Manager Assets连接器使用以下对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v1.8.61</td> 
  </tr>
 </tbody> 
 </table>

## 将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

要为您的[!DNL Adobe Experience Manager Assets]模块创建连接：

1. 单击[!UICONTROL 连接]框旁边的[!UICONTROL 添加]。

2. 选择正在创建的连接类型：

   * **[!DNL AEM Assets as a Cloud Service]**

     此配置需要来自[!DNL Adobe Admin Console]的信息。

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     此配置需要用户名和密码。

3. 填写要创建的连接类型的字段。

   对于[!DNL AEM Assets as a Cloud Service]，请参阅[配置 [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service)的连接。

   有关[!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services])，请参阅[配置[!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic)的连接。

4. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;保存连接并返回模块。


### 为[!DNL AEM Assets as a Cloud Service]配置连接

>[!NOTE]
>
>* 这些字段的信息是作为在[!DNL Adobe Developer Console]上设置[!UICONTROL 服务器到服务器]流的一部分生成的。 您可以在作为该设置的一部分生成的服务凭据JSON文件中找到这些值。
>
>   有关在[!UICONTROL Adobe Developer Console]上设置[!UICONTROL 服务器到服务器]流的说明，请参阅[为服务器端API生成访问令牌](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow)。
>
>* 您的Adobe Experience Manager技术帐户必须具有写入权限。
>
>   有关向Adobe Experience Manager技术帐户添加写入权限的说明，请参阅Adobe Experience Manager文档中的[服务凭据](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials)。


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[！UICONTROL连接名称]</td>
                  <td>
                      <p>输入此连接的名称</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL实例URL，不带尾随斜杠]</td>
                  <td>输入[!DNL Adobe Experience Manager]实例的URL。 不要在URL末尾包含斜杠<code>/</code>。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL帐户详细信息填充选项]</td>
                  <td>选择是要提供描述帐户详细信息的JSON，还是要手动输入详细信息。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL JSON格式的技术帐户详细信息]</td>
                  <td>如果提供JSON，请输入或粘贴描述您帐户详细信息的JSON。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL客户端ID]</td>
                  <td>如果手动输入详细信息，请输入在[！UICONTROL服务器到服务器]设置中生成的客户端ID。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL客户端密钥]</td>
                  <td>如果手动输入详细信息，请输入在[！UICONTROL服务器到服务器]设置中生成的客户端密钥。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL技术帐户ID]</td>
                  <td>如果手动输入详细信息，请输入技术帐户的ID。 这是客户端凭据JSON文件中的“[！UICONTROL id]”字段。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL组织ID]</td>
                  <td class="">如果人工输入详细信息，请输入组织的ID。 这是客户端凭据JSON文件中的“[！UICONTROL org]”字段。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL元范围]</td>
                  <td>输入在[！UICONTROL服务器到服务器]设置中生成的元范围。</td>
              </tr>
              <tr>
                  <td role="rowheader">[！UICONTROL私钥]</td>
                  <td>输入在[！UICONTROL服务器到服务器]安装程序中生成的私钥。 要提取私钥，请单击[！UICONTROL提取]，然后输入要提取的文件和文件的密码。</td>
              </tr>
          </tbody>
      </table>


### 配置[!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])的连接

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[！UICONTROL连接名称]</td>
                <td>
                    <p>输入此连接的名称</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL实例URL，不带尾随斜杠]</td>
                <td>输入[!DNL Adobe Experience Manager]实例的URL。 不要在URL末尾包含斜杠<code>/</code>。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL用户名]</td>
                <td>输入此连接使用的[!DNL AEM Assets]帐户的用户名。</td>
            </tr>
            <tr>
                <td role="rowheader">[！UICONTROL密码]</td>
                <td>输入此连接使用的[!DNL AEM Assets]帐户的密码。</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets]模块及其字段

配置[!DNL Adobe Experience Manager Essentials]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Adobe Experience Manager Essentials]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

![](assets/map-toggle-350x74.png)

* [复制文件夹或资源](#copy-a-folder-or-asset)
* [创建记录](#create-a-record)
* [删除文件夹、资源或演绎版](#delete-a-folder-asset-or-rendition)
* [获取文件夹列表](#get-a-folder-listing)
* [进行自定义API调用](#make-a-custom-api-call)
* [移动文件夹或资源](#move-a-folder-or-asset)
* [更新记录](#update-a-record)
* [上传资源](#upload-an-asset)

### [!UICONTROL 复制文件夹或资产]

此操作模块会将文件夹或资产复制到Adobe Experience Manager Assets帐户中的其他位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您要复制文件夹还是资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹] / [！UICONTROL资产选择]</td> 
   <td>选择或映射要复制的文件夹或资源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目标路径]</td> 
   <td>选择路径，或将路径映射到新文件夹或资源的位置。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">已复制文件夹的[！UICONTROL名称] / [！UICONTROL资产]</td> 
   <td>输入新文件夹或资源的名称。 在[!DNL Adobe Experience Manager Assets]中显示的文件夹名称与原始名称相同。 此处输入的名称将显示在新文件夹或资产的URL中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL复制子项]</td> 
   <td>启用此选项以复制文件夹中的任何子文件夹或资源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL覆盖]</td> 
   <td>启用此选项以覆盖目标位置中与要复制的文件夹或资源同名的任意文件夹或资源。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 创建记录]

此操作模块可创建文件夹或资产评论。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL对象类型]</td> 
   <td> <p>选择想要创建文件夹还是要在资源上创建评论。</p> 
    <ul> 
     <li> <p>[！UICONTROL文件夹]</p> <p>填写以下字段：</p> 
      <ul> 
       <li> <p>[！UICONTROL名称]</p> <p>输入文件夹的名称。 此名称将显示在文件路径中，因此不得包含空格或其他字符。 </p> </li> 
       <li> <p>[！UICONTROL标题]</p> <p>输入文件夹的标题，该标题可以显示而不是名称。</p> </li> 
      </ul> </li> 
     <li> <p>[！UICONTROL资产注释]</p> <p>填写以下字段：</p> 
      <ul> 
       <li> <p>[！UICONTROL资源选择]</p> <p>选择或映射您要为其添加评论的资产ID。</p> </li> 
       <li> <p>[！UICONTROL Comment]</p> <p>输入注释的文本。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 删除文件夹、资源或演绎版]

此操作模块可删除文件夹、资源或演绎版。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您要删除文件夹、资源还是演绎版。</p> 
    <ul> 
     <li> <p>[！UICONTROL文件夹]</p> <p>通过选择路径中的文件夹来选择要删除的文件夹。</p> </li> 
     <li> <p>[！UICONTROL资产] </p> <p>选择资源的方法是选择其路径中的文件夹，然后选择要删除的资源。</p> </li> 
     <li> <p>[！UICONTROL演绎版]</p> <p>通过选择格式副本路径中的文件夹来选择格式副本。</p> <p>输入或映射演绎版的名称。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 获取文件夹列表]

此操作模块检索现有文件夹及其子实体（文件夹或资产）的表示形式。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹]</td> 
   <td>选择或映射要检索的文件夹。 要将子文件夹添加到路径中，请单击加号图标并选择子文件夹。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 进行自定义API调用]

此操作模块对[!DNL Adobe Experience Manager Assets] API进行自定义API调用。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对于您的[!DNL Adobe Experience Manager]基本URL的路径。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP请求方法。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Headers]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串] </td> 
   <td> <p>输入请求查询字符串。 对于每个键/值对，单击<b>[！UICONTROL添加项]</b>并输入[！UICONTROL键]和[！UICONTROL值]。</p> </td> 
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

### [!UICONTROL 移动文件夹或资源]

此操作模块会将给定路径下的资产或文件夹移动到新位置。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您要移动文件夹还是资产。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL文件夹] / [！UICONTROL资产]</td> 
   <td>选择或映射要移动的文件夹或资源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目标路径]</td> 
   <td>选择路径，或将路径映射到要将文件夹或资源移动到的位置。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">已移动文件夹的[！UICONTROL名称] / [！UICONTROL资产]</td> 
   <td>为移动的文件夹或资源输入新名称。 在[!DNL Adobe Experience Manager Assets]中显示的文件夹名称与原始名称相同。 此处输入的名称将显示在移动的文件夹或资产的URL中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL覆盖]</td> 
   <td>启用此选项以覆盖目标位置中与要复制的文件夹或资源同名的任意文件夹或资源。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 更新记录]

此操作模块更新现有记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择您要删除资源元数据还是资源演绎版。</p> 
    <ul> 
     <li> <p>[！UICONTROL资产元数据]</p> 
      <ul> 
       <li> <p>选择要为其更新元数据的资源。</p> </li> 
       <li> <p>输入资源的新标题。</p> </li> 
      </ul> </li> 
     <li> <p>[！UICONTROL资产演绎版]</p> 
      <ul> 
       <li> <p>选择要为其更新演绎版的资源。</p> </li> 
       <li> <p>从上一个模块中选择源文件，或映射源文件的名称和数据。</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 上传资产]

此操作模块会将资产上传到您的[!DNL Adobe Experience Manager Assets]帐户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关将[!DNL Adobe Experience Manager Assets]帐户连接到[!DNL Workfront Fusion]的说明，请参阅本文中的<a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">将[!DNL Adobe Experience Manager Assets]连接到[!DNL Workfront Fusion]</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL目标]</td> 
   <td> <p>选择要上传资源的文件夹。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Source file]</td> 
   <td>输入或映射源文件的名称和数据。</td> 
  </tr> 
 </tbody> 
</table>
