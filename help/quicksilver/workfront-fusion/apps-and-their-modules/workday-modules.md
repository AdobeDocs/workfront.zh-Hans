---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Workday模块
description: 在Adobe Workfront Fusion场景中，您可以自动执行使用 [!DNL Workday]，并将其连接到多个第三方应用程序和服务。
author: Becky
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 1%

---

# [!DNL Workday] 模块

在 [!DNL Adobe Workfront Fusion] 方案中，您可以自动执行使用 [!DNL Workday]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参阅 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 先决条件

使用 [!DNL Workday] 模块，您必须：

* 拥有 [!DNL Workday] 帐户。

* 在中创建OAuth应用程序 [!DNL Workday]. 有关说明，请参阅 [!DNL Workday] 文档。

## 连接 [!DNL Workday] to [!DNL Workfront Fusion]

1. 在任意 [!DNL Workfront Fusion] 模块，单击 [!UICONTROL 添加] 旁边 [!UICONTROL 连接] 字段

2. 填写以下字段：

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL连接名称]</p>
                </td>
                <td>输入连接的名称</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday主机]</td>
                <td>输入的地址 [!DNL Workday] 不包含 <code>https://</code>. 例如： <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL服务URL]</td>
                <td>输入的地址 [!DNL Workday] Web服务不提供 <code>https://</code>. 例如： <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL租户名称]</td>
                <td>输入此的租户 [!DNL Workday] 帐户。 您的租户是贵组织的标识符，可在用于登录Workday的URL中看到。 示例：地址 <code>https://www.myworkday.com/mycompany</code>，租户为 <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL客户端ID]</td>
                <td>输入的客户端ID [!DNL Workday] 此连接使用的应用程序。 在中创建应用程序时，即会获取此信息 [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL客户端密钥]</td>
                <td>输入的客户端密钥 [!DNL Workday] 此连接使用的应用程序。 在中创建应用程序时，即会获取此信息 [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL会话超时（分钟）]</td>
                <td >输入授权令牌在其后过期的分钟数。</td>
            </tr>
        </tbody>
    </table>


3. 单击 [!UICONTROL 继续] 保存连接并返回到模块

## [!DNL Workday] 模块及其字段

配置 [!DNL Workday] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除了这些， [!DNL Workday] 字段可能会显示，具体取决于诸如应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果您看到字段或函数上方的映射按钮，则可以使用它为该字段设置变量和函数。 有关更多信息，请参阅 [在 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [操作](#action)

* [搜索](#search)


### 操作

* [[!UICONTROL 创建记录]](#create-a-record)

* [[!UICONTROL 删除记录]](#delete-a-record)

* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)

* [[!UICONTROL 更新记录]](#update-a-record)


#### [!UICONTROL 创建记录]

此操作模块在 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL连接]</td>
            <td>有关连接 [!DNL Workday] 帐户到Workfront Fusion，请参阅 <a href="#Connect" class="MCXref xre[!DNL ]f" >连接 [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL记录类型]</td>
            <td>选择要创建的记录类型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>输入或映射要创建的记录的ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL子资源ID]</td>
            <td >输入或映射要创建的子资源的ID。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 删除记录]

此操作模块将删除 [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL连接]</td>
            <td>有关连接 [!DNL Workday] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#Connect" class="MCXref xre[!DNL ]f" >连接 [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL记录类型]</td>
            <td>选择要删除的记录类型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL特定记录类型]</td>
            <td>选择要删除的特定记录类型。 这些值基于您选择的记录类型。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL子资源ID]</td>
            <td>输入或映射要删除的子资源的ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >输入或映射要删除的记录的ID。</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL 进行自定义API调用]

通过此操作模块，您可以对 [!DNL Workday] API。 这样，您就可以创建数据流自动化，而另一个数据流无法实现 [!DNL Workday] 模块。

配置此模块时，将显示以下字段。

模块会返回状态代码，以及API调用的标头和正文。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>有关连接 [!DNL Workday] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#Connect" class="MCXref xre[!DNL ]f" >连接 [!DNL Workday] to [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>输入相对于 <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL方法]</td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion]会为您添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL查询字符串]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的查询。</p> <p>例如： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式为API调用添加正文内容。</p> <p>注释:  <p>使用条件语句时，例如 <code>if</code> 在JSON中，将引号放置在条件语句的外部。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新记录]

此操作模块会更新 [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL连接]</td>
            <td>有关连接 [!DNL Workday] 帐户到Workfront Fusion，请参阅 <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] 到Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">记录类型</td>
            <td>选择要更新的记录t[!UICONTROL ]的类型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>输入或映射要更新的记录的ID。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL子资源ID]</td>
            <td >输入或映射要更新的子资源的ID。</td>
        </tr>
    </tbody>
</table>

### 搜索

* [[!UICONTROL 读取记录]](#read-a-record)

* [[!UICONTROL 列出记录]](#list-records)


#### [!UICONTROL 读取记录]

此操作模块读取单个记录。

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL连接]</td>
            <td>有关连接 [!DNL Workday] 帐户到Workfront Fusion，请参阅 <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] 到Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL记录类型]</td>
            <td>选择要删除的记录类型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL特定记录类型]</td>
            <td>选择要读取的特定记录类型。 这些值基于您选择的记录类型。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >输入或映射要删除的记录的ID。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL 列出记录]

此搜索模块检索指定类型的记录列表。

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL连接]</td>
              <td>有关连接 [!DNL Workday] 帐户 [!DNL Workfront Fusion]，请参阅 <a href="#Connect" class="MCXref xref" >连接 [!DNL Workday] to [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL记录类型]</td>
              <td>选择要检索的记录类型。</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL限制]</td>
              <td >
                  <p>输入或映射您希望模块在每个方案执行周期期间检索的最大记录数。</p>
              </td>
          </tr>
      </tbody>
  </table>
