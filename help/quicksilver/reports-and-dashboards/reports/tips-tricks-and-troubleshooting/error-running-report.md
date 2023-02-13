---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: “运行报表时出现错误消息：“您当前未登录。”
description: 您必须具有以下访问权限才能执行本文中的步骤 — 编辑我。
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# 运行报表时出现错误消息：“您当前未登录。”

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划，工作</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报表、功能板、日历的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 问题

运行报表或在功能板中显示报表时，会返回以下错误：\
*让我们再试一次。 您当前未登录。*

报表中未显示任何结果。

## 原因

报表当前设置为以停用用户的身份运行。

## 解决方案

您必须拥有报表的“管理”权限才能更改报表设置。\
要调整报表并查看结果，请执行以下操作：

1. 转到报表。
1. 单击 **报表操作** > **编辑** > **报表设置**.

1. 在 **使用以下访问权限运行此报表：** 字段。\
   或\
   离开 **使用以下访问权限运行此报表：** 字段。

1. 单击 **完成**.
1. 单击 **保存并关闭**.\
   运行此报表时，不应再次显示错误。
