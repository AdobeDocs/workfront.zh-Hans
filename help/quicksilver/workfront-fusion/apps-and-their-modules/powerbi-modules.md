---
filename: powerbi-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Power BI模块
description: 除了Adobe Workfront许可证之外，Adobe Workfront Fusion还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: 01405f5f-6821-4c38-b34c-373922f63004
source-git-commit: 8dbb29b297d4f8840d5ecb81f819e89b5325f62c
workflow-type: tm+mt
source-wordcount: '2471'
ht-degree: 0%

---

# [!DNL Power BI]模块

[!DNL Power BI]是一个应用程序，它允许您可视化数据并向利益相关者展示数据。 它可以获取来自各种来源的数据。

>[!NOTE]
>
>[!DNL Workfront Fusion]不是数据源。 虽然[!DNL Workfront Fusion]可以创建和使用数据源，但它不会存储您的数据。


## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!DNL Plan]， [!DNL Work]</p> </td> 
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

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

&#42;&#42;有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## [!DNL Power BI]模块及其字段

配置[!DNL Power BI]时，[!DNL Workfront Fusion]显示下面列出的字段。 除此以外，还可能会显示其他字段，具体取决于应用程序或服务中的访问级别等因素。 模块中的粗体标题表示必填字段。

如果看到字段或函数上方的映射按钮，则可以使用该按钮设置该字段的变量和函数。 有关详细信息，请参阅[在Adobe Workfront Fusion中将信息从一个模块映射到另一个模块](../../workfront-fusion/mapping/map-information-between-modules.md)。

![](assets/map-toggle-350x74.png)

* [仪表板](#dashboards)
* [报告](#reports)
* [数据集](#dataset)
* [应用程序](#apps)
* [其他](#other)

### 仪表板

* [创建功能板](#create-a-dashboard)
* [获取功能板](#get-a-dashboard)
* [获取功能板拼贴](#get-a-dashboard-tile)
* [列出功能板磁贴](#list-dashboard-tiles)
* [列出仪表板](#list-dashboards)

#### [!UICONTROL 创建仪表板]

此操作模块将创建一个新仪表板。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
      <td>输入或映射功能板的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射将拥有新功能板的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取仪表板]

此操作模块检索指定功能板的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入功能板ID]</td>
      <td>
        <p>选择或映射选项以选择要为其检索元数据的仪表板。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL功能板ID]</td>
      <td>
        <p>输入或映射要为其检索元数据的仪表板的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有您要为其检索元数据的功能板的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取仪表板磁贴]

此操作模块可检索指定功能板拼贴的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入功能板ID]</td>
      <td>
        <p>选择或映射选项以选择要检索的仪表板详细信息。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL功能板ID]</td>
      <td>
        <p>输入或映射要检索其详细信息的仪表板的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL拼贴ID]</td>
      <td>输入或映射要检索其详细信息的[!DNL Power BI]拼贴的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有您要检索的拼贴的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出仪表板磁贴]

此搜索模块可检索功能板磁贴的列表。

<table>
<col/>
<col/>
<tbody>
  <tr>
    <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL输入功能板ID]</td>
    <td>
      <p>选择或映射选项以选择要列出其图块的仪表板。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL功能板ID]</td>
    <td>
      <p>输入或映射包含要列出的图块的仪表板的ID。</p>
    </td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL组ID]  </td>
    <td>选择或映射拥有包含要列出的图块的仪表板的组的ID。</td>
  </tr>
  <tr>
    <td role="rowheader">[！UICONTROL限制]  </td>
    <td>
      <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
    </td>
  </tr>
</tbody>
</table>

#### [!UICONTROL 列出仪表板]

此搜索模块可检索功能板列表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>
        <p>选择或映射拥有要列出的功能板的组的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
      </td>
    </tr>
  </tbody>
</table>

### 报告

* [复制报告](#copy-a-report)
* [删除报告](#delete-a-report)
* [获取报表](#get-a-report)
* [列表报告](#list-reports)

#### [!UICONTROL 复制报告]

此操作模块复制现有报表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入报表ID]</td>
      <td>
        <p>选择或映射选项以选择要复制的报表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>输入或映射要复制的报表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有要复制的报表的组的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL新复制的报表名称]</td>
      <td>输入或映射新报表的名称。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 删除报告]

此操作模块删除报表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入报表ID]</td>
      <td>
        <p>选择或映射选项以选择要删除的报表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>输入或映射要删除的报表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有要删除的报表的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取报表]

此操作模块检索指定报表的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入报表ID]</td>
      <td>
        <p>选择或映射选项以选择要为其检索元数据的报表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>输入或映射要为其检索元数据的报表的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有您要为其检索元数据的报表的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出报告]

此搜索模块可检索报告列表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>
        <p>选择或映射拥有要列出的报告的组的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
      </td>
    </tr>
  </tbody>
</table>


### 数据集

* [在数据集表中添加/删除行](#add-or-delete-rows-in-a-dataset-table)
* [创建数据集](#create-a-dataset)
* [删除数据集](#delete-a-dataset)
* [获取数据集](#get-a-dataset)
* [列出数据集](#list-datasets)
* [刷新数据集](#refresh-a-dataset)

#### [!UICONTROL 在数据集表中添加或删除行]

此操作模块添加或删除指定推送数据集表的行。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入表]</td>
      <td>选择或映射选项以选择包含要调整的表的数据集。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL数据集ID]</td>
      <td>输入或映射包含要添加或删除的行的数据集的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL表名称]  </td>
      <td>
        <p>输入或映射包含要添加或删除的行的表的名称。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>输入或映射拥有数据集的组的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL选择操作]</td>
      <td>
        <p>选择或映射要执行的操作。</p>
        <ul>
          <li>
            <p>[！UICONTROL添加行]</p>
          </li>
          <li>
            <p>[！UICONTROL Delete All Rows]</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL行]</td>
      <td>
        <p>添加行字段。</p>
        <ul>
          <li>
            <p><b>[！UICONTROL键]</b>
            </p>
            <p>输入或映射密钥名称。</p>
          </li>
          <li>
            <p><b>[！UICONTROL字段类型]</b>
            </p>
            <p>选择或映射字段类型：</p>
            <ul>
              <li>
                <p>布尔型</p>
              </li>
              <li>
                <p>日期</p>
              </li>
              <li>
                <p>文本</p>
              </li>
              <li>
                <p>数字</p>
              </li>
            </ul>
          </li>
          <li>
            <p>[！UICONTROL值]</p>
            <p>输入或映射键值。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 创建数据集]

此操作模块将创建新数据集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
      <td>输入或映射数据集的名称。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射将拥有新数据集的组的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL默认模式]</td>
      <td>
        <p>选择或映射数据集的默认模式：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL As Azure]</b>：与有实时连接的数据集 [!DNL Azure Analysis Service]</p>
          </li>
          <li>
            <p><b>[！UICONTROL As on Prem]</b>：与[!DNL On-premise Analysis]服务有实时连接的数据集</p>
          </li>
          <li>
            <p><b>[!DNL Push]</b>：允许以编程方式访问将数据推入的数据集 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Push Streaming]</b>：支持数据流式传输并允许以编程方式访问将数据推入的数据集 [!DNL Power BI]</p>
          </li>
          <li>
            <p><b>[!DNL Streaming]</b>：支持数据流的数据集</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Tables]</td>
      <td>向数据集添加表。 有关字段，请参阅<a href="#Table" class="MCXref_0">表字段</a></td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Data sources]</td>
      <td>添加数据源。 有关字段，请参阅<a href="#Data" class="MCXref_0">数据源字段</a>。</td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Default Retention Policy]  </td>
      <td>
        <p>选择或映射数据集的有意策略：</p>
        <ul>
          <li>
            <p>[！UICONTROL无]</p>
          </li>
          <li>
            <p>[！UICONTROL基本FIFO]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

##### 表格字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL名称]</td>
      <td>
        <p>  输入或映射表的名称。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL列]</td>
      <td>
        <p>添加列：</p>
        <ul>
          <li>
            <p><b>[！UICONTROL名称]</b>
            </p>
            <p>输入（映射）列名。</p>
          </li>
          <li>
            <p><b>[！UICONTROL数据类型]</b>
            </p>
            <p>选择或映射数据类型：</p>
            <ul>
              <li>
                <p>[！UICONTROL字符串]</p>
              </li>
              <li>
                <p>[！UICONTROL整数]</p>
              </li>
              <li>
                <p>[！UICONTROL Boolean]</p>
              </li>
              <li>
                <p>[！UICONTROL日期时间]</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>[！UICONTROL格式字符串]</b>
            </p>
            <p>输入（映射）格式字符串。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL行]</td>
      <td>输入或映射行详细信息。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Measures]</td>
      <td>为表添加度量。</td>
    </tr>
  </tbody>
</table>

##### 数据源字段

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL数据库]  </td>
      <td>
        <p>输入或映射要使用的数据库。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Server]  </td>
      <td>
        <p>输入或映射要使用的服务器的名称。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL URL]  </td>
      <td>
        <p>输入或映射要使用的URL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL数据源ID]</td>
      <td>
        <p>  输入或映射数据源的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL数据源类型]  </td>
      <td>
        <p>选择或映射数据源类型。 示例： SQL。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL网关ID]  </td>
      <td>输入或映射要使用的网关ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 删除数据集]

此操作模块删除数据集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入报表ID]</td>
      <td>
        <p>选择或映射选项以选择要删除的数据集。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>输入或映射要删除的数据集的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有要删除的数据集的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取数据集]

此操作模块检索指定数据集的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入报表ID]</td>
      <td>
        <p>选择或映射选项以选择要为其检索元数据的报表。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>输入或映射要为其检索元数据的数据集的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有要为其检索元数据的数据集的组的ID。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出数据集]

此搜索模块可检索数据集列表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>选择或映射拥有您要为其检索元数据的报表的组的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]</td>
      <td>
        <p>在每个方案执行周期中，输入或映射您希望模块记录的最大数目，即[action]。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 刷新数据集]

此操作模块刷新指定的数据集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL输入数据集]</td>
      <td>选择或映射选项以选择要刷新的数据集。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL数据集ID]</td>
      <td>输入或映射要刷新的数据集的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL表名称]  </td>
      <td>
        <p>输入或映射包含要添加或删除的行的表的名称。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL组ID]  </td>
      <td>输入或映射拥有数据集的组的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Notify选项]  </td>
      <td>
        <p>选择或映射要通知的选项：</p>
        <ul>
          <li>
            <p>[！UICONTROL Mail On Completion]</p>
          </li>
          <li>
            <p>[！UICONTROL失败时发送邮件]</p>
          </li>
          <li>
            <p>[！UICONTROL无通知]</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 应用程序

* [获取应用程序](#get-an-app)
* [获取应用程序仪表板](#get-an-apps-dashboard)
* [获取应用程序的报表](#get-an-apps-report)
* [列出应用程序的控制面板](#list-apps-dashboards)
* [列出应用程序的报表](#list-apps-reports)
* [列出应用程序](#list-apps)
* [Watch应用程序](#watch-apps)

#### [!UICONTROL 获取应用]

此操作模块可检索指定应用程序的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL应用程序ID]  </td>
      <td>
        <p>选择或映射您要检索的应用程序的ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取应用程序的仪表板]

此操作模块可检索指定应用程序功能板的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL应用程序ID]  </td>
      <td>
        <p>选择或映射包含要检索的功能板的应用程序的ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>  选择或映射要检索的仪表板ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 获取应用的报告]

此操作模块检索指定应用程序报表的元数据。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL应用程序ID]  </td>
      <td>
        <p>选择或映射包含要检索的报表的应用程序ID。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL报表ID]</td>
      <td>
        <p>  选择或映射要检索的报表的ID。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出应用]

此搜索模块可检索已安装的所有应用程序的列表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出应用的控制面板]

此搜索模块从指定的应用程序中检索功能板列表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL应用程序ID]</td>
      <td>选择或映射您要从中列出功能板的应用程序的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 列出应用的报告]

此搜索模块从指定的应用程序中检索所有报表的列表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL应用程序ID]</td>
      <td>选择或映射要从中列出报表的应用程序的ID。</td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 观看应用]

此触发器模块会在应用程序更新时启动方案。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL限制]  </td>
      <td>
        <p>输入或映射您希望模块在每个方案执行周期内返回的最大记录数。</p>
      </td>
    </tr>
  </tbody>
</table>

### 其他

#### [!UICONTROL 进行API调用]

此操作模块对[!DNL Power BI] API执行API调用。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[！UICONTROL Connection]</td>
   <td> <p>有关将[!DNL Power BI]帐户连接到[!DNL Workfront Fusion]的说明，请参阅<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">创建与Adobe[!DNL Workfront Fusion]的连接 — 基本说明</a></p> </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL路径]</p>
      </td>
      <td>
        <p>输入相对于<code>https://api.powerbi.com</code>的路径。 示例： <code>/v1.0/myorg/datasets</code>。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[！UICONTROL方法]</p>
      </td>
      <td>
        <p>选择配置API调用所需的[！UICONTROL HTTP]请求方法。 有关更多信息，请参阅[！UICONTROL HTTP]请求方法。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[！UICONTROL Headers]</td>
      <td>
        <p>以标准JSON对象的形式添加请求的标头。</p>
        <p>例如， <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 自动添加授权标头和x-api-key标头。</p>
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
   <td> <p>以标准JSON对象的形式添加API调用的正文内容。</p> <p>注意：  <p>在JSON中使用条件语句（如<code>if</code>）时，请将引号放在条件语句之外。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
