---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: AdobeMaestro模块
description: 使用 [!DNL Adobe Maestro] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于您的事件的场景 [!DNL Adobe] Maestro帐户，创建、读取或更新协议和其它记录，使用您设置的标准搜索记录，以及上载文档。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL Adobe Maestro] 模块

使用 [!DNL Adobe Maestro] 模块，则可以在Maestro中发生事件时触发方案。 您还可以创建、读取、更新和删除记录，或者对执行自定义API调用 [!DNL Adobe Maestro] 帐户。

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

## 创建与的连接 [!DNL Adobe Maestro]

您可以创建与 [!DNL Maestro] 直接从 [!DNL Workfront Fusion] 模块。

1. 在任何 [!DNL Maestro] 应用程序模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 盒子。
1. 输入此连接的名称。
1. 选择您要连接到生产环境还是非生产环境。
1. 选择您是要连接到服务帐户还是个人帐户。
1. 单击 **[!UICONTROL SAML登录]** 以创建连接并返回模块。

## [!DNL Adobe Maestro] 模块及其字段

### 观看活动

在Maestro中创建、更新或删除记录、记录类型或工作区时，此触发器模块会启动一个方案。

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
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL对象类型]</td>
      <td>选择您要监视记录、记录类型还是工作区。</td>
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

### 删除记录类型

此操作模块通过ID删除Maestro中的单个记录类型。

>[!WARNING]
>
>删除Maestro中的记录类型也会删除记录类型表中的所有记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录类型ID]</p>
      </td>
      <td>输入或映射要删除的字段的ID。</td> 
      </tr>
  </tbody>
</table>

### 进行自定义API调用

此模块对进行自定义API调用 [!DNL Adobe Maestro] API。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL路径]</p>
      </td>
      <td>
        <p>输入相对于https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/的路径</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL API版本]</p>
      </td>
      <td>
        <p>选择要使用的API版本。 如果不选择版本，则默认情况下将使用最新版本。</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL API路径覆盖]</p>
      </td>
      <td>
        <p>输入相对于https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/的路径</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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
        <p>对于要添加到查询字符串的每个键/值对，单击 <b>添加项目</b> 并输入键和值。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Body]</td>
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### 创建记录

此操作在Maestro中创建单个记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录类型ID]</p>
      </td>
      <td>输入或映射要创建的记录类型。 可用的记录类型取决于您的Maestro帐户。</td> 
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

此操作模块删除Maestro中的指定记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
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

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
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

此操作模块从检索单个记录 [!DNL Adobe Maestro]，由其ID指定。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
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
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL工作区]</td>
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

此操作模块检索 [!DNL Adobe Maestro] 帐户。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
  </tbody>
</table>

### 更新记录

此操作更新Maestro中的单个记录。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
      <td>有关创建与的连接 [!DNL Adobe Maestro]，请参见 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >创建与的连接 [!DNL Adobe Maestro]</a> 本文章中。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[！UICONTROL记录ID]</p>
      </td>
      <td>输入或映射要更新的记录类型。 可用的记录类型取决于您的Maestro帐户。</td> 
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

### 搜索记录

此操作模块根据您指定的条件检索记录列表。

>[!NOTE]
>
>此模块正在构建中。

