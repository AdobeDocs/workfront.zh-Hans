---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 查看Jira活动日志
description: 作为 [!DNL Jira] 管理员，您可以在活动日志中查看在 [!DNL Adobe Workfront] 和 [!DNL Jira] 之间同步或创建票证期间发生的异常和错误。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# 查看[!UICONTROL [!DNL Jira]活动日志]

作为[!DNL Jira]管理员，您可以在[!UICONTROL 活动日志]中查看在[!DNL Adobe Workfront]和[!DNL Jira]之间同步或创建票证期间发生的异常和错误。

您在活动日志中最多可以看到500个项目，这些项目将从最新项目开始列出。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL Adobe Workfront]计划</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront]许可证概述</a>*</td> 
   <td> <p>[!UICONTROL 计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要提示：建议您在[!DNL Jira]和[!DNL Workfront]中创建单独的系统管理员帐户以专门用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是[!DNL Workfront]管理员。 有关[!DNL Workfront]管理员的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> <p>注意：如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

在链接[!DNL Workfront]和[!DNL Jira]之间的项目之前，您必须

* 安装[!DNL Workfront for Jira]

  有关安装[!DNL Workfront for Jira]的说明，请参阅[安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

## 访问[!UICONTROL [!DNL Jira]活动日志]：

1. 以系统管理员身份登录Jira。
1. 在主[!DNL Jira]菜单中单击&#x200B;**[!UICONTROL 设置]**。
1. 单击&#x200B;**[!UICONTROL 插件]**，然后单击&#x200B;**[!UICONTROL 管理插件]**。

1. 展开&#x200B;**[!DNL Workfront]**&#x200B;加载项。
1. 单击&#x200B;**[!UICONTROL 配置]**。
1. 以系统管理员身份登录到[!DNL Workfront]。
1. 选择&#x200B;**[!UICONTROL 活动日志]**&#x200B;选项卡。

   查看有关创建项目或同步两个应用程序之间的字段期间发生的异常和错误的信息。

   日志包含以下字段：

   * 发生日期
   * Jira中的用户的名称
   * Jira问题编号
   * 所发生错误的简短描述。
