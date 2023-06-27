---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Anaplan模块
description: 在 [!DNL Adobe Workfront Fusion] 场景中，您可以自动执行使用Anaplan的工作流，并将其连接到多个第三方应用程序和服务。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 1%

---

# [!DNL Anaplan] 模块

在 [!DNL Adobe Workfront Fusion] 场景，您可以自动执行使用 [!DNL Anaplan]，并将其连接到多个第三方应用程序和服务。

如果您需要有关创建方案的说明，请参阅 [在中创建方案 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

有关模块的信息，请参见 [中的模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## 先决条件

在使用 [!DNL Anaplan] 连接器时，必须确保满足以下先决条件：

* 您必须拥有有效的 [!UICONTROL Anaplan] 帐户。
* 必须配置工作区、模型及其他 [!DNL Anaplan] 中的对象 [!UICONTROL Anaplan] 之前的帐户 [!DNL Workfront Fusion] 可以和他们互动。

## Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

为创建连接 [!DNL Anaplan] 模块：

1. 单击 **[!UICONTROL 添加]** 旁边的 [!UICONTROL 连接] 盒子。
1. 选择连接类型。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [！UICONTROL Basic]</td> 
      <td> <p>An [!DNL Anaplan] [！UICONTROL Basic]连接只需要电子邮件地址和密码即可创建连接。 </p> <p>输入连接名称，然后输入您的电子邮件地址和密码 [!DNL Anaplan] 帐户。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [！UICONTROL CA证书]</td> 
      <td> <p>An [!DNL Anaplan] [！UICONTROL CA Certificate]连接需要[！UICONTROL证书密钥]、[！UICONTROL编码数据]和[！UICONTROL编码签名数据]。 您可以在以下位置生成这些 [!DNL Anaplan] 帐户。 有关说明，请参阅 [!DNL Anaplan] 文档。</p> <p>输入连接名称，然后输入您在中生成的[！UICONTROL证书密钥]、[！UICONTROL编码数据]和[！UICONTROL编码签名数据] [!DNL Anaplan] 帐户。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 继续]** 以保存连接并返回到模块。

## [!DNL Anaplan] 模块及其字段

配置时 [!DNL Anaplan] 模块， [!DNL Workfront Fusion] 显示下面列出的字段。 除此以外，还有 [!DNL Anaplan] 可能会显示字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关更多信息，请参阅 [在中将信息从一个模块映射到另一个模块 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [触发器](#triggers)
* [操作](#actions)
* [搜索](#searches)

### 触发器

#### [!DNL Watch records]

此触发器模块在创建或更新所选类型的记录时启动方案。

>[!NOTE]
>
>此模块返回新记录的数据。 它不会返回修改后的现有记录的数据。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">要观看的对象类型</td> 
   <td>选择要监视的项目类型。 当创建或更新此类型的记录时，方案即开始。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>在Anaplan中输入与要监视的对象相关联的对象ID，例如模型或模块</td> 
  </tr> 
  <tr> 
   <td role="rowheader">限制</td> 
   <td> <p>在每个方案执行周期中，输入或映射您希望模块记录的最大数量[action]。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 操作

* [[!UICONTROL 创建列表项]](#create-a-list-item)
* [[!UICONTROL 进行自定义API调用]](#make-a-custom-api-call)
* [[!UICONTROL 读取记录]](#read-a-record)
* [[!UICONTROL 运行操作]](#run-an-action)
* [[!UICONTROL 更新记录]](#update-a-record)
* [[!UICONTROL 上传文件]](#upload-a-file)

#### [!UICONTROL 创建列表项]

此操作模块向Anaplan中的列表添加新项。

<table style="table-layout:auto">
    <tr>
        <td>[！UICONTROL连接]</td>
        <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td>
    </tr>
    <tr>
        <td>[！UICONTROL工作区ID]</td>
        <td>选择或映射包含要添加项目的列表的Anaplan Workspace的ID。</td>
    </tr>
    <tr>
        <td>[！UICONTROL模型ID]</td>
        <td>选择或映射包含要添加项目的列表的模型的ID。</td>
    </tr>
    <tr>
        <td>[！UICONTROL列表ID]</td>
        <td>选择或映射要在其中创建项目的列表的ID。</td>
    </tr>
    <tr>
        <td>[！UICONTROL名称]</td>
        <td>输入新项目的名称。</td>
    </tr>
    <tr>
        <td>[！UICONTROL代码]</td>
        <td>输入新项目的代码。 代码是用户生成的代码，可用于区分具有相同名称的行项目。</td>
    </tr>
    <tr>
        <td>[！UICONTROL Parent]</td>
        <td>输入要在其下创建新项目的父项目的名称。</td>
    </tr>
    <tr>
        <td>[！UICONTROL属性]</td>
        <td>如果要将项目添加到的列表具有自定义属性，请选择要为其添加值的属性，然后添加值。</td>
    </tr>
    <tr>
        <td>[！UICONTROL子集]</td>
        <td>如果要将项目添加到的列表具有自定义子集，请选择要将该项目添加到的子集，然后选择 <b>[！UICONTROL是]</b> 将新项添加到该子集。</td>
    </tr>
</table>

#### [!UICONTROL 进行自定义API调用]

利用此模块，可对 [!DNL Anaplan] API。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL URL]</p> </td> 
   <td> <p>输入相对路径 <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL方法]</p> </td> 
   <td> <p>选择配置API调用所需的HTTP请求方法。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">中的HTTP请求方法 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL标头]</td> 
   <td> <p>以标准JSON对象的形式添加请求的标头。</p> <p>例如， <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 自动添加授权标头。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL查询字符串] </td> 
   <td> <p>输入请求查询字符串。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL主体]</td> 
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注释:  <p>使用条件语句(例如 <code>if</code> 在JSON中，将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 删除记录]

此操作模块删除现有记录。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL工作区ID]</td> 
   <td>选择或映射包含要删除的对象的Anaplan工作区的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL模型ID]</td> 
   <td>输入或映射包含要删除对象的模型的ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">删除</td> 
   <td> <p>选择要删除的对象类型。</p> 
    <ul> 
     <li> <p><b>操作</b> </p> <p>选择或映射要删除的操作。</p> </li> 
     <li> <p><b>列表项</b> </p> <p>选择要从中删除项目的列表，然后输入或映射要删除的项目的ID或代码</p>  </li> 
     <li> <p><b>[！UICONTROL文件]</b> </p> <p>选择或映射要删除的文件。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 读取记录]

该操作模块读取单个记录。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要读取的记录类型。</p> 
    <ul> 
     <li> <p><b>模型</b> </p> <p>选择或映射要读取的模型的ID</p> </li> 
     <li> <p><b>模型列表</b> </p> <p>选择或映射包含要读取的列表的工作区和模型的ID，然后选择列表。 在[！UICONTROL数据类型]字段中，选择要读取数据还是元数据。</p> </li> 
     <li> <p><b>模型版本</b> </p> <p>选择或映射要读取的模型的ID。</p> </li> 
     <li> <p><b>用户</b> </p> <p>选择是要返回有关正在使用的帐户的所有者的数据，还是要返回其他用户的数据。 如果选择另一个用户，请选择该用户的名称。</p> </li> 
     <li> <p><b>Workspace</b> </p> <p>选择或映射您要读取的工作区的ID。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 运行操作]

此操作模块可导入、导出、删除或处理一项操作。

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[！UICONTROL连接]</td>
        <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#Connect" class="MCXref xref" >[！UICONTROL Connect Anaplan到Workfront Fusion]</a> 本文章中。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL工作区ID]</td>
        <td>选择或映射 [!DNL Anaplan] 要在其中执行操作的工作区</td>
      </tr>
      <tr >
        <td role="rowheader">[！UICONTROL模型ID]</td>
        <td>选择或映射要执行操作的模型的ID。</td>
      </tr>
      <tr>
        <td role="rowheader">[！UICONTROL操作类型]</td>
        <td>
          <p>选择要执行的操作</p>
            <ul>
              <li>
                <p><b>[！UICONTROL Delete]</b>
                </p>
                <p>输入或映射要删除的操作的ID。</p>
              </li>
              <li>
                <p><b>[！UICONTROL导出]</b>
                </p>
                <p>输入或映射要使用的导出定义的ID。 可导出为以下文件格式：</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[！UICONTROL导入] </b>
                  </p>
                  <p style="font-weight: normal;">输入或映射要使用的导入定义的ID。</p>
                </li>
                <li>
                 <p><b>[！UICONTROL进程]</b>
                 </p>
                  <p>输入或映射要使用的进程的ID。 </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL 更新记录]

此操作模块更新中的单个记录 [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要更新的记录类型。</p> 
    <ul> 
     <li> <p><b>[！UICONTROL列表项]</b> </p> <p>有关字段，请参阅 <a href="#create-a-list-item" class="MCXref xref">创建列表项</a> 本文章中。</p> </li> 
     <li> <p><b>[！UICONTROL模块单元格数据]</b> </p> <p>更新单元格数据时，使用该数据的所有下游计算也会更新。</p> <p>填写以下字段：</p> 
      <ul> 
       <li> <p><b>[！UICONTROL模型ID]</b> </p> <p>选择或映射包含要更新的单元格的模型。</p> </li> 
       <li> <p><b>[！UICONTROL模块ID]</b> </p> <p>选择或映射包含要更新的单元格的模块</p> </li> 
       <li> <p><b>[！UICONTROL行项目名称]</b> </p> <p>选择或映射要更新的单元格的行项</p> </li> 
       <li> <p style="font-weight: bold;">[！UICONTROLDimensionID]</p> <p>选择或映射行项目上的维度。</p> 
       <p><b>注释: </b> 
       <ul>
       <li> Dimension键（值）必须为 <code>dimensionName</code> （下一个）或 <code>dimensionId</code> (ID)。</li>
       <li>项目键（值）必须为 <code>itemName</code> （文本）， <code>itemCode</code> （文本），或 <code>itemId</code> (ID)。</li>
       <li>Dimension和项目键必须属于相同类型（文本或ID）。
       </ul>
        </p> 
        <p>Dimension有关维度的信息，请在 [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[！UICONTROL值]</b> </p> <p>输入或映射单元格的新值。</p> </li> 
      </ul> </li> 
     <li> <p><b>[！UICONTROL模型当前会计年度]</b> </p> <p>输入要更新其会计年度的模型的工作区ID和模型ID，然后为模型输入或映射新年份。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 上传文件]

此操作模块将文件上传到Anaplan。 该文件必须已上传到Anaplan。 您可以使用此模块将其上传到Anaplan中的其他位置。
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[！UICONTROL连接]</td>
<td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td>
</tr>
<tr>
<td role="rowheader">[！UICONTROL工作区ID]</td>
<td>选择或映射 [!DNL Anaplan] 要在其中上传文件的工作区。</td>
</tr>
<tr>
<td role="rowheader">[！UICONTROL模型ID]</td>
<td>选择或映射要上传文件的模型的ID。</td>
</tr>
<tr>
<td role="rowheader">[！UICONTROL文件ID]</td>
<td>选择或映射要上传的文件的ID。</td>
</tr>
</tbody>
</table>
</div>

### 搜索

#### [!UICONTROL 获取记录]

此搜索模块返回所选类型的所有可访问记录。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[！UICONTROL连接]</td> 
   <td>有关创建与的连接 [!DNL Anaplan]，请参见 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Connect [!DNL Anaplan] 到 [!DNL Workfront Fusion]</a> 本文章中。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL记录类型]</td> 
   <td> <p>选择要检索的记录类型。</p> 
      <ul> 
       <li> <p><b>[！UICONTROL工作区]</b> </p> </li> 
       <li> <p><b>[！UICONTROL模型]</b> </p> </li> 
       <li> <p><b>[！UICONTROL行项目]</b> </p> <p>选择或映射包含 [!DNL line] 要检索的项目。</p> </li> 
       <li> <p><b>[！UICONTROL模型列表]</b> </p> <p>选择或映射包含要检索的模型列表的工作区ID和模型ID。</p> </li> 
       <li> <p><b>[！UICONTROL模型日历]</b> </p> <p>选择或映射包含要检索的模型日历的工作区的ID。</p> </li> 
       <li> <p><b>模型版本</b> </p> </li> 
       <li> <p>选择或映射[！UICONTROL ]包含要检索的模型版本的模型ID。</p> </li> 
       <li> <p><b>[！UICONTROL用户]</b> </p> </li> 
       <li> <p><b>[！UICONTROL视图]</b> </p> <p>选择是要按模块还是按模型选择视图，然后选择或映射包含要检索的视图的模块或模型的ID。</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL返回工作区大小]</td> 
   <td>启用此选项可返回工作区的当前大小的估计值。 此估算基于工作区中包含的所有模块的大小。</td> 
  </tr> 
 </tbody> 
</table>
