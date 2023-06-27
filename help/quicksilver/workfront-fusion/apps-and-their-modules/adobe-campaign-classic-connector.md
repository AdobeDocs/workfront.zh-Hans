---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic模块
description: 使用 [!DNL Adobe Campaign Classic] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 场景基于中的事件 [!DNL Adobe Campaign Classic] 帐户、创建、读取或更新协议和其它记录、使用您设置的标准搜索记录以及上传文档。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '1194'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic] 模块

使用 [!DNL Adobe Campaign Classic] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 场景基于中的事件 [!DNL Adobe Campaign Classic] 帐户、创建、读取或更新记录、使用您设置的标准搜索记录，以及执行自定义API调用。

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

## Connect [!DNL Adobe Campaign Classic] 到 [!DNL Adobe Workfront Fusion]

1. 在任意 [!DNL Adobe Campaign Classic] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
1. 输入用于连接到您的网站的基本URL [!DNL Adobe Campaign Classic] 实例。
1. 输入用户名和密码。
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Adobe Campaign Classic] 模块及其字段

配置时 [!DNL Adobe Campaign Classic] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Adobe Campaign Classic] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观看记录]

此计划触发器模块在记录更改时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td>选择是要监视新记录、更新的记录，还是同时监视两者。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择要监视的资源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要包含在输出中的[！UICONTROL字段]</td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要包含在输出中的[！UICONTROL自定义字段]</td> 
   <td>对于要包含在输出中的每个自定义字段，请单击 <b>[！UICONTROL添加]</b> 并输入自定义字段的名称。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回结果的最大数目]</td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
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

此操作模块在中创建新记录 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign Classic] 要创建的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段] </td> 
   <td>选择创建记录时要为其设置值的字段，然后填写这些字段的值。 字段因您选择的记录类型而异。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自定义字段]</td> 
   <td> 对于要添加到新记录的每个自定义字段，单击 <b>[！UICONTROL添加项]</b> 并输入或映射字段的名称和值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行自定义API调用]

此模块对进行自定义API调用 [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL操作]</td>
      <td><p>选择您希望API调用执行的操作。</p>
      <p>[！UICONTROL执行查询]</p>
      <p>[！UICONTROL写入]</p>
      <p>[！UICONTROL Get entity if more recent]</p>
      <p>[！UICONTROL全选]</p>
      <p>[！UICONTROL推送事件]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL标头]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加[！UICONTROL x-security]令牌标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL XML正文]</td>
   <td> <p>在XML中添加API调用的正文内容，而不使用会话元素。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块会从中删除单个记录 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择要删除的资源类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL ID]</td> 
   <td>输入或映射要删除的资源的ID。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 执行操作]

此操作模块对中的对象执行选定的操作 [!DNL Adobe Campaign Classic] API。

有关特定操作和字段的信息，请参阅 [[!DNL Adobe Campaign] - API文档](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作]</td> 
   <td><p>选择要在对象上执行的操作。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 有关可用字段，请参阅 <a href="#search" class="MCXref xref" >[！UICONTROL搜索]</a> 本文章中。 </p></li>
     <li><p><b>[！UICONTROL Get]</b></p><p> 有关可用字段，请参阅 <a href="#search" class="MCXref xref" >[！UICONTROL搜索]</a> 本文章中。 </p></li> 
   <li><p><b>[！UICONTROL创建]</b></p><p> 有关可用字段，请参阅 <a href="#create-a-record" class="MCXref xref" >[！UICONTROL创建记录]</a> 本文章中。 </p></li>
   <li><p><b>[！UICONTROL更新]</b></p><p> 有关可用字段，请参阅 <a href="#update-record" class="MCXref xref" >[！UICONTROL更新记录]</a> 本文章中。 </p></li>
   <li><p><b>[！UICONTROL Delete]</b></p><p> 有关可用字段，请参阅 <a href="#delete-record" class="MCXref xref" >[！UICONTROL删除记录]</a> 本文章中。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块从以下位置读取记录 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign Classic] 您想要读取的记录。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL ID] </td> 
   <td>在映射中输入要读取的记录的ID。</td> 
  </tr> 
 <tr> 
   <td role="rowheader">要包含在输出中的[！UICONTROL字段] </td> 
   <td>选择要包含在模块输出中的字段。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要包含在输出中的[！UICONTROL自定义字段]</td> 
   <td>对于要包含在输出中的每个自定义字段，请单击 <b>[！UICONTROL添加]</b> 并输入自定义字段的名称。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 订阅或取消订阅]

此操作模块为用户订阅或取消订阅信息服务。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL订阅或取消订阅]</td> 
   <td>选择您要订阅还是取消订阅信息服务。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL服务名称]</td> 
   <td>选择要订阅或取消订阅的服务。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL收件人电子邮件地址] </td> 
   <td>输入或映射要订阅或取消订阅信息服务的用户的电子邮件地址。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块更新中的单个记录 [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign Classic] 要创建的记录。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL ID] </td> 
   <td>输入要更新的记录ID的映射。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL字段] </td> 
   <td>选择要更新值的字段，然后填写这些字段的值。 字段因您选择的记录类型而异。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自定义字段]</td> 
   <td> 对于每个要更新的自定义字段，请单击 <b>[！UICONTROL添加项]</b> 并输入或映射字段的名称和值。 </td> 
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
   <td role="rowheader">[！UICONTROL连接]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign Classic]，请参见 <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >创建连接 [!DNL Adobe Campaign Classic]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign Classic] 要创建的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
