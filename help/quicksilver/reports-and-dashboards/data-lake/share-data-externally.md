---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立与Workfront数据连接的连接
description: Workfront Data Connect允许您将组织的Workfront数据与商业智能工具结合使用，或将其存储在外部数据仓库中。
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 1%

---

# 建立与Workfront数据连接的连接

Workfront Data Connect允许您将组织的Workfront数据与商业智能工具结合使用，或将其存储在外部数据仓库中。

为了将Data Connect数据湖与外部产品连接，您必须首先按照[为Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)创建读取器帐户或连接中的说明创建连接。 然后，必须按照下面[将IP添加到允许列表](#add-ips-to-the-allowlist)中所述将任何必需的IP添加到。

大多数产品都需要提供关于您的数据湖的以下信息才能建立连接：

| 字段名称 | 值 |
|---------------|-------------|
| Server | 无`https://`部分的连接URL（可在Workfront*中的&#x200B;**Data Connect**&#x200B;页面上找到） |
| 端口 | `443` |
| 数据库 | `WORKFRONT` |
| 仓库 | `READER_WH` |
| 架构 | `WF` |
| 角色 | `READER_ROLE` |
| 用户名 | 创建连接时选择的用户名（可在Workfront中的&#x200B;**Data Connect**&#x200B;页面上找到*） |
| 密码 | 首次Snowflake登录时选择的密码* |

*有关在何处查找包含您的连接的&#x200B;**Data Connect**&#x200B;页面的信息，请参阅[为Snowflake创建读取器帐户或连接](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。

>[!IMPORTANT]
>
>将某个条目添加到IP允许列表后，将不再允许所有其他IP地址。 在尝试使用可视化工具之前，请确保已输入所有必需的IP地址 — 用于可视化工具的构建和读取体验。 否则，您可能会遇到有关无效凭据的错误。
>
>如果您的BI工具中未包含任何IP地址，但仍无法连接到BI允许列表，请检查BI工具的代理服务器配置。

## 访问权限要求

+++ 展开以查看访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>Ultimate</p>
    <p>工作流 Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将IP添加到允许列表

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据连接**。

1. 单击“**允许的IP**”选项卡，然后单击“**将IP地址添加到您的”**&#x200B;按钮。

1. 在&#x200B;**IP地址描述**&#x200B;中输入IP地址的名称，然后输入要在&#x200B;**IP地址**&#x200B;中使用的工具的IP地址（或CIDR块），然后单击&#x200B;**将IP添加到中**。

   ![添加IP地址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 查找Microsoft Power BI的Azure IP范围

到Data Connect的Microsoft Power BI流量并非来自单个固定地址。 Microsoft会将IP范围发布为大型JSON文件中的CIDR块。 本节介绍如何查找您实际使用的区域的块。

### Azure IP范围和服务标签的官方Microsoft来源

Microsoft将在[Azure IP范围和服务标签 — 公共云下载页面](https://www.microsoft.com/en-us/download/details.aspx?id=56519)上发布列表。 下载当前JSON文件（文件名通常类似于`ServiceTags_Public_YYYYMMDD.json`）。 当Microsoft更新此文件时，或在Microsoft更改后出现连接问题时，请刷新您的允许列表。

>[!NOTE]
>
>JSON文件非常大，通常远超过100,000行。 这是正常情况。 所需的部分很小；您不需要手动读取整个文件。

### Power BI与Power Query Online

当流量实际来自Power Query组件时，客户有时会报告“Power BI”，而Microsoft会将此类组件视为服务标签列表中的单独Azure服务。

| 如果您的用户…… | 在JSON中查找此服务标签 |
|----------------|---------------------------------------|
| 使用Power BI服务、在Azure中托管的数据集或云上下文中的网关 | `PowerBI` （全局或区域条目，如`PowerBI.EastUS`） |
| 使用Power Query Online、云数据流和类似体验 | `PowerQueryOnline` （全局或区域条目，如`PowerQueryOnline.EastUS`） |

如果贵组织同时使用这两种体验，请为同一地区同时添加`PowerBI`和`PowerQueryOnline`中的CIDR块。 如果仅添加一个，则某些用户可能仍会被阻止，而其他用户可能会成功。

### 选择区域标记，而不是全局聚合

JSON文件包含`PowerBI`的单个全区域条目（对于`PowerQueryOnline`也是如此），该条目聚合了多个区域，可以包含数百个CIDR块，以及许多较小的区域条目，如`PowerBI.WestUS`、`PowerBI.WestUS2`和`PowerBI.WestUS3`。 每个区域对象仅列出该区域的前缀，通常最多几十行。 我们建议不要添加全局条目，除非您有文档记录要求允许每个Azure区域。 对于大多数Data Connect客户，区域条目是正确的默认设置。 添加Power BI租户和用户实际运行的区域，以及小缓冲区作为冗余（例如，公司使用的辅助灾难恢复区域）。

### 选择您的地区

Microsoft在文件中的区域名称类似于`EastUS`、`WestEurope`、`GermanyWestCentral`等。 使用Power BI容量和用户所在的区域，而不是使用您的办公室所在的位置，但它们通常保持一致。

| 场景 | 首先添加什么 |
|----------|-------------------|
| 美国使用情况 | 从您知道租户使用的美国地区开始（示例： `EastUS`、`EastUS2`、`WestUS`、`WestUS2`、`WestUS3`、`CentralUS`、`SouthCentralUS`）。 除非您的Microsoft管理员确认多区域托管，否则您不需要美国每个区域。 |
| 欧盟或英国用法 | 从租户使用的区域开始（示例： `WestEurope`、`NorthEurope`、`FranceCentral`、`GermanyWestCentral`、`SwedenCentral`、`UKSouth`）。 仅当用户跨越其他Microsoft区域时才添加更多。 |
| 亚太地区使用情况 | 添加您的Power BI或Azure管理员确认的区域（示例： `SoutheastAsia`、`EastAsia`、`AustraliaEast`）。 |
| 多个地理位置 | 为每个服务(`PowerBI`和`PowerQueryOnline`（如果都在使用中）)添加两组区域标记（例如，EU和US）。 |
| 未知区域 | 请咨询Microsoft 365或Power BI管理员哪些Azure区域托管您的Power BI资源，或查看Power BI管理员租户设置。 如果必须快速取消阻止以进行测试，请添加一个已知区域对（例如，`EastUS`和`WestUS`）并监视，然后在确认后缩小列表。 |

### 查找IP范围并将它们添加到允许列表

要从Microsoft收集IP范围并将它们添加到Workfront，请执行以下操作：

1. 打开[Azure IP范围和服务标签 — 公共云下载页面](https://www.microsoft.com/en-us/download/details.aspx?id=56519)，下载服务标签JSON文件，并将其保存在本地（例如，`Downloads\ServiceTags_Public_YYYYMMDD.json`）。

1. 在任何能够很好地处理大型JSON的编辑器（如Visual Studio代码）中打开该文件。

1. 使用编辑器的查找功能（ Windows上的`Ctrl+F`或macOS上的`Cmd+F`）查找其`"name"`字段等于服务标签（如`PowerBI.EastUS`或`PowerQueryOnline.WestEurope`）的JSON对象。 有用的搜索：

   * `"name": "PowerBI.WestUS"` — 跳转到美国西部Power BI。
   * `"name": "PowerQueryOnline.WestUS"` — 跳转到West US Power Query Online。
   * `PowerBI.` — 列出所有Power BI区域标记，然后完善到您的区域名称。

1. 在每个匹配对象下，查找名为`addressPrefixes`的数组。 该数组中的每个字符串都是一个CIDR块（例如，`20.59.79.96/27`或IPv6前缀）。 这些是您将添加到Workfront的值。

1. 将每个CIDR添加到Workfront，如本文中的[将IP添加到允许列表](#add-ips-to-the-allowlist)中所述。 如果您的环境缓存规则，请留出几分钟时间进行策略传播。

1. 在Power BI或Power Query Online中，对Data Connect运行小型测试查询以验证连接。 如果失败，请捕获大约的时间，并询问您的网络团队拒绝次数是否与缺少的范围一致。 重新检查在仅添加`PowerBI`时是否错过了`PowerQueryOnline`，这是常见的间隔。

例如，如果Microsoft管理员确认Power BI工作负载使用West US、West US 2和West US 3，并且用户同时使用Power BI和Power Query Online，则您将打开六个对象： `PowerBI.WestUS`、`PowerBI.WestUS2`、`PowerBI.WestUS3`以及每个对象的匹配`PowerQueryOnline.<Region>`，然后从所有六个对象中复制`addressPrefixes`。

### JSON结构引用

从概念上讲，每个服务标签块如下所示。 真实的文件包含更多元数据。

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

`addressPrefixes`数组包含您将添加到Workfront的CIDR块。 其他字段适用于Azure网络场景，此处不适用。

### 保持允许列表

* Microsoft会随着时间的推移更改IP范围。 当Microsoft发布更新的JSON文件时，请定期刷新或比较允许列表，尤其是在发生连接事件后。
* 如果您的环境支持IPv6到Snowflake，并且Microsoft列出了IPv6前缀，如果您的安全策略允许IPv6，请包含这些前缀。 否则，请与您的网络团队协调。

## 从允许列表中删除IP地址

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据连接**。

1. 单击&#x200B;**允许的IP**&#x200B;选项卡，然后单击要删除的IP地址右侧的垃圾桶图标![删除图标](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)。

1. 在出现的窗口中，选中确认框，然后单击&#x200B;**删除**。

## 与商业智能工具共享数据

下面列出了许多常见的业务智能工具；请访问其文档站点以了解有关连接到数据湖的更多信息。

* 表格
* Power BI
* 多莫
* SAP HANA

## 将数据存储在外部数据仓库中

下面列出了许多常见的数据仓库；请访问其文档站点以了解有关连接到数据湖的更多信息。

* 数据块
* AWS Redshift
