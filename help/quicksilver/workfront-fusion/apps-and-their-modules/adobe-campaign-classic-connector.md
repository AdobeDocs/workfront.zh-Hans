---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8模块
description: 使用 [!DNL Adobe Campaign] 模块，您可以基于 [!DNL Adobe Campaign] 帐户中的事件启动 [!DNL Adobe Workfront Fusion] 方案，创建、读取或更新协议和其他记录，使用您设置的条件搜索记录以及上载文档。
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 1%

---

# [!DNL Adobe Campaign]模块

通过[!DNL Adobe Campaign]模块，您可以基于[!DNL Adobe Campaign v7/v8]帐户中的事件启动[!DNL Adobe Workfront Fusion]方案，创建、读取或更新记录，使用您设置的条件搜索记录，以及执行自定义API调用。

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

必须将Fusion IP地址添加到[!DNL Adobe Campaign]。

* 列入允许列表 列入允许列表有关将IP地址添加到Campaign的说明，请参阅Adobe Campaign文档中的[将IP地址添加到](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list)。
* 有关要添加到允许列表的IP地址列表，请参阅[用于访问Adobe Workfront Fusion的IP地址](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md)。

## Adobe Campaign API信息

Adobe Campaign连接器使用以下对象：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API标记</td> 
   <td>v1.7.22</td> 
  </tr>
 </tbody> 
 </table>

## 将[!DNL Adobe Campaign]连接到[!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>我们强烈建议创建服务器到服务器连接。 Adobe Campaign更新了其API，以仅接受服务器到服务器连接。 如果要连接到Campaign版本8或更高版本，则&#x200B;**必须**&#x200B;创建服务器到服务器连接。
>
>有关Campaign新连接要求的详细信息，请参阅Campaign文档中的[将Campaign技术操作员迁移到Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html)。

1. 在任意[!DNL Adobe Campaign]模块中，单击[!UICONTROL 连接]字段旁边的&#x200B;**[!UICONTROL 添加]**。
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
          <td>输入用于连接到[!DNL Adobe Campaign]实例的基本URL。</td>
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
          <td>如果要创建服务器到服务器连接，请输入您的[!DNL Adobe] [！UICONTROL客户端ID]。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。</td>
        </tr>
        <tr>
          <td role="rowheader">[！UICONTROL客户端密钥]</td>
          <td>如果要创建服务器到服务器连接，请输入您的[!DNL Adobe] [！UICONTROL客户端密钥]。 这可以在[!DNL Adobe Developer Console]的[！UICONTROL凭据详细信息]部分找到。
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
1. 单击&#x200B;**[!UICONTROL 继续]**&#x200B;以创建连接并返回模块。

## [!DNL Adobe Campaign]模块及其字段

配置[!DNL Adobe Campaign]模块时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，可能还会显示其他[!DNL Adobe Campaign]字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)中将信息从一个模块映射到另一个模块。

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
   <td role="rowheader">[！UICONTROL Connection]</td> 
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
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
   <td>对于要包含在输出中的每个自定义字段，请单击<b>[！UICONTROL添加]</b>并输入自定义字段的名称。</td> 
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

此操作模块在[!DNL Adobe Campaign]中创建新记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择要创建的[!DNL Adobe Campaign]记录的类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL字段] </td> 
   <td>选择创建记录时要为其设置值的字段，然后填写这些字段的值。 字段因您选择的记录类型而异。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL自定义字段]</td> 
   <td> 对于要添加到新记录的每个自定义字段，单击<b>[！UICONTROL添加项]</b>并输入或映射字段的名称和值。 </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 进行自定义API调用]

此模块对[!DNL Adobe Campaign] API进行自定义API调用

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
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

此操作模块从[!DNL Adobe Campaign]中删除单个记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
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

此操作模块对[!DNL Adobe Campaign] API中的对象执行选定的操作。

有关特定操作和字段的信息，请参阅[[!DNL Adobe Campaign] - API文档](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html)。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL操作]</td> 
   <td><p>选择要对对象执行的操作。</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> 有关可用字段，请参阅本文中的<a href="#search" class="MCXref xref" >[！UICONTROL搜索]</a>。 </p></li>
     <li><p><b>[！UICONTROL Get]</b></p><p> 有关可用字段，请参阅本文中的<a href="#search" class="MCXref xref" >[！UICONTROL搜索]</a>。 </p></li> 
   <li><p><b>[！UICONTROL创建]</b></p><p> 有关可用字段，请参阅本文中的<a href="#create-a-record" class="MCXref xref" >[！UICONTROL创建记录]</a>。 </p></li>
   <li><p><b>[！UICONTROL更新]</b></p><p> 有关可用字段，请参阅本文中的<a href="#update-record" class="MCXref xref" >[！UICONTROL更新记录]</a>。 </p></li>
   <li><p><b>[！UICONTROL Delete]</b></p><p> 有关可用字段，请参阅本文中的<a href="#delete-record" class="MCXref xref" >[！UICONTROL删除记录]</a>。 </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

此操作模块从[!DNL Adobe Campaign]读取记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择要读取的[!DNL Adobe Campaign]记录的类型。</td> 
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
   <td>对于要包含在输出中的每个自定义字段，请单击<b>[！UICONTROL添加]</b>并输入自定义字段的名称。</td> 
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
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
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

此操作模块更新[!DNL Adobe Campaign]中的单个记录。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL Connection]</td>
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择要创建的[!DNL Adobe Campaign]记录的类型。</td> 
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
   <td> 对于每个要更新的自定义字段，请单击<b>[！UICONTROL添加项]</b>并输入或映射该字段的名称和值。 </td> 
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
   <td>有关创建与[!DNL Adobe Campaign]的连接的说明，请参阅本文中的<a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >创建与[!DNL Adobe Campaign]</a>的连接。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL资源]</td> 
   <td>选择要创建的[!DNL Adobe Campaign]记录的类型。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL限制] </td> 
   <td>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</td> 
  </tr> 
 </tbody> 
</table>
