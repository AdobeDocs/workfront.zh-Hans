---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic模块
description: 使用 [!DNL Adobe Campaign Classic] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于 [!DNL Adobe Campaign Classic] 帐户、创建、读取或更新协议和其他记录、使用您设置的标准搜索记录，以及上传文档。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] 模块

使用 [!DNL Adobe Campaign Classic] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于 [!DNL Adobe Campaign Classic] 帐户、创建、读取或更新记录、使用您设置的标准搜索记录，以及执行自定义API调用。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 连接 [!DNL Adobe Campaign Classic] to [!DNL Adobe Workfront Fusion]

1. 在任意 [!DNL Adobe Campaign Classic] 模块，单击 **[!UICONTROL 添加]** 旁边 [!UICONTROL 连接] 字段。
1. 输入用于连接到的基本URL [!DNL Adobe Campaign Classic] 实例。
1. 输入您的用户名和密码。
1. 单击 **[!UICONTROL 继续]** 创建连接，然后返回到模块。

## [!DNL Adobe Campaign Classic] 模块及其字段

配置 [!DNL Adobe Campaign Classic] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Adobe Campaign Classic] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 监视记录]

此计划触发器模块会在记录发生更改时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td> 
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL过滤器]</td> 
   <td>选择您是要监视新记录、更新记录，还是同时监视这两者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源]</td> 
   <td>选择要监视的资源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要包含在输出中的字段]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要包含在输出中的自定义字段]</td> 
   <td>对于要包含在输出中的每个自定义字段，单击 <b>[!UICONTROL Add]</b> 并输入自定义字段的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL返回结果的最大数]</td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>


### 操作

* [[!UICONTROL 创建记录]](#create-a-record)
* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)
* [[!UICONTROL 删除记录]](#delete-record)
* [[!UICONTROL 执行操作]](#perform-an-action)
* [[!UICONTROL 读取记录]](#-read-a-record)
* [[!UICONTROL 订阅或取消订阅]](#subscribe-or-unsubscribe)
* [[!UICONTROL 更新记录]](#update-record)

#### [!UICONTROL 创建记录]

此操作模块会在 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源]</td> 
   <td>选择 [!DNL Adobe Campaign Classic] 记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL字段] </td> 
   <td>选择要在创建记录时为其设置值的字段，然后填写这些字段的值。 字段因您选择的记录类型而异。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自定义字段]</td> 
   <td> 对于要添加到新记录的每个自定义字段，单击 <b>[!UICONTROL添加项目]</b> 并输入或映射字段的名称和值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行自定义API调用]

此模块对 [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>选择您希望API调用执行的操作。</p>
      <p>[!UICONTROL Execute查询]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL获取实体（如果更新）]</p>
      <p>[!UICONTROL全选]</p>
      <p>[!UICONTROL推送事件]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL标头]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加[!UICONTROL x-security]令牌标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>在XML中为API调用添加正文内容，而不添加会话元素。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块从中删除单个记录 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源]</td> 
   <td>选择要删除的资源类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>输入或映射要删除的资源的ID。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 执行操作]

此操作模块对 [!DNL Adobe Campaign Classic] API。

有关特定操作和字段的信息，请参阅 [[!DNL Adobe Campaign] - API文档](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>选择要对对象执行的操作。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 有关可用字段，请参阅 <a href="#search" class="MCXref xref" >[!UICONTROL搜索]</a> 在本文中。 </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> 有关可用字段，请参阅 <a href="#search" class="MCXref xref" >[!UICONTROL搜索]</a> 在本文中。 </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> 有关可用字段，请参阅 <a href="#create-a-record" class="MCXref xref" >[!UICONTROL创建记录]</a> 在本文中。 </p></li>
   <li><p><b>[!UICONTROL更新]</b></p><p> 有关可用字段，请参阅 <a href="#update-record" class="MCXref xref" >[!UICONTROL更新记录]</a> 在本文中。 </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> 有关可用字段，请参阅 <a href="#delete-record" class="MCXref xref" >[!UICONTROL删除记录]</a> 在本文中。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从中读取记录 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源]</td> 
   <td>选择 [!DNL Adobe Campaign Classic] 要读的记录。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>输入要读取的记录的ID映射。</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL要包含在输出中的字段] </td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL要包含在输出中的自定义字段]</td> 
   <td>对于要包含在输出中的每个自定义字段，单击 <b>[!UICONTROL Add]</b> 并输入自定义字段的名称。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 订阅或取消订阅]

此操作模块可让用户订阅或取消订阅信息服务的用户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL订阅或取消订阅]</td> 
   <td>选择是要订阅还是取消订阅信息服务。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL服务名称]</td> 
   <td>选择要订阅或取消订阅的服务。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL收件人电子邮件地址] </td> 
   <td>输入或映射要订阅或取消订阅信息服务的用户的电子邮件地址。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块会更新 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源]</td> 
   <td>选择 [!DNL Adobe Campaign Classic] 记录。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>输入要更新记录的ID映射。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL字段] </td> 
   <td>选择要更新值的字段，然后填写这些字段的值。 字段因您选择的记录类型而异。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL自定义字段]</td> 
   <td> 对于要更新的每个自定义字段，单击 <b>[!UICONTROL添加项目]</b> 并输入或映射字段的名称和值。 </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 搜索]

此搜索模块根据指定的条件返回记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL连接]</td>
   <td>有关创建与 [!DNL Adobe Campaign Classic]，请参阅 <a href="#connect-adobe-campaign-connector-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 在本文中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL资源]</td> 
   <td>选择 [!DNL Adobe Campaign Classic] 记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL限制] </td> 
   <td>输入或映射您希望模块在每个方案执行周期期间返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
