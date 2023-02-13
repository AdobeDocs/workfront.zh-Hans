---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 配置主日历视图设置
description: 您可以配置“主日历”设置，以与基于Web的Outlook版本集成，并帮助您根据可用工作时间跟踪工作量。
author: Lisa
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 配置 [!UICONTROL 主日历] 查看设置

您可以配置 [!UICONTROL 主日历] 设置来执行以下操作：

* 与基于Web的 [!DNL Outlook] 云托管中 [!DNL Office 365] 或 [!DNL Outlook Live]. 您可以在Outlook日历和您选择的任何关联日历（如生日和假日日历）中显示所有事件 [!UICONTROL 主日历].
* 帮助您根据 [!UICONTROL 分配] 栏。

要了解有关主日历的更多信息，请参阅 [[!UICONTROL 主日历] 视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Work]或更高版本</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划或许可证类型，请联系 [!DNL Workfront] 管理员。

## 关于集成 [!DNL Microsoft Outlook] 日历

在使用 [!DNL Microsoft Outlook] 日历：

* 您只能集成基于Web的 [!DNL Outlook] 云托管中 [!DNL Office 365] 或 [!DNL Outlook Live].

   本地 [!DNL Outlook] 和 [!DNL Outlook] 基于云的企业 [!DNL Exchange] 不支持服务器。

   如果贵组织使用单点登录，则您需要 [!DNL Microsoft 365 E3] 或 [!DNL E5].

* 与您的 [!DNL Outlook] 事件未附加到 [!DNL Outlook] 活动。
* 与集成 [!DNL Outlook] 必须单独为每个用户填写日历。
* 在 [!UICONTROL 到期] 栏未显示在 [!DNL Microsoft] 日历，除非您从 [!UICONTROL 工作列表] 至 [!DNL Adobe Workfront] 日历。 有关更多信息，请参阅 [[!UICONTROL 到期] 栏](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) 和 [工作列表 [!UICONTROL 主日历]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL 主日历] 视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* 当您启用与的集成时 [!DNL Outlook]，仅拖动到上的工作项目 [!UICONTROL 主日历] 从那时开始，将同步。 在启用集成之前位于“主日历”中的项目将不会显示，如果希望这些项目显示在 [!DNL Outlook].
* 当您共享（或取消共享） [!DNL Outlook] 与他人共享的日历，或者当您更改与他人共享的日历的权限级别时，此更改不会影响其大约30分钟的日历(有关详细信息，请查阅 [!DNL Microsoft Outlook] 文档)。\
   因此，在集成 [!DNL Workfront] 具有 [!DNL Outlook] 您与其他用户共享的日历，他们将看不到您的 [!DNL Workfront] 大约30分钟的日历项目。

>[!NOTE]
>
>的 [!DNL Outlook] 日历配置与 [!DNL Outlook] 加载项([!UICONTROL [!DNL Outlook] 集成] 或 [!DNL Workfront Outlook])。 无需安装即可配置日历，但需要安装 [!DNL Outlook] 外接程序。 有关 [!DNL Outlook] 加载项请参阅 [设置 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## 配置 [!UICONTROL 主日历] 查看设置

1. 在 [!UICONTROL 主日历] 视图，单击 **[!UICONTROL 设置]** 齿轮图标 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) 在右上角打开 **[!UICONTROL 日历设置]** 面板。

   如果您需要有关访问 [!UICONTROL 主日历] 视图，请参阅 [查看 [!UICONTROL 主日历]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. （可选）要集成 [!DNL Microsoft Outlook] 日历，单击 **[!UICONTROL 添加帐户]** 的右上角 **[!UICONTROL 日历设置]** 的上界。 然后，如果系统提示您执行此操作，请输入 [!DNL Microsoft Outlook] 登录信息。 您可以重复此步骤以添加多个 [!DNL Outlook] 帐户。

   >[!NOTE]
   >
   >你必须给 [!DNL Workfront] 访问 [!DNL Outlook] 日历。 授予权限 [!DNL Workfront] 要保持对日历数据的访问，请阅读 [!DNL outlook] 配置文件，并读取和更新您的 [!DNL Microsoft] 日历。

1. 刷新浏览器窗口以查看 [!DNL Outlook] 日历和 [!UICONTROL 日历设置] 的上界。
1. 单击 **[!UICONTROL 设置]** 齿轮图标以打开 **[!UICONTROL 日历设置]** 的上界。 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. （可选）在 [!DNL Microsoft] 您在上一步中添加的帐户，请选择 **[!UICONTROL 查看]** 或 **[!UICONTROL 同步]**:

   * **[!UICONTROL 查看]**:这是一个只读选项，该选项将显示 [!DNL Microsoft] 您的日历事件 [!UICONTROL 主日历].
   * **[!UICONTROL 同步]**:此选项允许在 [!DNL Microsoft] 和 [!UICONTROL 主页] 日历。 换句话说， [!DNL Workfront] [!UICONTROL 主日历] 导出到 [!DNL Microsoft] 日历和 [!DNL Microsoft] 导入您的Workfront的日历项 [!UICONTROL 主日历] 实时。

      ![](assets/view-sync-checkboxes-qs.png)

1. （可选）在 [!DNL Workfront] 帐户或集成帐户，选择要在您的 [!UICONTROL 主日历] （例如PTO、生日或假日日历）然后单击浏览器的 [!UICONTROL 刷新] 或 [!UICONTROL 重新加载] 按钮以查看您所做的更改。

1. （可选）在 **[!UICONTROL 常规]** 部分 **[!UICONTROL 开始周]**，在“主日历”中选择要显示为工作周第一天的日期。

1. 配置以下选项：

   * **[!UICONTROL 我的工作日]:** 选择工作日。
   * **[!UICONTROL 我通常的开始时间]:** 选择开始工作日的时间。
   * **[!UICONTROL 我通常的结束时间]:** 选择结束工作日的时间。

   [!DNL Workfront] 使用这三个设置来计算您每周工作的小时数。 此数字会影响 [!UICONTROL 分配] 栏，可帮助您根据可用工作时间跟踪工作量。 有关更多信息，请参阅 [[!UICONTROL 分配] 栏](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) 在文章中 [[!UICONTROL 主日历] 视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. 单击 **[!UICONTROL 日历设置]** 要取消的区域。

   [!DNL Workfront] 自动保存更改。

有关使用 [!UICONTROL 日历] 查看管理工作分配和集成的日历事件，请参阅 [使用 [!UICONTROL 主日历] 视图](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
