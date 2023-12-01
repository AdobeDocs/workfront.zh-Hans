---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Forms模块
description: 使用 [!DNL Adobe Experience Manager Forms] 连接器 [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Forms] 帐户，创建、上传和更新资产，以及复制或移动文件夹和资产。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c4e068729d8de4bef4b2018868e3fa020ca61a06
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 1%

---

# [!DNL Adobe Experience Manager Forms] 模块

使用 [!DNL Adobe Experience Manager Forms] 连接器 [!DNL Adobe Workfront Fusion]，您可以根据中的事件启动方案 [!DNL Adobe Experience Manager Forms] 通过创建webhook创建的帐户。

您可以在中配置表单 [!DNL Adobe Experience Manager Forms] 以将表单提交发送到此webhook。

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
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关的信息 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

* 您必须拥有 [!DNL Adobe Experience Manager Forms] 帐户以使用此模块。

## 创建与Adobe Experience Manager Forms的连接

要为创建连接，请执行以下操作 [!DNL Adobe Experience Manager Forms] 模块：

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
        <td role="rowheader">[！UICONTROL环境]</td>
        <td>
          <p>选择此连接是连接到生产环境还是非生产环境。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL类型]</td>
        <td>
          <p>选择此帐户是服务帐户还是个人帐户。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL实例URL，不带尾随斜杠]</td>
        <td>
          <p>输入用于访问帐户的URL，不带最后一个斜杠。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL IMS端点]</td>
        <td>
          <p><code>https://ims-na1.adobelogin.com</code></p>
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
        <td role="rowheader">[！UICONTROL组织ID]</td>
        <td>输入您的 [!DNL Adobe] 组织ID。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL技术帐户ID]</td>
        <td>输入您的 [!DNL Adobe] 技术帐户ID。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL元范围]</td>
        <td>输入任何适当的元范围       </td>
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
              <p>单击 <b>[！UICONTROL保存]</b> 以提取文件并返回到连接设置。</p>
            </li>
          </ol>
        </td>
      </tr>
    </tbody>
    </table>

1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

## Adobe Experience Manager Forms模块及其字段

目前，Adobe Experience Manager Forms连接器只有一个模块。

### 关注表单事件

这个即时触发器(webhook)允许您在Adobe Experience Manager表单上发生提交操作时启动场景。

>[!IMPORTANT]
>
>此外，还需要在Adobe Experience Manager中配置此模块。 设置此webhook后，必须打开Adobe Experience Manager并配置表单以将提交内容发送到webhook。
>
><!--For instructions on the required form configuration, see insert url here-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Webhook名称]</td> 
   <td> <p>输入webhook的名称</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td> <p>有关连接 [!DNL Adobe Experience Manager] 帐户至 [!DNL Workfront Fusion]，请参见 <a href="../../workfront-fusion/apps-and-their-modules/aem-forms-modules.md#create-a-connection-to-adobe-experience-manager-forms" class="MCXref xref">创建与的连接 [!DNL Adobe Experience Manager Forms]</a></p> </td> 
  </tr>

模块将创建一个webhook并提供webhook地址，您可以在中的表单提交对话框中输入该地址 [!DNL Adobe Experience Manager Forms].











