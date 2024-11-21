---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: 建立与Workfront数据连接的连接
description: Workfront Data Connect允许您将组织的Workfront数据与商业智能工具结合使用，或将其存储在外部数据仓库中。
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 7b50876f1be16473704eddeb3157dacfacd96e90
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 1%

---

# 建立与Workfront数据连接的连接

Workfront Data Connect允许您将组织的Workfront数据与商业智能工具结合使用，或将其存储在外部数据仓库中。

为了将Data Connect数据湖与外部产品连接，您必须首先按照[为Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)创建读取器帐户或连接中的说明创建连接。 然后，必须按照下面[将IP添加到允许列表 列入允许列表](#add-ips-to-the-allowlist)中所述将任何必需的IP添加到。

大多数产品都需要提供关于您的数据湖的以下信息才能建立连接：

| 字段名称 | 值 |
|---------------|-------------|
| 服务器 | 无`https://`部分的连接URL(可在Workfront*中的&#x200B;**Data Connect**&#x200B;页面上找到) |
| 端口 | `443` |
| 数据库 | `WORKFRONT` |
| 仓库 | `READER_WH` |
| 模式 | `WF` |
| 角色 | `READER_ROLE` |
| 用户名 | 创建连接时选择的用户名(可在Workfront中的&#x200B;**Data Connect**&#x200B;页面上找到*) |
| 密码 | 首次Snowflake登录时选择的密码* |

*有关在何处查找包含您的连接的&#x200B;**Data Connect**&#x200B;页面的信息，请参阅[为Snowflake创建读取器帐户或连接](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)。

>[!IMPORTANT]
>
>将某个条目添加到IP允许列表后，将不再允许所有其他IP地址。 在尝试使用可视化工具之前，请确保已输入所有必需的IP地址 — 用于可视化工具的构建和读取体验。 否则，您可能会遇到有关无效凭据的错误。
>
>如果您的BI工具中未包含任何IP地址，但仍无法连接到BI允许列表，请检查BI工具的代理服务器配置。

## 访问要求

+++ 展开以查看访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td><p>包括在以下计划中：</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>可作为以下计划的附加组件购买：</p> 
    <ul>
        <li>选择</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect不适用于旧版Workfront计划。</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将IP添加到允许列表

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据连接**。

1. 列入允许列表单击“**允许的IP**”选项卡，然后单击“**将IP地址添加到您的”**&#x200B;按钮。

1. 列入允许列表在&#x200B;**IP地址描述**&#x200B;中输入IP地址的名称，然后输入要在&#x200B;**IP地址**&#x200B;中使用的工具的IP地址（或CIDR块），然后单击&#x200B;**将IP添加到中**。

   ![添加IP地址](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

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

* 数据库
* AWS Redshift
