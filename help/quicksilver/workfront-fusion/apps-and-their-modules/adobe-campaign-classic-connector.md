---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8模块
description: 使用 [!DNL Adobe Campaign] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于您的事件的场景 [!DNL Adobe Campaign] 帐户，创建、读取或更新协议和其它记录，使用您设置的标准搜索记录，以及加载文档。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 7decc5cbf4bb2c3d4d1802dec1f369ca061f6b48
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# [!DNL Adobe Campaign] 模块

使用 [!DNL Adobe Campaign] 模块，您可以启动 [!DNL Adobe Workfront Fusion] 基于您的事件的场景 [!DNL Adobe Campaign v7/v8] 帐户，创建、读取或更新记录，使用您设置的标准搜索记录，以及执行自定义API调用。

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

必须将Fusion IP地址添加到 [!DNL Adobe Campaign].

* 有关将IP地址添加到Campaign允许列表的说明，请参阅 [将IP地址添加到允许列表](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) 请参阅Adobe Campaign文档。
* 有关要添加到允许列表的IP地址的列表，请参见 [用于访问Adobe Workfront Fusion的IP地址](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## 连接 [!DNL Adobe Campaign] 到 [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>我们强烈建议创建服务器到服务器连接。 Adobe Campaign更新了其API，以仅接受服务器到服务器连接。 如果您要连接到Campaign版本8或更高版本，则 **必须** 创建服务器到服务器连接。
>
>有关Campaign新连接要求的更多信息，请参阅 [将Campaign技术操作员迁移到Adobe Developer控制台](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) 请参阅Campaign文档。

1. 在任何 [!DNL Adobe Campaign] 模块，单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 字段。
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
            <p>选择是要创建基本连接，还是要创建服务器到服务器连接。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL连接名称]</td>
          <td>
            <p>输入此连接的名称。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL基本URL]</td>
          <td>输入用于连接到 [!DNL Adobe Campaign] 实例。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL用户名]</td>
          <td>如果要创建基本连接，请输入您的Adobe Campaign用户名。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL密码]</td>
          <td>如果要创建基本连接，请输入您的Adobe Campaign密码。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端ID]</td>
          <td>如果要创建服务器到服务器连接，请输入 [!DNL Adobe] [！UICONTROL客户端ID]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端密钥]</td>
          <td>如果要创建服务器到服务器连接，请输入 [!DNL Adobe] [！UICONTROL客户端密钥]。 可在[！UICONTROL凭据详细信息]部分中找到此凭据。 [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL环境]</td>
          <td>选择您是连接到生产环境还是非生产环境。
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL类型]</td>
          <td>选择您是要连接到服务帐户还是个人帐户。
        </tr>
   </tbody>
    </table>
1. 单击 **[!UICONTROL 继续]** 以创建连接并返回模块。

## [!DNL Adobe Campaign] 模块及其字段

配置时 [!DNL Adobe Campaign] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Adobe Campaign] 字段可能会显示，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!UICONTROL 观察记录]

此计划触发器模块在记录更改时启动方案。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL筛选器]</td> 
   <td>选择要监视新记录、更新记录还是两者。</td> 
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
   <td role="rowheader">[！UICONTROL要包含在输出中的自定义字段]</td> 
   <td>对于每个要包含在输出中的自定义字段，请单击 <b>[！UICONTROL添加]</b> 并输入自定义字段的名称。</td> 
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

此操作模块在中创建新记录 [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign] 要创建的记录。</td> 
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

此模块对进行自定义API调用 [!DNL Adobe Campaign] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
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
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加[！UICONTROL x-security]令牌标头。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL XML Body]</td>
   <td> <p>以XML形式为API调用添加正文内容，而不添加会话元素。 </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块会从中删除单个记录 [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
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

此操作模块对中的对象执行选定的操作 [!DNL Adobe Campaign] API。

有关特定操作和字段的信息，请参阅 [[!DNL Adobe Campaign] - API文档](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作]</td> 
   <td><p>选择要对对象执行的操作。</p>
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

此操作模块从读取记录 [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign] 要读取的记录。</td> 
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
   <td role="rowheader">[！UICONTROL要包含在输出中的自定义字段]</td> 
   <td>对于每个要包含在输出中的自定义字段，请单击 <b>[！UICONTROL添加]</b> 并输入自定义字段的名称。</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL 订阅或取消订阅]

此操作模块为用户订阅或取消订阅信息服务的用户。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
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

此操作模块更新中的单个记录 [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign] 要创建的记录。</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[！UICONTROL ID] </td> 
   <td>输入要更新的记录的映射ID。</td> 
  </tr> 
<tr> 
   <td role="rowheader">[！UICONTROL字段] </td> 
   <td>选择要更新其值的字段，然后填写这些字段的值。 字段因您选择的记录类型而异。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自定义字段]</td> 
   <td> 对于每个要更新的自定义字段，请单击 <b>[！UICONTROL添加项]</b> 并输入或映射字段的名称和值。 </td> 
  </tr> 
 </tbody> 
</table>

### 搜索

#### [!UICONTROL 搜索]

此搜索模块会根据指定的条件返回记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与的连接 [!DNL Adobe Campaign]，请参见 <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与的连接 [!DNL Adobe Campaign]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择类型 [!DNL Adobe Campaign] 要创建的记录。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
