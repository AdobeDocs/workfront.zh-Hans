---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Workfront规划模块
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning]模块

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [Adobe Workfront规划模块](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

通过[!DNL Adobe Workfront Planning]模块，您可以在Workfront Planning中发生事件时触发方案。 您还可以创建、读取、更新和删除记录，或者对您的[!DNL Adobe Workfront Planning]帐户执行自定义API调用。

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

## Adobe Workfront规划API信息

Adobe Workfront Planning连接器使用以下对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">基本URL</td> 
   <td>https://&lbrace;&lbrace;connection.host&rbrace;&rbrace;/maestro/api/&lbrace;&lbrace;common.maestroApiVersion&rbrace;&rbrace;/</td> 
  </tr>
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v1.13.7</td> 
  </tr>
 </tbody> 
 </table>

## 创建与[!DNL Adobe Workfront Planning]的连接

您可以在[!DNL Workfront Fusion]模块内直接创建与[!DNL Workfront Planning]帐户的连接。

1. 在任意[!DNL Adobe Workfront Planning]模块中，单击“连接”框旁边的&#x200B;**[!UICONTROL 添加]**。

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
          <td>选择您要连接到生产环境还是非生产环境。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL类型]</td>
          <td>选择您是要连接到服务帐户还是个人帐户。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端ID]<p>（可选）</p></td>
          <td>输入您的[!DNL Adobe] [！UICONTROL客户端ID]。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端密钥]<p>（可选）</p></td>
          <td>输入您的[!DNL Adobe] [！UICONTROL客户端密钥]。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL身份验证URL]<p>（可选）</p></td>
          <td>输入您的Workfront实例将用于对此连接进行身份验证的URL。 <p>默认值为<code>https://oauth.my.workfront.com/integrations/oauth2</code>。</p>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL主机前缀]</td>
          <td>输入您的主机前缀。<p>默认值为<code>origin-</code>。</p>
        </tr>
      </tbody>
    </table>
1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;保存连接并返回模块。

## [!DNL Adobe Workfront Planning]模块及其字段

### 触发器

#### 观看活动

在Workfront Planning中创建、更新或删除记录、记录类型或工作区时，此触发器模块将启动一个方案。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Webhook]</td>
      <td>选择要使用的webhook，或单击“添加”以创建一个新挂接。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL对象类型]</td>
      <td>选择您要监视记录、记录类型还是工作区。</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[！UICONTROL事件过滤器]</p> </td> 
      <td> <p>您可以设置过滤器，以仅监视符合您选择标准的记录。</p> <p>对于每个筛选器，输入希望筛选器计算的字段、运算符以及希望筛选器允许的值。 通过添加AND规则，您可以使用多个过滤器。</p> <p>注意：您无法编辑现有[!DNL Workfront] Webhook中的筛选器。 要为[!DNL Workfront]事件订阅设置不同的筛选器，请删除当前webhook并创建一个新筛选器。</p> <p>有关事件过滤器的详细信息，请参阅Workfront模块文章中的[!DNL Workfront] &gt; [！UICONTROL监视事件]模块中的<a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">事件订阅过滤器</a>。</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[！UICONTROL要监视的对象]</td>
      <td>选择是否要监视新的。 更新、新增和更新或删除的记录。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL排除此连接所做的更新]</p>
      </td>
      <td>启用此选项可防止在此模块使用的连接进行更改时触发场景。 如果场景执行触发操作，这将阻止触发场景的另一个实例。</td> 
      </tr>
  </tbody>
</table>

### 操作

* [删除记录类型](#delete-a-record-type)
* [进行自定义AI调用](#make-a-custom-api-call)

#### 删除记录类型

此操作模块通过ID删除Workfront Planning中的单个记录类型。

>[!WARNING]
>
>删除Workfront Planning中的记录类型也会删除记录类型表中的所有记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录类型ID]</p>
      </td>
      <td>输入或映射要删除的字段的ID。</td> 
      </tr>
  </tbody>
</table>

#### 进行自定义API调用

此模块对[!DNL Adobe Workfront Planning] API进行自定义API调用。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL URL]</p>
      </td>
      <td>
        <p>输入相对路径 <code>https://(YOUR_WORKFRONT_DOMAIN)/maestro/api/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关详细信息，请参阅[!DNL Adobe Workfront Fusion]</a>中的<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP请求方法。</p> </td> 
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
        <p>对于要添加到查询字符串的每个键/值对，单击<b>添加项</b>并输入键和值。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--
### Searches

#### Search records

This action module retrieves a list of records based on criteria you specify.

-->

### 未分类


#### 创建记录

此操作在Workfront Planning中创建单个记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录类型ID]</p>
      </td>
      <td>输入或映射要创建的记录类型。 可用的记录类型基于您的Workfront Planning帐户。</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>其他字段</p>
      </td>
      <td>这些字段基于您选择的记录类型。</td> 
      </tr>
     <tr>
  </tbody>
</table>

### 删除记录

此操作模块删除Workfront Planning中的指定记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录ID]</p>
      </td>
      <td>输入或映射要删除的记录的ID。</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### 获取记录

此操作模块从其ID指定的[!DNL Adobe Workfront Planning]中检索单个记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL记录ID]</td>
      <td>输入或映射要检索的记录的ID。</td>
    </tr>
  </tbody>
</table>

### 按记录类型获取记录

此操作模块检索指定类型的所有记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Workspace]</td>
      <td>选择或映射包含要检索的记录的工作区。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL记录类型]</td>
      <td>选择要检索的记录类型。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL返回的最大记录数]</p>
      </td>
      <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tbody>
</table>

### 获取记录类型

此操作模块检索[!DNL Adobe Workfront Planning]帐户中的记录类型列表。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
  </tbody>
</table>

### 更新记录

此操作更新Workfront Planning中的单个记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与[!DNL Adobe Workfront Planning]的连接的说明，请参阅本文中的<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >创建与[!DNL Adobe Workfront Planning]</a>的连接。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录ID]</p>
      </td>
      <td>输入或映射要更新的记录类型。 可用的记录类型基于您的Workfront Planning帐户。</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>其他字段</p>
      </td>
      <td>这些字段基于您选择的记录类型。</td> 
      </tr>
     <tr>
  </tbody>
</table>
