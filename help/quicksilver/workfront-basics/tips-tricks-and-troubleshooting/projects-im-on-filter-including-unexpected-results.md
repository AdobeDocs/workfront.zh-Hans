---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 我参与的项目过滤器包括意外结果
description: 阅读本文以对我的项目过滤器进行故障排除，包括意外结果。
feature: Get Started with Workfront
author: Nolan
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 1%

---

# 我在处理的项目过滤器包括意外结果

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe[!DNL Workfront]许可证</strong></td> 
   <td> <p>[!UICONTROL 计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[!UICONTROL 系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

我所参与的&#x200B;[!UICONTROL **项目**]&#x200B;筛选器包含我无法预料的结果，因为我没有被分配这些项目或与其关联。

## 解决方案

[!UICONTROL **我参与的项目**]&#x200B;过滤器包括的项目包含位于其任何&#x200B;[!UICONTROL **项目详细信息**]&#x200B;字段中的用户的项目，其中包括容易错过或自动填写的字段，如&#x200B;[!UICONTROL **输入者**]&#x200B;或&#x200B;[!UICONTROL **发起人ID**]。 要删除不需要的结果，有两种可能的解决方案：

1. 检查筛选器包含的每个意外项目的&#x200B;[!UICONTROL **项目详细信息**]，并从所有字段中移除您的名称。

   或

1. 尝试使用类似的过滤器，如&#x200B;[!UICONTROL **我拥有的项目**]，它仅包括专门分配给您的项目。

有关在[!DNL Workfront]中使用筛选器的更多信息，请参阅[筛选器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
