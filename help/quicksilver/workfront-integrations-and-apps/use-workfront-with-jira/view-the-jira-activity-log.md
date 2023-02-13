---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: 查看Jira活动日志
description: As a [!DNL Jira] 管理员，您可以查看在同步或创建票证期间在 [!DNL Adobe Workfront] 和 [!DNL Jira] 活动日志中。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# 查看 [!UICONTROL [!DNL Jira] 活动日志]

As a [!DNL Jira] 管理员，您可以查看在同步或创建票证期间在 [!DNL Adobe Workfront] 和 [!DNL Jira] 在 [!UICONTROL 活动日志].

您最多可以在活动日志中看到500个项目，这些项目从最近的项目开始列出。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 计划</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 许可证概述</a>*</td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] 访问</td> 
   <td> <p>系统管理员访问权限</p> <p>重要信息：我们建议您在 [!DNL Jira] 和 [!DNL Workfront] 专门用于此集成，而不是使用可能附加到用户的现有集成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

在您关联项目之前 [!DNL Workfront] 和 [!DNL Jira]，您必须

* 安装 [!DNL Workfront for Jira]

   有关安装的说明 [!DNL Workfront for Jira]，请参阅 [安装 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## 访问 [!UICONTROL [!DNL Jira] 活动日志]:

1. 以系统管理员身份登录Jira。
1. 单击 **[!UICONTROL 设置]** 在主 [!DNL Jira] 菜单。
1. 单击 **[!UICONTROL 附加组件]**，则 **[!UICONTROL 管理附加组件]**.

1. 展开 **[!DNL Workfront]** 附加组件。
1. 单击 **[!UICONTROL 配置]**.
1. 登录到 [!DNL Workfront] 作为系统管理员。
1. 选择 **[!UICONTROL 活动日志]** 选项卡。

   查看在创建项目或在两个应用程序之间同步字段期间发生的例外和错误的信息。

   日志包含以下字段：

   * 发生日期
   * Jira中用户的名称
   * Jira问题编号
   * 所发生错误的简要描述。
