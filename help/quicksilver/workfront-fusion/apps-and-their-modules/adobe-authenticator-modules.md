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
source-git-commit: 61a579c19228381d0aa06de3db5217614999731b
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 1%

---

# Adobe Authenticator模块

Adobe Authenticator模块允许您通过单个连接连接到任何AdobeAPI。 这允许您更轻松地连接到尚未拥有专用Fusion连接器的Adobe产品。

与HTTP模块相比，其优点是您可以创建连接，就像在专用应用程序中一样。

要查看可用AdobeAPI的列表，请参阅 [ADOBEAPI](https://developer.adobe.com/apis). 您可能只能使用分配给您的API。

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
   <p>当前Fusion许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版Fusion许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">产品</td>
      <td>
   <p>新的Workfront计划：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>当前Workfront计划：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td>
    </tr>
  </tbody>
</table>

## 先决条件

* 您必须具有您希望模块连接到的Adobe产品的访问权限。
* 您必须有权访问Adobe Developer控制台。
* 您在Adobe Developer控制台上必须有一个项目，该项目包含希望模块连接到的API。 您可以：

   * 使用API创建新项目。

     或
   * 将API添加到现有项目。

  有关在Adobe Developer控制台中创建或向项目添加API的信息，请参阅 [创建项目](https://developer.adobe.com/dep/guides/dev-console/create-project/) 在Adobe文档中。

## 创建连接

Adobe Authenticator连接可连接到Adobe Developer控制台上的单个项目。 要对多个AdobeAPI使用相同的连接，请将API添加到同一项目，然后创建与该项目的连接。

您可以为不同的项目创建单独的连接，但无法使用连接访问不在该连接中指定的项目上的API。

>[!IMPORTANT]
>
>使用Adobe Authenticator连接器，您可以选择建立OAuth服务器到服务器连接或服务帐户(JWT)连接。 Adobe已弃用JWT凭据，这些凭据将在2025年1月1日之后停止工作。 **因此，我们强烈建议您创建OAuth连接。**
>
>有关这些类型连接的详细信息，请参见 [服务器到服务器身份验证](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) Adobe文档中的

要创建连接，请执行以下操作：

1. 在任意Adobe Authenticator模块中，单击 **添加** ，位于连接字段旁。
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
        <td>输入您的 [!DNL Adobe] 客户端ID。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL客户端密钥]</td>
        <td>输入您的 [!DNL Adobe] 客户端密码。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL范围]</td>
        <td>如果您选择了OAuth连接，请输入此连接所需的范围。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL技术帐户ID]</td>
        <td>输入您的 [!DNL Adobe] 技术帐户ID。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL组织ID]</td>
        <td>如果您已选择JWT连接，请输入 [!DNL Adobe] 组织ID。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL元范围]</td>
        <td>如果已选择JWT连接，请输入此连接所需的元范围。 </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL私钥]</td>
        <td>
          <p>如果您选择了JWT连接，请输入您的凭据在中创建时生成的私钥。 [!DNL Adobe Developer Console]. </p>
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
              <p>单击 <b>[！UICONTROL保存]</b> 以提取文件并返回到连接设置。</p>
            </li>
          </ol>
        </td>
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

1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

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
     <td>有关创建与Adobe Authenticator模块的连接的说明，请参阅 <a href="#create-a-connection" class="MCXref xref" >创建连接</a> 本文章中。</td>
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
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
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

