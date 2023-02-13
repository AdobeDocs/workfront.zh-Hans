---
title: AtTask OnPremise支持策略
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront于2011年12月31日转为使用100% Software-As-A-Service模式，并停止销售内部部署软件。 自2014年起，不再支持AtTask OnPremise，但许可证密钥相关问题除外。 内部部署应用程序不再可供下载或安装。
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# AtTask OnPremise支持策略

Adobe Workfront于2011年12月31日转为使用100% Software-As-A-Service模式，并停止销售内部部署软件。 自2014年起，不再支持AtTask OnPremise，但许可证密钥相关问题除外。 内部部署应用程序不再可供下载或安装。

如果您已经拥有应用程序并且需要重新安装OnPremise，请下载安装指南。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

下载有关SSL/TSL设置的说明。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 更新OnPremise许可证密钥

如果您需要新的许可证密钥，请致电Workfront客户支持844-306-HELP(4357)。

一旦你获得了新的许可证密钥，

1. 停止atTask服务器。
1. 重命名当前license.key文件（位于AtTaskDoc文件夹中）。
1. 将新的license.key文件复制到适当位置。
1. 重新启动atTask服务器。

本文包括以下附件：
