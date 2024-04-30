---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: 建立与Workfront数据湖的连接
description: Workfront数据湖允许您通过常用的商业智能工具使用组织的Workfront数据，或将其存储在外部数据仓库中。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 508e3c786bc6cfe676fb2cb33080c99b76c3d6a0
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 1%

---

# 建立与Workfront数据湖的连接

Workfront数据湖允许您通过商业智能工具使用组织的Workfront数据，或将其存储在外部数据仓库中。

要将Workfront列入允许列表数据湖数据与外部产品连接，您必须首先向添加任何必需的IP，如中所述 [将IP添加到允许列表](#add-ips-to-the-allowlist) 下。 此外，大多数产品都需要提供关于您的数据湖的其他信息才能建立连接：

| 字段名称 | 值 |
|---------------|-------------|
| 服务器 | 连接的URL，不带 `https://` 部分(可在 **数据访问** 第页(在Workfront中) |
| 端口 | `443` |
| 数据库 | `WORKFRONT` |
| 仓库 | `READER_WH` |
| 架构 | `WF` |
| 角色 | `READER_ROLE` |
| 用户名 | 创建连接时选择的用户名(可在 **数据访问** 第页(在Workfront中) |
| 密码 | 首次Snowflake登录时选择的密码* |

*有关在何处查找 **数据访问** 包含数据湖连接的页面，请参见 [创建用于Snowflake的Reader（服务）帐户](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>将某个条目添加到IP允许列表后，将不再允许所有其他IP地址。 在尝试使用可视化工具之前，请确保已输入所有必需的IP地址 — 用于可视化工具的构建和读取体验。 否则，您可能会遇到有关无效凭据的错误。

## 将IP添加到允许列表

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **设置**.

1. 在左侧面板中，单击 **系统** > **数据访问**.

1. 单击 **允许的IP** 选项卡，然后单击 **将IP地址添加到允许列表** 按钮。

1. 在中输入IP地址的名称 **IP地址说明** 并输入要在其中使用的工具的IP地址（或CIDR块） **IP地址**，然后单击 **将IP添加到允许列表**.

   ![添加IP地址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 从允许列表中删除IP地址

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **设置**.

1. 在左侧面板中，单击 **系统** > **数据访问**.

1. 单击 **允许的IP** 选项卡，然后单击垃圾桶图标 ![“删除”图标](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 要移除的IP地址的右侧。

1. 在出现的窗口中，选中确认框，然后单击 **删除**.

## 与商业智能工具共享数据

下面列出了许多常见的业务智能工具；这些链接会将您转到服务的文档站点，了解有关连接到数据湖的更多信息。

* [表格](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [多莫](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 将数据存储在外部数据仓库中

下面列出了许多常见的数据仓库；这些链接会将您转到每个服务的文档站点，您可以在其中了解有关连接到数据湖的更多信息。

* [数据库](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
