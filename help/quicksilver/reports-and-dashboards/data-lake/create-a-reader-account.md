---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: 为Snowflake创建读取器帐户
description: 要访问Data Connect数据，您必须首先创建一个Snowflake读取器帐户。
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# 为Snowflake创建Reader帐户或连接

要访问Data Connect数据，您必须首先为贵组织创建Snowflake读取器（或服务）帐户，然后为要访问Data Connect的每个用户或工具创建新连接。

创建连接后，您可以在&#x200B;**现有连接**&#x200B;选项卡下的&#x200B;**Data Connect**&#x200B;页面（**主菜单** > **设置** > **系统** > **Data Connect**）上单击该连接，找到其关联的URL和用户名。

有关将新创建的连接与外部产品结合使用的信息，请参阅[建立与Workfront Data Connect的连接](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md)。

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
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect不适用于旧版Workfront计划。</p> 
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建读者帐户

在开始创建连接之前，必须为您的组织创建新的Snowflake读取器帐户。

>[!IMPORTANT]
>
>每个组织只需完成此流程一次。 如果&#x200B;**创建Reader帐户**&#x200B;按钮不存在于下面描述的位置，则表示已创建您的读者帐户。

要创建读取器帐户，请执行以下操作：

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据连接**。

1. 单击&#x200B;**创建Reader帐户**&#x200B;按钮开始创建贵组织的读者帐户。 该过程是自动的，但可能需要几分钟才能完成。

1. 完成后，将显示一个对话框窗口，说明您的阅读器帐户现在处于活动状态。 刷新浏览器页面以获得对&#x200B;**新建连接**&#x200B;按钮的访问权限。

![Reader帐户创建的对话框](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## 创建连接

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据连接**。

1. 单击&#x200B;**新建连接**

1. 在出现的窗口中，在&#x200B;**连接引用描述**&#x200B;中输入连接名称，在&#x200B;**连接用户**&#x200B;中输入用户名，然后单击&#x200B;**生成连接**。

   ![创建新连接](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. 将生成&#x200B;**默认密码**&#x200B;以及可通过Snowflake查看您的数据的URL。 您需要将密码与您选择用于首次登录Snowflake的用户名结合使用，因此请确保同时记录该密码和URL。 选中声明已完成此操作的框，然后单击&#x200B;**关闭**。

   ![默认帐户密码](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. 使用浏览器打开Snowflake以导航到上一步的URL，输入您选择的用户名和上一步的默认密码，然后单击&#x200B;**登录**。

1. 首次成功登录后，系统将提示您选择新密码。 在&#x200B;**新密码**&#x200B;和&#x200B;**确认密码**&#x200B;字段中输入您选择的密码，然后单击&#x200B;**提交**。

   ![重置Snowflake密码](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. 您现在可以使用用户名和新密码访问Snowflake中的Data Connect数据湖或您选择的业务可视化工具。

## 撤销读取者帐户

1. 单击Adobe Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon.png)，或（如果可用）单击左上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png)，然后单击&#x200B;**设置**。

1. 在左侧面板中，单击&#x200B;**系统** > **数据访问**。

1. 单击要撤销的帐户右侧的垃圾桶图标![删除图标](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)。

1. 在出现的窗口中，选中确认框，然后单击&#x200B;**删除**。
