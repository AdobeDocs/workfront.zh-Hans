---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Power BI工具无法使用提供的密码进行连接
description: 当您尝试从Power BI工具登录Data Connect时，您会收到一个登录错误。
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Power BI工具无法使用提供的密码进行连接

## 问题

当您尝试从Power BI工具登录Data Connect时，您会看到以下错误：

`Cannot connect from BI tool with provided password`

## 原因

创建JDBC连接时，Workfront会为Data Connect提供临时口令。

在通过Power BI访问Data Connect之前，您必须首先使用提供的连接详细信息登录，更新临时密码，然后继续登录。


## 解决方案

在Workfront中重置连接密码，然后使用在“编辑连接”对话框中提供的链接创建新密码。

### 在Workfront中重置连接密码

1. 转到Workfront >设置>系统>数据连接。
1. 从列表中查找并打开连接。
1. 在&#x200B;**重置连接密码**&#x200B;下，选中方框以确认您要重置密码。
1. 单击&#x200B;**重置连接密码**。
   ![重置连接密码](assets/reset-password.png)
1. 继续下面的部分。

### 为连接创建新密码

1. 复制URL并将其粘贴到新的浏览器选项卡中。
1. 在Workfront中，将连接用户名和默认密码复制并粘贴到新的浏览器选项卡中。
   ![复制url和默认密码](assets/link-password.png)
1. 单击&#x200B;**登录**。
1. 输入新密码，然后单击&#x200B;**提交**。
1. 转到Power BI工具，然后使用新密码登录。

