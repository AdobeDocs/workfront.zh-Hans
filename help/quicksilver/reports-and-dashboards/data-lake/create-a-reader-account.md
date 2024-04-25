---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: 创建用于Snowflake的Reader（服务）帐户
description: 要访问Workfront数据湖中的数据，您必须首先为Snowflake创建读取器帐户。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# 创建用于Snowflake的Reader（服务）帐户

要访问Workfront数据湖数据，您必须首先为每个新连接创建一个Snowflake读取器（或服务）帐户。 创建连接后，您可以通过单击 **数据访问** 页面(**主菜单** > **设置** > **系统** > **数据访问**)下 **现有连接** 选项卡。

有关将新创建的连接与外部产品配合使用的信息，请参阅 [建立与Workfront数据湖的连接](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>待定</td> 
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

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 创建读者帐户

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **设置**.

1. 在左侧面板中，单击 **系统** > **数据访问**.

1. 单击 **创建新连接**

1. 在出现的窗口中，输入连接的名称 **连接引用说明** 和中的用户名 **连接用户**，然后单击 **生成连接**.

   ![创建读者帐户](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **默认密码** 将生成，以及可通过Snowflake查看您的数据的URL。 您需要将密码与您选择用于首次Snowflake的用户名结合使用，因此请确保同时记录该密码和URL。 选中声明已完成的框，然后单击 **关闭**.

   ![默认帐户密码](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. 使用浏览器打开Snowflake以导航到上一步骤中的URL，输入您选择的用户名和上一步骤中的默认密码，然后单击 **登录**.

1. 首次成功登录后，系统将提示您选择新密码。 输入您选择的密码，输入 **新密码** 和 **确认密码** 字段，然后单击 **提交**.

   ![重置Snowflake密码](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. 您现在可以使用用户名和新密码访问Snowflake中的Workfront数据湖或您选择的业务可视化工具。

## 撤销读取者帐户

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **设置**.

1. 在左侧面板中，单击 **系统** > **数据访问**.

1. 单击垃圾桶图标 ![“删除”图标](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 要撤销的帐户的右侧。

1. 在出现的窗口中，选中确认框，然后单击 **删除**.
