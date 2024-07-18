---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: 配置主页日程表视图设置
description: 您可以配置主页日历设置以与基于Web的Outlook版本集成，并帮助您根据可用工作时间跟踪工作负载。
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# 配置[!UICONTROL 主页日历]视图设置

<!--Audited: 01/2024-->

您可以配置[!UICONTROL 主页日历]设置以执行以下操作：

* 在云托管的 [!DNL Office 365] 或 [!DNL Outlook Live] 中与 [!DNL Outlook] 基于网络的版本集成。在Adobe Workfront中，您可以显示Outlook日历的所有活动以及在[!UICONTROL 主页日历]中选择的任何关联日历。
* 帮助您根据[!UICONTROL 分配]栏上的可用工作时间跟踪工作负载。

若要了解有关主页日历的更多信息，请参阅[[!UICONTROL 主页日历]视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)。

本文介绍了如何配置主页日历设置以及如何将主页日历与外部Outlook日历集成。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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

*要了解您拥有什么计划或许可证类型，请与[!DNL Workfront]管理员联系。 有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于集成[!DNL Microsoft Outlook]日历

在使用[!DNL Microsoft Outlook]日历配置主页日历时，请考虑以下事项：

* 您只能在云托管的[!DNL Office 365]或[!DNL Outlook Live]中集成基于Web的[!DNL Outlook]版本。

  不支持基于云的企业[!DNL Exchange]服务器上的内部部署[!DNL Outlook]和[!DNL Outlook]。

  如果您的组织使用单点登录，则您需要[!DNL Microsoft 365 E3]或[!DNL E5]。

* 与您的[!DNL Outlook]活动关联的附件未附加到您的主页日历中的[!DNL Outlook]活动。
* 必须为每个用户分别完成与[!DNL Outlook]日历的集成。
* 出现在[!UICONTROL 到期]栏中的事件不会出现在您的[!DNL Microsoft]日历中，除非您将其从[!UICONTROL 工作列表]拖到[!DNL Adobe Workfront]日历中。 有关详细信息，请参阅[[!UICONTROL 主页日历]视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)中[!UICONTROL 主页日历]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view)的[[!UICONTROL 到期]栏](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar)和[工作列表。

* 启用与[!DNL Outlook]的集成时，只有从该时间点开始拖放到[!UICONTROL 主页日历]上的工作项才会同步。 在启用集成之前位于主页日历上的项目将不会显示，如果您希望这些项目在[!DNL Outlook]中显示，必须将其再次拖动到主页日历上。
* 当您与其他人共享（或取消共享）一个[!DNL Outlook]日历，或者当您更改与其他人共享的日历的权限级别时，此更改不会影响他们的日历约30分钟。 有关详细信息，请参阅[!DNL Microsoft Outlook]文档。\
   因此，当您将[!DNL Workfront]日历与您与其他用户共享的[!DNL Outlook]日历集成时，他们将在大约30分钟内看不到您的[!DNL Workfront]日历项目。

>[!NOTE]
>
>[!DNL Outlook]日历配置与[!DNL Outlook]加载项（[!UICONTROL [!DNL Outlook]集成]或[!DNL Workfront Outlook]）完全不同。 无需安装即可配置日历，但[!DNL Outlook]加载项需要安装。 有关[!DNL Outlook]加载项的更多信息，请参阅[设置 [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md)。

## 配置[!UICONTROL 主页日历]视图设置并将其与Outlook日历集成

1. 在[!UICONTROL 主页日历]视图中，单击右上角的&#x200B;**[!UICONTROL 设置]**&#x200B;齿轮图标![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)以打开右边的&#x200B;**[!UICONTROL 日历设置]**&#x200B;面板。

   如果您需要有关访问[!UICONTROL 主页日历]视图的信息，请参阅[查看[!UICONTROL 主页日历]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md)。

1. （可选）要集成[!DNL Microsoft Outlook]日历，请单击&#x200B;**[!UICONTROL 日历设置]**&#x200B;面板右上角的&#x200B;**[!UICONTROL 添加帐户]**。 然后，如果系统提示您输入登录信息[!DNL Microsoft Outlook]。 您可以重复此步骤以添加多个[!DNL Outlook]帐户。

   >[!NOTE]
   >
   >您必须授予[!DNL Workfront]权限才能访问您的[!DNL Outlook]日历。 授予权限允许[!DNL Workfront]保持对日历数据的访问权限，读取您的[!DNL outlook]配置文件，以及读取和更新您的[!DNL Microsoft]日历。

1. 刷新浏览器窗口，在日历和[!UICONTROL 日历设置]面板中查看[!DNL Outlook]帐户的信息。
1. 再次单击右上角的&#x200B;**[!UICONTROL 设置]**&#x200B;齿轮图标以打开&#x200B;**[!UICONTROL 日历设置]**&#x200B;面板。 ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. （可选）在上一步中添加的每个[!DNL Microsoft]帐户下，选择&#x200B;**[!UICONTROL 查看]**&#x200B;或&#x200B;**[!UICONTROL 同步]**：

   * **[!UICONTROL 查看]**：这是一个只读选项，在您的[!UICONTROL 主页日历]上显示[!DNL Microsoft]个日历事件。
   * **[!UICONTROL 同步]**：此选项允许在[!DNL Microsoft]和[!UICONTROL Home]日历之间进行双向同步。 换句话说，[!DNL Workfront] [!UICONTROL 主页日历]项目将实时导出到您的[!DNL Microsoft]日历，而[!DNL Microsoft]日历项目将导入到您的Workfront [!UICONTROL 主页日历]。

     ![](assets/view-sync-checkboxes-qs.png)

1. （可选）在您的[!DNL Workfront]帐户或集成帐户下，选择要在[!UICONTROL 主页日历]上查看的相关日历（如PTO、生日或节假日），然后单击浏览器的[!UICONTROL 刷新]或[!UICONTROL 重新加载]按钮查看更改。

1. （可选）在&#x200B;**[!UICONTROL 开始周日期]**&#x200B;下的&#x200B;**[!UICONTROL 常规]**&#x200B;部分中，选择要作为工作周的第一天显示在主页日历中的日期。

   ![](assets/general-section-home-calendar-settings-panel.png)

1. 配置以下选项：

   * **[!UICONTROL 我的工作日]：**&#x200B;选择您工作的日。
   * **[!UICONTROL 我的常用开始时间]：**&#x200B;选择您开始工作日的时间。
   * **[!UICONTROL 我的常用结束时间]：**&#x200B;选择您结束工作日的时间。

   [!DNL Workfront]使用这三个设置计算您一周的工作小时数。 此数字影响[!UICONTROL 分配]栏，这有助于您根据可用工作时间跟踪工作负载。 有关详细信息，请参阅文章[[!UICONTROL 主页日历]视图](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md)中的[[!UICONTROL 分配]栏](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time)。

1. 单击&#x200B;**[!UICONTROL 日历设置]**&#x200B;区域外部以将其关闭。

   [!DNL Workfront]自动保存您的更改。

有关使用[!UICONTROL 日历]视图管理您的工作分派和集成日历事件的信息，请参阅[使用[!UICONTROL 主页日历]视图](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md)。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
