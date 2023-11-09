---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: “日历上的错误消息：‘此日历拥有已停用用户的查看权限。’”
description: 了解“此日历具有查看已停用用户的权限”错误消息。
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 5%

---

# 日历上的错误消息：“此日历具有已停用用户的查看权限。”

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
   <td> <p>编辑对报告、功能板和日历的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对日历的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 问题

在访问与您共享的日历时，您会收到以下错误： 

*此日历具有查看已停用的用户的权限。请让管理员修复该日历的特权。*

## 原因

创建此日历的用户（其原始所有者）是已停用的用户。 

## 解决方案

您可以通过以下方式解决此问题：

1. 复制原始日历。 当您复制日历时，您就成为该日历的所有者。 复制的日历应显示原始日历中的所有信息。\
   有关复制日历的详细信息，请参阅 [复制日历报告](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. 与原始日历相同的用户共享复制的日历。 所有用户在新日历上都应看到相同的信息。
1. （可选且视情况而定）如果您有管理原始日历的权限，请从日历共享区域删除与其共享日历的所有其他用户。 这消除了用户尝试显示错误日历时的困惑。
