---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: “运行报告时的错误消息：‘您当前未登录。’”
description: 了解“您当前未登录”错误消息。
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 1%

---

# 运行报告时的错误消息：“您当前未登录。”

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划、工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

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
