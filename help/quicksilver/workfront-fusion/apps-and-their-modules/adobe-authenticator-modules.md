---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Authenticator模块
description: 借助Adobe Authenticator模块，您可以使用单个连接通过API连接到任何Adobe产品。
author: Becky
feature: Workfront Fusion
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 443bdb5caee4b8a7ba9df95b0befff27b7aaabc2
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 1%

---

# Adobe Authenticator模块

Adobe Authenticator模块允许您通过单个连接连接到任何AdobeAPI。 这允许您更轻松地连接到尚未拥有专用Fusion连接器的Adobe产品。

与HTTP模块相比，其优点是您可以创建连接，就像在专用应用程序中一样。

要查看可用AdobeAPI的列表，请参阅[AdobeAPI](https://developer.adobe.com/apis)。 您可能只能使用分配给您的API。

## 访问要求

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 计划</td>
      <td>
        <p>新建：任何</p><p>或</p><p>当前： [！UICONTROL Pro]或更高版本</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 许可证</td>
      <td>
        <p>新增：标准</p><p>或</p><p>当前： [！UICONTROL计划]，[！UICONTROL工作]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证</td>
      <td>
   <p>当前Fusion许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版Fusion许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">产品</td>
      <td>
   <p>新的Workfront计划：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中所述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>当前Workfront计划：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中描述的功能。</p>
   </td>
    </tr>
  </tbody>
</table>

## 先决条件

* 您必须具有您希望模块连接到的Adobe产品的访问权限。
* 您必须具有Adobe Developer Console的访问权限。
* 您在Adobe Developer Console上必须有一个项目，该项目包含您希望模块连接到的API。 您可以：

   * 使用API创建新项目。

     或
   * 将API添加到现有项目。

  有关在Adobe Developer Console上创建API或将API添加到项目的信息，请参阅Adobe文档中的[创建项目](https://developer.adobe.com/dep/guides/dev-console/create-project/)。

## 创建连接

Adobe Authenticator连接可连接到Adobe Developer Console上的单个项目。 要对多个AdobeAPI使用相同的连接，请将API添加到同一项目，然后创建与该项目的连接。

您可以为不同的项目创建单独的连接，但无法使用连接访问不在该连接中指定的项目上的API。

>[!IMPORTANT]
>
>使用Adobe Authenticator连接器，您可以选择建立OAuth服务器到服务器连接或服务帐户(JWT)连接。 Adobe已弃用JWT凭据，这些凭据将在2025年1月1日之后停止工作。 **因此，我们强烈建议您创建OAuth连接。**
>
>有关这些类型连接的详细信息，请参阅Adobe文档中的[服务器到服务器身份验证](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/)

要创建连接，请执行以下操作：

1. 在任意Adobe Authenticator模块中，单击连接字段旁边的&#x200B;**添加**。
1. 填写以下字段：

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL连接类型]</td>
        <td>
          <p>选择是要创建OAuth服务器到服务器连接，还是要创建服务帐户(JWT)连接。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL连接名称]</td>
        <td>
          <p>输入此连接的名称。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL客户端ID]</td>
        <td>输入您的[!DNL Adobe]客户端ID。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL客户端密钥]</td>
        <td>输入您的[!DNL Adobe]客户端密钥。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL范围]</td>
        <td>如果您选择了OAuth连接，请输入此连接所需的范围。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL技术帐户ID]</td>
        <td>输入您的[!DNL Adobe]技术帐户ID。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL组织ID]</td>
        <td>如果您选择了JWT连接，请输入您的[!DNL Adobe]组织ID。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL元范围]</td>
        <td>如果已选择JWT连接，请输入此连接所需的元范围。 </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL私钥]</td>
        <td>
          <p>如果您选择了JWT连接，请输入在[!DNL Adobe Developer Console]中创建凭据时生成的私钥。 </p>
          <p>要提取您的私钥或证书，请执行以下操作：</p>
          <ol>
            <li value="1">
              <p>单击<b>[！UICONTROL提取]</b>。</p>
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
              <p>单击<b>[！UICONTROL保存]</b>以提取文件并返回到连接设置。</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL基本URL]</td>
        <td>必须添加希望此验证器允许的基本URL。 在场景的后面部分使用进行自定义API调用模块时，您将添加选定URL的相对路径。 通过在此处输入URL，您可以控制发出自定义API调用模块可以连接到的内容，从而提高安全性。<p>对于要添加到验证器的每个基本URL，单击<b>添加项</b>并输入基本URL。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL身份验证URL]</td>
        <td>将此项留空以使用<code>https://ims-na1.adobelogin.com</code>的标准Adobe IMS身份验证URL。 如果不使用Adobe IMS进行身份验证，请输入用于身份验证的URL。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL环境]</td>
        <td>选择您要连接到生产环境还是非生产环境。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL类型]</td>
        <td>选择您是要连接到服务帐户还是个人帐户。</td>
      </tr>
    </tbody>
    </table>

1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;保存连接并返回模块。

## 模块

### 进行自定义API调用

通过此操作模块，可调用任何AdobeAPI。

>[!TIP]
>
>您必须为要连接的API输入整个URL。 此模块不接受相对URL。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[！UICONTROL Connection]</td>
     <td>有关创建与Adobe Authenticator模块的连接的说明，请参阅本文中的<a href="#create-a-connection" class="MCXref xref" >创建连接</a>。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL URL]</p>
      </td>
      <td>
        <p>输入要连接到的API点的整个URL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion会自动添加授权标头。</p>
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
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入您希望模块在一个执行周期内返回的结果的最大数目。</p>
      </td>
    </tr>
  </tbody>
</table>
