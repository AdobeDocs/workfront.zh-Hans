---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 运行报告时的错误消息：“您当前未登录。”
description: 了解“您当前未登录”错误消息。
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 13%

---

# 运行报告时的错误消息：“您当前未登录。”

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> 
     <p>标准</p>
     <p>工作版或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 问题

运行报表或在仪表板中显示报表时，会返回以下错误：\
*让我们再试一次。您当前未登录。*

报告中不显示任何结果。

## 原因

报告当前设置为以已停用用户身份运行。

## 解决方案

您必须具有报表的管理权限才能更改报表设置。\
要调整报表并查看结果，请执行以下操作：

1. 转到报告。
1. 单击&#x200B;**报告操作** > **编辑** > **报告设置**。

1. 在&#x200B;**运行此报告的“访问权限：**”字段中指定活动用户的名称。\
   或\
   将&#x200B;**Run this report with the Access Rights of：**&#x200B;字段保留为空。

1. 单击&#x200B;**完成**。
1. 单击&#x200B;**保存+关闭**。\
   运行此报告时，不应再次出现此错误。
