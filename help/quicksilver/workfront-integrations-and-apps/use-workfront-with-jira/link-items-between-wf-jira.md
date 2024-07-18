---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 链接介于 [!DNL Adobe Workfront] 和 [!DNL Jira]之间的项目
description: 您可以自动或手动将 [!DNL Jira] 问题链接到 [!DNL Adobe Workfront] 任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 0%

---

# [!DNL Adobe Workfront]和[!DNL Jira]之间的链接项

您可以自动或手动将[!DNL Jira]问题链接到[!DNL Adobe Workfront]任务或问题。

只能将[!DNL Workfront]中的一个项目链接到[!DNL Jira]中的一个项目。 您永远不能将一个[!DNL Workfront]项目链接到多个[!DNL Jira]问题，也不能将一个[!DNL Jira]问题链接到多个[!DNL Workfront]项目。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront]计划]</a>*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe[!DNL Workfront]许可证概述</a>*</td> 
   <td> <p>计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira访问</td> 
   <td> <p>系统管理员访问权限</p> <p><b>重要</b>

我们建议您在[!DNL Jira]和[!DNL Workfront]中创建单独的系统管理员帐户以专用于此集成，而不是使用可能附加到用户的现有帐户。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须是[!DNL Workfront]管理员。 有关[!DNL Workfront]管理员的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> <p><b>注释</b>

如果您仍然没有访问权限，请询问您的[!DNL Workfront]管理员是否对您的访问级别设置了其他限制。 有关[!DNL Workfront]管理员如何修改访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

## 先决条件

在链接[!DNL Workfront]和[!DNL Jira]之间的项目之前，您必须

* 为[!DNL Jira]安装[!DNL Workfront]

  有关安装适用于Jira的Workfront的说明，请参阅[安装适用于Jira的Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md)。

* 为Jira配置[!DNL Workfront]

  有关为Jira配置Workfront的说明，请参阅[为Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)。

## 自动将[!DNL Workfront]项链接到[!DNL Jira]问题

作为[!DNL Workfront]管理员，您可以定义每次在[!DNL Workfront]中的任务或问题满足特定条件时，可在[!DNL Jira]中自动创建问题的触发器。 Workfront和[!DNL Jira]项已链接。

完成Jira的[!DNL Workfront]配置后，在[!DNL Workfront]中创建或更新项以匹配触发器时，将在[!DNL Jira]中自动创建新项。\
创建和更新Workfront项目的Workfront用户不需要[!DNL Jira]许可证即可触发在[!DNL Jira]中创建项目。

有关定义自动创建Jira问题的触发器的更多信息，请参阅[为Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)配置 [!DNL Adobe Workfront] 。

>[!NOTE]
>
>通过将模板附加到项目，您可以自动创建[!DNL Jira]项。 如果模板包含的工作分配符合[!DNL Jira]触发器，则新任务将生成新的[!DNL Jira]问题。

自动将[!DNL Workfront]问题链接到[!DNL Jira]问题与自动将[!DNL Workfront]任务链接到[!DNL Jira]问题相同。

要自动将[!DNL Workfront]任务链接到[!DNL Jira]问题：

1. 确保您的[!DNL Jira]系统管理员已配置触发器，以便在分配[!DNL Workfront]项时自动创建[!DNL Jira]问题，然后使用允许您创建任务的访问级别登录到[!DNL Workfront]。

   有关访问任务的更多信息，请参阅[授予访问任务的权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。

1. 转到项目，然后在左侧面板中选择&#x200B;**[!UICONTROL 任务]** ![](assets/tasks-icon-in-left-panel-14x14.png)。

1. 单击&#x200B;**[!UICONTROL 新建任务]**

   或

   选择现有任务，然后单击&#x200B;**编辑**。

1. 指定或更新任务可用的任何字段。
1. 单击&#x200B;**[!UICONTROL 分配]**&#x200B;并将任务分配给在[!DNL Jira]集成中指定为触发器的用户、角色或团队。

1. 单击&#x200B;**保存更改**。

   将在Workfront中创建新任务。

   在新任务的&#x200B;**[!UICONTROL 更新]**&#x200B;区域中，有一个注释指示已在[!DNL Jira]中创建新问题。

1. （可选）单击指向Jira问题的链接以在Jira中打开。

   或

   单击&#x200B;**[!UICONTROL 详细信息]**&#x200B;部分的&#x200B;**[!UICONTROL 集成]**&#x200B;区域或任务或问题标题中的&#x200B;**[!UICONTROL 转到Jira]**&#x200B;链接，以打开[!DNL Jira]问题。

   您的系统或组管理员必须将[!UICONTROL 集成]字段添加到您的布局模板中，才能在任务或问题标题中显示该字段。 有关信息，请参阅[使用布局模板自定义对象标头](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

   任何[!DNL Jira]用户都可以立即开始处理从[!DNL Workfront]自动创建的项目，其更新将传输到[!DNL Workfront]，而无需[!DNL Workfront]的许可证即可完成此操作。

   只有您在[!DNL Workfront]加载项设置期间作为[!DNL Workfront]管理员配置的字段才会更新。

   有关在Workfront和Jira之间同步字段的更多信息，请参阅[为Jira配置Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)中的[为Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira)部分。

   >[!NOTE]
   >
   >从Workfront自动创建[!DNL Jira]问题时，该问题未分配给[!DNL Jira]中的任何人。

## 手动将[!DNL Jira]问题链接到[!DNL Workfront]个项目

在[!DNL Jira]和[!DNL Workfront]中创建相互独立的项后，您可以手动将[!DNL Jira]问题链接到现有的[!DNL Workfront]任务或问题。\
您无法手动将[!DNL Workfront]项从[!DNL Workfront]链接到现有[!DNL Jira]项。

>[!NOTE]
>
>如果[!DNL Jira]问题不位于未在[!DNL Workfront]集成中识别为触发器的项目上，则在与[!DNL Jira]内部部署集成时，无法手动将其链接到Workfront项。\
>有关为Workfront到Jira工作流设置触发器的更多信息，请参阅[自动将Workfront项目链接到Jira问题](#automatically-link-workfront-items-to-jira-issues)。

当链接[!DNL Workfront]和[!DNL Jira]项时，一项中的某些字段会在另一项中自动更新。\
有关更新链接项的更多信息，请参阅[在Jira和Adobe Workfront之间更新链接项](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md)。

要手动将[!DNL Jira]问题链接到[!DNL Workfront]项，请执行以下操作：

1. （视情况而定）登录到[!DNL Workfront]并找到要链接到[!DNL Jira]问题的问题或任务。
1. （视情况而定）从项的地址栏中，复制Workfront中项的&#x200B;**URL**。

   或

   从[!UICONTROL 详细信息]区域，复制Workfront中该项的&#x200B;**[!UICONTROL 参考编号]**。

   >[!NOTE]
   >
   >您必须拥有[!DNL Workfront]许可证才能登录到[!DNL Workfront]。 否则，[!DNL Workfront]用户必须提供此信息给您。

1. 在[!DNL Jira]中，导航到要手动链接到[!DNL Workfront]项目的问题。
1. 在[!DNL Workfront]右侧面板中，粘贴要链接到它的[!DNL Workfront]项的&#x200B;**URL**&#x200B;或&#x200B;**[!UICONTROL 参考号]**。

1. 单击&#x200B;**[!UICONTROL 链接]**。

   这两个项目将链接，[!DNL Workfront]右侧面板中填充了[!DNL Workfront]项目中的信息。

   以下[!DNL Workfront]字段默认显示在[!DNL Workfront]右侧面板的[!DNL Jira]中：

   * 项目的&#x200B;**[!UICONTROL Name]**：您可以通过单击面板中的名称来访问[!DNL Workfront]项目。
   * **[!UICONTROL 项目名称]**
   * 项目的&#x200B;**[!UICONTROL 状态]**
   * 项目的&#x200B;**[!UICONTROL 优先级]**
   * 创建日期[!DNL Workfront]
   * 项目的&#x200B;**[!UICONTROL 计划小时数]**
   * **[!UICONTROL 参考编号]**：您可以通过单击面板中的[!UICONTROL 参考编号]来访问[!DNL Workfront]项。

有关启用其他字段在右侧面板中显示的详细信息，请参阅[配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)中的[配置 [!DNL Jira] 和 [!DNL Workfront] 项](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization)之间的字段同步。 来自与集成关联的[!DNL Workfront]管理员的注释已发布在[!DNL Jira]问题的&#x200B;**[!DNL Workfront]**&#x200B;选项卡中，以确认已创建新的[!DNL Jira]项目。 该评论包含指向[!DNL Jira]问题的链接。

## 取消链接[!DNL Jira]和[!DNL Workfront]之间的项目

可以手动从[!DNL Jira]中取消链接[!DNL Jira]和[!DNL Workfront]之间的链接项。\
您无法取消与[!DNL Workfront]中对应项[!DNL Jira]的[!DNL Workfront]项目的链接。

您需要以下访问权限才能取消手动链接项目的链接：

* 您是手动链接项目的用户
* 您是[!DNL Jira]系统管理员

只有[!DNL Workfront]管理员可以取消自动链接项目的链接。

要从[!DNL Workfront]项中取消链接[!DNL Jira]问题，请执行以下操作：

1. 在[!DNL Jira]中，导航到链接到[!DNL Workfront]任务或问题的问题。
1. 转到[!DNL Workfront]右侧面板，单击&#x200B;**[!UICONTROL 取消链接]**&#x200B;图标，然后单击&#x200B;**[!UICONTROL 取消链接]**。

   以前链接的[!DNL Jira]和[!DNL Workfront]项现在已取消链接。 将来可能单独更新的任何字段、注释或文档，不会在另一个应用程序中的以前对应字段上更新。
