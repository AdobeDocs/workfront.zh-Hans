---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: 从 [!DNL Slack]中的共享链接访问 [!DNL Adobe Workfront] 对象
description: 当在Slack渠道中与您共享指向 [!DNL Adobe Workfront] 对象的链接时，在安装和配置 [!DNL Workfront] 进行Slack后，您可以在Slack中查看有关这些对象的其他信息。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 587c6ac7-cc56-480f-852d-f0bd36b3f3cf
source-git-commit: eeb90d8f80b1680d880d07f41e9d80c0658495fa
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 0%

---

# 从[!DNL Slack]中的共享链接访问[!DNL Adobe Workfront]对象

当指向[!DNL Adobe Workfront]对象的链接在[!DNL Slack]渠道中与您共享时，安装并配置[!DNL Workfront for Slack]后，您可以在[!DNL Slack]中查看有关这些对象的附加信息。

有关配置[!DNL Workfront for Slack]的详细信息，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

您必须在单独的浏览器选项卡中登录到[!DNL Workfront]，才能打开链接或从[!DNL Slack]对这些对象执行其他操作。

当用户与您共享指向[!DNL Workfront]中对象的链接时，有关该对象的附加信息可能也会与该链接一起显示。 发送链接的用户必须具有对该对象的至少[!UICONTROL 查看]权限，其他信息才能显示在[!DNL Slack]中。

## 访问要求

您必须具有以下权限才能使用本文中所述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

在从[!DNL Slack]访问收藏夹和最新项目之前，您必须

* 配置[!DNL Workfront for Slack]\
   有关配置[!DNL Workfront for Slack]的说明，请参阅[配置 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)。

## 从[!DNL Slack]访问项目

1. 登录到您的[!DNL Slack]实例并登录到[!DNL Workfront from Slack.]

   有关从[!DNL Slack]登录到[!DNL Workfront]的更多信息，请参阅[访问 [!DNL Adobe Workfront from Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“登录到[!DNL Workfront from Slack]”部分。

1. 导航到包含指向[!DNL Workfront]项目的链接的消息。

   >[!NOTE]
   >
   >共享链接的用户必须至少具有项目的[!UICONTROL 查看]权限，您才能查看有关该项目的其他信息。

1. （可选）单击项目的名称，以在新浏览器选项卡的[!DNL Workfront]中打开该项目。
1. 考虑查看有关项目的以下附加信息：

   * **[!UICONTROL 状态]：**&#x200B;有关项目状态的详细信息，请参阅[访问系统项目状态列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)。

   * **[!UICONTROL 计划完成日期]**：有关计划完成日期的详细信息，请参阅[设置项目计划完成日期](../../manage-work/projects/planning-a-project/project-planned-completion-date.md)。

   * **[!UICONTROL Portfolio]**&#x200B;名称：有关项目组合的详细信息，请参阅Adobe Workfront中的[Portfolio概述](../../manage-work/portfolios/portfolios-overview/portfolio-overview.md)。

   * **[!UICONTROL 完成情况]**：有关项目完成情况的详细信息，请参阅[项目完成情况和完成情况类型概览](../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)。

   * **[!UICONTROL 完成百分比]**：有关项目的完成百分比值的详细信息，请参阅[项目完成百分比概述](../../manage-work/tasks/task-information/project-percent-complete.md)。

   * **[!UICONTROL 参考编号]**：有关对象参考编号的详细信息，请参阅[使用对象参考编号](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)。

1. （可选）单击&#x200B;**[!UICONTROL 订阅]**&#x200B;以订阅项目。

   您将收到一个确认信息，确认您已成功订阅了项目。

## 从[!DNL Slack]访问任务

1. 登录到您的[!DNL Slack]实例并登录到[!DNL Workfront from Slack]。

   有关从[!DNL Slack]登录到[!DNL Workfront]的更多信息，请参阅[访问 [!DNL Adobe Workfront from Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 导航到包含指向[!DNL Workfront]任务的链接的消息。

   >[!NOTE]
   >
   >共享链接的用户必须至少具有任务的[!UICONTROL 查看]权限，您才能查看有关该任务的其他信息。

1. （可选）单击任务的名称以在新浏览器选项卡的[!DNL Workfront]中打开它。
1. 考虑查看有关任务的以下附加信息：

   * **[!UICONTROL 状态]**

     有关任务状态的详细信息，请参阅[访问系统任务状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)。

   * 已完成&#x200B;**[!UICONTROL 百分比]**
   * **[!UICONTROL 已分配给名称]**
   * **[!DNL Planned Completion Date]**
   * **[!UICONTROL 项目名称]**&#x200B;或&#x200B;**[!UICONTROL 父任务名称]**
   * **[!UICONTROL 参考编号]**

     有关对象参考编号的详细信息，请参阅[使用对象参考编号](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)。

1. （可选）单击&#x200B;**[!UICONTROL 订阅]**&#x200B;以订阅任务。

   您将收到确认信息，确认您已成功订阅任务。

1. （可选）单击&#x200B;**[!UICONTROL 分配给用户]**&#x200B;以将任务分配给用户。
1. （视情况而定）如果您已单击&#x200B;**[!UICONTROL 分配给用户]**，则开始键入用户的名称。

   您无法从[!DNL Slack]将任务分配给工作角色或团队。

## 来自[!DNL Slack]的访问问题

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。

   有关从[!DNL Slack]登录到Workfront的更多信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 导航到包含指向[!DNL Workfront]问题的链接的消息。

   >[!NOTE]
   >
   >共享链接的用户必须至少具有问题的[!UICONTROL 查看]权限，您才能查看有关该问题的其他信息。

1. （可选）单击问题的名称以在新浏览器选项卡的[!DNL Workfront]中将其打开。
1. 考虑查看有关任务的以下附加信息：

   * **[!UICONTROL 状态]**：有关问题状态的详细信息，请参阅[访问系统问题状态的列表](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)。

   * **[!UICONTROL 已分配给名称]**
   * **[!UICONTROL 计划完成日期]**
   * **[!UICONTROL 项目名称]**
   * **[!UICONTROL 参考编号]**：有关对象参考编号的详细信息，请参阅[使用对象参考编号](../../workfront-basics/navigate-workfront/search/reference-number-of-objects.md)。

1. （可选）单击&#x200B;**[!UICONTROL 订阅]**&#x200B;以订阅问题。

   您会收到确认信息，确认您已成功订阅问题。

1. （可选）单击&#x200B;**[!UICONTROL 分配给用户]**&#x200B;以将问题分配给用户。
1. （视情况而定）如果您已单击&#x200B;**[!UICONTROL 分配给用户]**，则开始键入用户的名称。

   您无法从[!DNL Slack]将问题分配给工作角色或团队。

## 从[!DNL Slack]访问项目组合

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。

   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 导航到包含指向[!DNL Workfront]项目组合链接的消息。

   >[!NOTE]
   >
   >共享链接的用户必须至少具有项目组合的[!UICONTROL 查看]权限，您才能查看有关该项目组合的其他信息。

1. （可选）单击项目组合的名称，以在新浏览器选项卡的[!DNL Workfront]中将其打开。
1. 考虑查看有关项目组合的以下附加信息：

   * **[!UICONTROL Portfolio管理器名称]**
   * **[!UICONTROL 开启时间]**
   * **[!UICONTROL ROI]**
   * **[!UICONTROL 净值]**
   * **[!UICONTROL 状态]**
   * **[!UICONTROL 预算]**
   * **[!UICONTROL 已对齐]**

     有关项目组合量度的详细信息，包括[!UICONTROL ROI]、[!UICONTROL 净值]、[!UICONTROL 一致性]以及[!UICONTROL 准时]和[!UICONTROL 预算]值，请参阅[了解[!UICONTROL Portfolio优化器]。](../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)

## 从[!DNL Slack]访问程序

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。

   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 导航到包含指向[!DNL Workfront]节目的链接的消息。

   >[!NOTE]
   >
   > 共享链接的用户必须具有对该程序的至少[!UICONTROL 查看]权限，您才能查看有关该程序的其他信息。

1. （可选）单击程序的名称，以在新浏览器选项卡的[!DNL Workfront]中打开该程序。
1. 考虑查看有关项目的以下附加信息：

   * **[!UICONTROL 描述]**
   * **[!UICONTROL Portfolio名称]**
   * **[!UICONTROL 项目经理姓名]**

     有关程序的详细信息，请参阅[创建和管理程序。](../../manage-work/portfolios/create-and-manage-programs/create-and-manage-programs.md)

## 从[!DNL Slack]访问报告

1. 从[!DNL Slack]登录到[!DNL Slack]实例并登录到[!DNL Workfront]。

   有关从[!DNL Slack]登录到[!DNL Workfront]的详细信息，请参阅[访问 [!DNL Adobe Workfront] 从 [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md)中的“从[!DNL Slack]登录到[!DNL Workfront]”部分。

1. 导航到包含指向[!DNL Workfront]报告的链接的消息。

   >[!NOTE]
   >
   >共享链接的用户必须至少具有报表的[!UICONTROL 查看]权限，您才能查看有关该链接的其他信息。

1. （可选）单击报告的名称以在新浏览器选项卡的[!DNL Workfront]中将其打开。
