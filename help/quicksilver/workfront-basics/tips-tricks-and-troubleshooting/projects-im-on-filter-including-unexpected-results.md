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
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 许可证</strong></td> 
   <td> <p>[！UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

此 [!UICONTROL **我在处理的项目**] 过滤器包含我预料不到的结果，因为我没有被分派这些项目或与其相关联。

## 解决方案

此 [!UICONTROL **我在处理的项目**] 过滤器包含的项目包含位于其任意位置中的用户。 [!UICONTROL **项目详细信息**] 字段，包括容易错过或自动填写的字段，例如 [!UICONTROL **输入者**] 或 [!UICONTROL **发起人ID**]. 要删除不需要的结果，有两种可能的解决方案：

1. 查看 [!UICONTROL **项目详细信息**] 对于该过滤器包含的每个意外项目，从所有字段中移除您的名称。

   或

1. 尝试使用类似的过滤器，例如 [!UICONTROL **我拥有的项目**]，其中仅包括专门分配给您的项目。

有关在中使用过滤器的更多信息 [!DNL Workfront]，请参见 [过滤器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md).
