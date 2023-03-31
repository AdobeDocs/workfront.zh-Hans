---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 我正在筛选的项目，包括意外结果
description: 请阅读本文以对“我所在的项目”筛选器进行故障诊断，包括意外结果。
feature: Get Started with Workfront
author: Nolan
source-git-commit: 5a4c98f9ce6bb7eb936a0b24b634d2545a0f13ee
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 1%

---

# “我所在的项目”筛选器包含意外结果

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 许可证</strong></td> 
   <td> <p>[!UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[!UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 问题

的 [!UICONTROL **我正在执行的项目**] 过滤器包含我预期不到的结果，因为我没有被分配或与这些项目关联。

## 解决方案

的 [!UICONTROL **我正在执行的项目**] 过滤器包含包含其任何 [!UICONTROL **项目详细信息**] 字段，包括容易遗漏或自动填充的字段，如 [!UICONTROL **输入者**] 或 [!UICONTROL **赞助商ID**]. 要删除不需要的结果，可能有两种解决方案：

1. 检查 [!UICONTROL **项目详细信息**] 对于过滤器包含的每个意外项目，请从所有字段中删除您的名称。

或

1. 尝试使用类似的过滤器，例如 [!UICONTROL **我拥有的项目**]，其中仅包括专门分配给您的项目。

有关在 [!DNL Workfront]，请参阅 [过滤器概述 [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)