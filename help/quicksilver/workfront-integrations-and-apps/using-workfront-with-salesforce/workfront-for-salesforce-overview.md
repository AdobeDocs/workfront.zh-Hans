---
content-type: overview
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Adobe Workfront for Salesforce概述
description: 您可以安装 [!DNL Adobe Workfront] ，以便您的Salesforce用户能够提交 [!DNL Workfront] 无需离开Salesforce即可请求和自动创建项目。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 65d4cdae-1d34-4a8a-a1c0-706cd41fc75e
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# [!DNL Adobe Workfront for Salesforce] 概述

A [!UICONTROL Pro] [!DNL Workfront] 使用此功能需要计划。 有关各种可用计划的更多信息，请参阅 [[!DNL Workfront] 计划。](https://www.workfront.com/plans)

您可以安装 [!DNL Adobe Workfront for Salesforce] 允许 [!DNL Salesforce] 用户提交 [!DNL Workfront] 请求并自动创建项目，无需离开 [!DNL Salesforce].

As a [!DNL Workfront] 管理员，您可以下载和配置 [!DNL Workfront for Salesforce]. 然后，您可以共享所有其他内容 [!DNL Salesforce] 用户。

有关安装的详细信息 [!DNL Workfront for Salesforce]，请参阅 [安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).\
有关配置 [!DNL Workfront] 部分 [!DNL Salesforce] 对于所有用户，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## 访问要求

您必须具有以下访问权限才能使用本文中描述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## [!DNL Workfront for Salesforce]

使用 [!DNL Workfront for Salesforce]:

* 手动创建新 [!DNL Workfront] 请求 [!DNL Salesforce] 在Opportunity或Account中。

   有关创建 [!DNL Workfront] 请求 [!DNL Salesforce]，请参阅 [提交 [!DNL Adobe Workfront] 请求 [!DNL Salesforce] 对象](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md).

* 自动触发在中创建项目 [!DNL Workfront] 在 [!DNL Salesforce]. 您的 [!DNL Salesforce] 系统管理员必须配置从创建项目的触发器 [!DNL Salesforce].

   有关创建 [!DNL Workfront] 项目 [!DNL Salesforce]，请参阅 [创建 [!DNL Adobe Workfront] 项目 [!DNL Salesforce] 对象](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

使用时请考虑以下事项 [!DNL Workfront] 表示 [!DNL Salesforce]:

* 我们支持 [!DNL Salesforce Classic] 和 [!DNL Lightning Experience] 框架。
* 项目只能从 [!DNL Salesforce] 到 [!DNL Workfront].
* 您可以查看有关 [!DNL Workfront] 项目 [!DNL Salesforce].

   无法自定义此信息。

   要获取 [!DNL Workfront] 可从中查看的字段 [!DNL Salesforce]，请参阅  [提交 [!DNL Adobe Workfront] 请求 [!DNL Salesforce] 对象](../../workfront-integrations-and-apps/using-workfront-with-salesforce/submit-workfront-requests-from-salesforce-objects.md)  和 [创建 [!DNL Adobe Workfront] 项目 [!DNL Salesforce] 对象](../../workfront-integrations-and-apps/using-workfront-with-salesforce/create-wf-projects-from-salesforce-objects.md).

* 您可以直接访问链接到的项目 [!DNL Salesforce] 单击 **[!UICONTROL 转到Salesforce]** 链接自Workfront。

   您无法查看有关 [!DNL Salesforce] 项目 [!DNL Workfront]，但您有一个指向 [!UICONTROL Salesforce] 项目自 [!DNL Workfront] 查看 [!DNL Salesforce].

   [!UICONTROL 的 **转到Salesforce**] 链接会在以下区域中显示：

   * 的 [!UICONTROL 详细信息] 项目或问题部分
   * 项目或问题的标题。

      您的系统或组管理员必须将 [!UICONTROL 集成] 字段来查看 [!UICONTROL 转到Salesforce] 链接或问题标题。
   * 的 [!DNL Summary] 在单击 [!UICONTROL 打开摘要] ![](assets/summary-panel-icon.png) 中。

      >[!NOTE]
      >
      >的 [!UICONTROL 转到Salesforce] 链接对所有 [!DNL Workfront] 可以查看项目或问题的用户。 您必须具有 [!DNL Salesforce] 帐户 [!DNL Salesforce] 记录问题的机会或帐户。

* 更新一个应用程序中某个项目的字段时，不会更新另一个应用程序中链接项目的任何信息。
