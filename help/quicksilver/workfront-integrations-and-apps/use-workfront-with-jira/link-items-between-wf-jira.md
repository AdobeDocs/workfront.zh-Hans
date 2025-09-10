---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 链接介于 [!DNL Adobe Workfront] 和 [!DNL Jira]之间的项目
description: 您可以自动或手动将 [!DNL Jira] 问题链接到 [!DNL Adobe Workfront] 任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '1324'
ht-degree: 0%

---

# [!DNL Adobe Workfront]和[!DNL Jira]之间的链接项

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，Workfront for Jira集成在&#x200B;**2026年2月28日**&#x200B;后不可用。
>
>为了满足贵组织与Jira的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Jira的Workfront自动化和集成模块的特定功能的信息，请参阅[Jira软件模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules)。

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

您可以自动或手动将[!DNL Jira]问题链接到[!DNL Adobe Workfront]任务或问题。

只能将[!DNL Workfront]中的一个项目链接到[!DNL Jira]中的一个项目。 您永远不能将一个[!DNL Workfront]项目链接到多个[!DNL Jira]问题，也不能将一个[!DNL Jira]问题链接到多个[!DNL Workfront]项目。

## 访问要求

您必须具备以下条件：

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] 计划]</a></td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront]许可证概述</a></td> 
   <td> 
   <p>新增：标准<p>
   <p>或</p>
   <p>当前：计划 </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira访问</td> 
   <td> <p>系统管理员访问权限</p> <p><b>重要</b>

我们建议您在[!DNL Jira]和[!DNL Workfront]中创建单独的系统管理员帐户以专用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是[!DNL Workfront]管理员。 有关[!DNL Workfront]管理员的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> <p><b>注释</b>

如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在链接[!DNL Workfront]和[!DNL Jira]之间的项目之前，您必须执行以下操作：

* 为[!DNL Workfront]安装[!DNL Jira]。

  有关说明，请参阅[安装Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

* 为Jira配置[!DNL Workfront]。

  有关说明，请参阅[配置Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 自动将[!DNL Workfront]项链接到[!DNL Jira]问题

作为[!DNL Workfront]管理员，您可以定义触发器，该触发器将在每次在[!DNL Jira]中的任务或问题满足特定条件时在[!DNL Workfront]中自动创建问题。 Workfront和[!DNL Jira]项已链接。

完成Jira的[!DNL Workfront]配置后，在[!DNL Workfront]中创建或更新项以匹配触发器时，将在[!DNL Jira]中自动创建新项。

创建和更新Workfront项目的Workfront用户不需要[!DNL Jira]许可证即可触发在[!DNL Jira]中创建项目。

有关详细信息，请参阅[为Jira [!DNL Adobe Workfront] 配置](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

>[!NOTE]
>
>通过将模板附加到项目，您可以自动创建[!DNL Jira]项。 如果模板包含的工作分配符合[!DNL Jira]触发器，则新任务将生成新的[!DNL Jira]问题。

自动将[!DNL Workfront]问题链接到[!DNL Jira]问题与自动将[!DNL Workfront]任务链接到[!DNL Jira]问题相同。

要自动将[!DNL Workfront]任务链接到[!DNL Jira]问题：

1. 确保您的[!DNL Jira]系统管理员已配置触发器，以便在分配[!DNL Jira]项时自动创建[!DNL Workfront]问题，然后使用允许您创建任务的访问级别登录到[!DNL Workfront]。

   有关访问任务的更多信息，请参阅[授予访问任务的权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。

{{step1-to-projects}}

1. 在&#x200B;**项目**&#x200B;页面上，选择一个项目。

1. 在项目左侧面板中，选择&#x200B;**[!UICONTROL 任务]**。

1. 单击&#x200B;**+新任务**。

   >[!NOTE]
   >
   >要将现有Workfront项目链接到Jira问题，请从该项目的&#x200B;**更多** **更多图标**&#x200B;菜单中选择![编辑](assets/more-icon.png)。

1. 指定或更新任务可用的任何字段。
1. 在&#x200B;**[!UICONTROL 工作总揽]**&#x200B;字段中，搜索并选择在[!DNL Jira]集成中指定为触发器的用户、角色或团队。

1. 单击&#x200B;**创建任务**。 任务已在Workfront中创建，且任务的&#x200B;**更新**&#x200B;选项卡中会显示新注释，以指示已在[!DNL Jira]中创建新问题。

1. （可选）在任务或问题标题的&#x200B;**[!UICONTROL 详细信息]**&#x200B;部分的&#x200B;**[!UICONTROL 集成]**&#x200B;区域中，单击&#x200B;**[!UICONTROL 转到Jira]**&#x200B;链接以在Jira中打开问题。

   您的系统或组管理员必须将[!UICONTROL 集成]字段添加到您的布局模板中，才能在任务或问题标题中显示该字段。 有关信息，请参阅[使用布局模板自定义对象标头](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

   任何[!DNL Jira]用户都可以立即开始处理从[!DNL Workfront]自动创建的项目，其更新将传输到[!DNL Workfront]，而无需[!DNL Workfront]的许可证即可完成此操作。

   只有您在[!DNL Workfront]加载项设置期间作为[!DNL Workfront]管理员配置的字段才会更新。

   有关在Workfront和Jira之间同步字段的更多信息，请参阅[为Jira配置Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)中的“为Jira配置Adobe Workfront”部分。

   >[!NOTE]
   >
   >从Workfront自动创建[!DNL Jira]问题时，该问题未分配给[!DNL Jira]中的任何人。

## 手动将[!DNL Jira]问题链接到[!DNL Workfront]个项目

在[!DNL Jira]和[!DNL Workfront]中创建相互独立的项后，您可以手动将[!DNL Jira]问题链接到现有的[!DNL Workfront]任务或问题。

您无法手动将[!DNL Workfront]项从[!DNL Workfront]链接到现有[!DNL Jira]项。

>[!NOTE]
>
>如果[!DNL Jira]问题不位于未在[!DNL Workfront]集成中识别为触发器的项目上，则在与[!DNL Jira]内部部署集成时，无法手动将其链接到Workfront项。\
>有关为Workfront到Jira工作流设置触发器的更多信息，请参阅[自动将Workfront项目链接到Jira问题](#automatically-link-workfront-items-to-jira-issues)。

当链接[!DNL Workfront]和[!DNL Jira]项时，一项中的某些字段会在另一项中自动更新。\
有关更新链接项的更多信息，请参阅[在Jira和Adobe Workfront之间更新链接项](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md)。

要手动将[!DNL Jira]问题链接到[!DNL Workfront]项，请执行以下操作：

1. （视情况而定）登录到[!DNL Workfront]并找到要链接到[!DNL Jira]问题的问题或任务。
1. （视情况而定）在&#x200B;**任务详细信息**&#x200B;或&#x200B;**问题详细信息**&#x200B;选项卡的&#x200B;**基本信息**&#x200B;部分中，复制Workfront中项目的&#x200B;**[!UICONTROL 参考编号]**。

   或

   从项目的地址栏中，复制Workfront中项目的&#x200B;**URL**。

   >[!IMPORTANT]
   >
   >如果您的组织已载入到Adobe Unified Experience，则必须使用&#x200B;**参考编号**&#x200B;将Workfront项目链接到Jira。 （URL选项可用，但如果您使用它，则将返回错误。） 有关Unified Experience的信息，请参阅[适用于Workfront的Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md)。
   >
   >对于不在Adobe Unified Experience上的组织，不建议使用URL选项，因为URL可能会发生更改。

   >[!NOTE]
   >
   >您必须拥有[!DNL Workfront]许可证才能登录到[!DNL Workfront]。 否则，[!DNL Workfront]用户必须提供此信息给您。

1. 在[!DNL Jira]中，导航到要手动链接到[!DNL Workfront]项目的问题。
1. 在[!DNL Workfront]右侧面板中，粘贴要将其链接到的&#x200B;**[!UICONTROL 项的]**&#x200B;引用编号&#x200B;**或** URL[!DNL Workfront]。

1. 单击&#x200B;**[!UICONTROL 链接]**。 这两个项目将链接，[!DNL Workfront]右侧面板中填充了[!DNL Workfront]项目中的信息。

   默认情况下，以下[!DNL Workfront]字段在[!DNL Jira]右侧面板的[!DNL Workfront]中可见：

   * 项的&#x200B;**[!UICONTROL Name]**。 您可以通过单击面板中的名称来访问[!DNL Workfront]项。
   * **[!UICONTROL 项目名称]**。
   * 项目的&#x200B;**[!UICONTROL 状态]**。
   * 该项的&#x200B;**[!UICONTROL 优先级]**。
   * 创建日期为[!DNL Workfront]。
   * 项目的&#x200B;**[!UICONTROL 计划小时数]**。
   * **[!UICONTROL 参考编号]**。 您可以通过单击面板中的[!DNL Workfront]参考编号&#x200B;**来访问**&#x200B;项。

   有关启用其他字段在右侧面板中显示的详细信息，请参阅[!DNL Jira]配置[!DNL Workfront]中的“配置[和 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)项之间的字段同步”部分。 来自与集成关联的[!DNL Workfront]管理员的注释已发布在&#x200B;**[!DNL Workfront]**&#x200B;问题的[!DNL Jira]选项卡中，以确认已创建新的[!DNL Jira]项目。 该评论包含指向[!DNL Jira]问题的链接。

## 取消链接[!DNL Jira]和[!DNL Workfront]之间的项目

在[!DNL Jira]中可以手动取消链接[!DNL Workfront]和[!DNL Jira]之间的链接项。 您无法取消与[!DNL Workfront]中对应项[!DNL Jira]的[!DNL Workfront]项目的链接。

您需要以下访问权限才能取消手动链接项目的链接：

* 您是手动链接项目的用户。
* 您是[!DNL Jira]系统管理员。

>[!NOTE]
>
>只有[!DNL Workfront]管理员可以取消自动链接项目的链接。

要从[!DNL Jira]项中取消链接[!DNL Workfront]问题，请执行以下操作：

1. 登录Jira。
1. 导航到链接到[!DNL Workfront]任务或问题的问题。
1. 转到&#x200B;**Workfront**&#x200B;右侧面板。
1. 单击&#x200B;**[!UICONTROL 取消链接]**&#x200B;图标，然后单击&#x200B;**[!UICONTROL 取消链接]**。 之前链接的[!DNL Jira]和[!DNL Workfront]项已取消链接。

   以后更新的任何字段、注释或文档都不会在另一个应用程序中的以前对应项上更新。
