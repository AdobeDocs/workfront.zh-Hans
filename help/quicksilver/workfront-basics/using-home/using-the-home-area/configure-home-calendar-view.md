---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 配置主页日程表视图设置
description: 您可以配置主页日历设置以与基于Web的Outlook版本集成，并帮助您根据可用工作时间跟踪工作负载。
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 3b3ba7cc6a975af71205f7f524e1a9a91a9d3810
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 1%

---

# 配置您的 [!UICONTROL 主页日程表] 查看设置

<!--Audited: 01/2024-->

您可以配置 [!UICONTROL 主页日程表] 设置完成以下操作：

* 在云托管的 [!DNL Office 365] 或 [!DNL Outlook Live] 中与 [!DNL Outlook] 基于网络的版本集成。您可以显示Outlook日历中的所有事件以及在中选择的任何关联日历 [!UICONTROL 主页日程表] 在Adobe Workfront中。
* 帮助您根据您在上可用的工作时间跟踪工作负载 [!UICONTROL 分配] 栏。

要了解有关主页日程表的详细信息，请参阅 [[!UICONTROL 主页日程表] 视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

本文介绍了如何配置主页日历设置以及如何将主页日历与外部Outlook日历集成。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>当前： [！UICONTROL Work]或更高版本</p> 
   或
   <p>新文档： [！UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*要了解您的计划或许可证类型，请联系贵机构的 [!DNL Workfront] 管理员。 有关更多信息，请参阅 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 关于集成 [!DNL Microsoft Outlook] 日历

在使用配置主页日程表时，请考虑以下事项 [!DNL Microsoft Outlook] 日历：

* 您只能集成基于Web的版本 [!DNL Outlook] 在云托管中 [!DNL Office 365] 或 [!DNL Outlook Live].

  内部部署 [!DNL Outlook] 和 [!DNL Outlook] 基于云的企业 [!DNL Exchange] 服务器不受支持。

  如果您的组织使用单点登录，您需要 [!DNL Microsoft 365 E3] 或 [!DNL E5].

* 与您的关联的附件 [!DNL Outlook] 事件未附加到 [!DNL Outlook] 您的主页日程表上的活动。
* 与集成 [!DNL Outlook] 必须为每个用户分别完成日历。
* 在中显示的事件 [!UICONTROL 到期] 栏未显示在您的 [!DNL Microsoft] 除非您从 [!UICONTROL 工作列表] 敬您的 [!DNL Adobe Workfront] 日历。 有关更多信息，请参阅 [[!UICONTROL 到期] 条形图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) 和 [上的工作列表 [!UICONTROL 主页日程表]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) 在 [[!UICONTROL 主页日程表] 视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* 当您启用与的集成时 [!DNL Outlook]，仅限拖动到上的工作项 [!UICONTROL 主页日程表] 从此刻开始，将进行同步。 在启用集成之前位于主页日历上的项目将不会显示，如果您希望这些项目在中显示，必须将其再次拖动到主页日历上 [!DNL Outlook].
* 当您共享（或取消共享） [!DNL Outlook] 其他人共享的日历，或者当您更改与其他人共享的日历的权限级别时，此更改不会影响他们的日历，时间约为30分钟。 欲知更多信息，请参见 [!DNL Microsoft Outlook] 文档。\
   因此，当您集成 [!DNL Workfront] 带有以下内容的日历 [!DNL Outlook] 您与其他用户共享的日历，他们将看不到您的 [!DNL Workfront] 日历项目约30分钟。

>[!NOTE]
>
>此 [!DNL Outlook] 日历配置与 [!DNL Outlook] 加载项([!UICONTROL [!DNL Outlook] 集成] 或 [!DNL Workfront Outlook])。 无需安装即可配置日历，但需要安装 [!DNL Outlook] 加载项。 欲知关于 [!DNL Outlook] 加载项请参阅 [设置 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## 配置您的 [!UICONTROL 主页日程表] 查看设置并将其与Outlook日历集成

1. 在 [!UICONTROL 主页日程表] 视图，单击 **[!UICONTROL 设置]** 齿轮图标 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) 在右上角打开 **[!UICONTROL 日历设置]** 在右边的面板中。

   如果您需要有关访问 [!UICONTROL 主页日程表] 视图，请参阅 [查看 [!UICONTROL 主页日程表]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. （可选）要集成 [!DNL Microsoft Outlook] 日历，单击 **[!UICONTROL 添加帐户]** 位于的右上角 **[!UICONTROL 日历设置]** 面板。 然后，如果系统提示您这样做，请输入 [!DNL Microsoft Outlook] 登录信息。 您可以重复此步骤以添加多个 [!DNL Outlook] 帐户。

   >[!NOTE]
   >
   >你必须给予 [!DNL Workfront] 访问 [!DNL Outlook] 日历。 授予权限允许 [!DNL Workfront] 要维护对日历数据的访问，请阅读 [!DNL outlook] 个人资料，并读取和更新 [!DNL Microsoft] 日历。

1. 刷新浏览器窗口查看来自您的的信息 [!DNL Outlook] 日历中的帐户和 [!UICONTROL 日历设置] 面板。
1. 单击 **[!UICONTROL 设置]** 再次打开右上角的齿轮图标 **[!UICONTROL 日历设置]** 面板。 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. （可选）在每个 [!DNL Microsoft] 在上一步中添加的帐户，选择 **[!UICONTROL 视图]** 或 **[!UICONTROL 同步]**：

   * **[!UICONTROL 视图]**：这是一个只读选项，会显示 [!DNL Microsoft] 您的日历活动 [!UICONTROL 主页日程表].
   * **[!UICONTROL 同步]**：此选项允许您的主机和服务器之间 [!DNL Microsoft] 和 [!UICONTROL 主页] 日历。 换句话说， [!DNL Workfront] [!UICONTROL 主页日程表] 导出到 [!DNL Microsoft] 日历和 [!DNL Microsoft] 将日历项目导入您的Workfront [!UICONTROL 主页日程表] 实时。

     ![](assets/view-sync-checkboxes-qs.png)

1. （可选）在您的下 [!DNL Workfront] 帐户或集成帐户，选择要在 [!UICONTROL 主页日程表] （例如您的PTO、生日或节假日日历），然后单击浏览器的 [!UICONTROL 刷新] 或 [!UICONTROL 重新加载] 按钮以查看您所做的更改。

1. （可选）在 **[!UICONTROL 常规]** 部分在 **[!UICONTROL 每周开始于]**，选择要作为工作周的第一天在主页日历中显示的那一天。

   ![](assets/general-section-home-calendar-settings-panel.png)

1. 配置以下选项：

   * **[!UICONTROL 我的工作日]：** 选择您工作的日期。
   * **[!UICONTROL 我的常用开始时间]：** 选择您开始工作日的时间。
   * **[!UICONTROL 我的常用结束时间]：** 选择结束工作日的时间。

   [!DNL Workfront] 使用这三个设置来计算您一周的工作小时数。 此数字会影响 [!UICONTROL 分配] 栏可帮助您根据可用工作时间跟踪工作负载。 有关更多信息，请参阅 [[!UICONTROL 分配] 条形图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) 在文章中 [[!UICONTROL 主页日程表] 视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. 在 **[!UICONTROL 日历设置]** 区域将其关闭。

   [!DNL Workfront] 自动保存更改。

有关使用 [!UICONTROL 日历] 查看以管理您的工作分派和集成的日历事件，请参阅 [使用 [!UICONTROL 主页日程表] 视图](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
