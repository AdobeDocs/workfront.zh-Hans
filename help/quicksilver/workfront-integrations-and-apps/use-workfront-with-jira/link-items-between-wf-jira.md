---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: 链接项目之间 [!DNL Adobe Workfront] 和 [!DNL Jira]
description: 您可以链接 [!DNL Jira] 问题 [!DNL Adobe Workfront] 自动或手动执行任务或问题。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f533c9000c14d5692c87987973eb0b1d6665229d
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 0%

---

# 链接项目之间 [!DNL Adobe Workfront] 和 [!DNL Jira]

您可以链接 [!DNL Jira] 问题 [!DNL Adobe Workfront] 自动或手动执行任务或问题。

中只有一个项目 [!DNL Workfront] 可链接到 [!DNL Jira]. 您永远无法链接一个 [!DNL Workfront] 项目至多个 [!DNL Jira] 问题，也不是问题 [!DNL Jira] 多个问题 [!DNL Workfront] 项目。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 计划]</a>*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] 许可证概述</a>*</td> 
   <td> <p>计划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira访问</td> 
   <td> <p>系统管理员访问权限</p> <p><b>重要信息</b>

我们建议您在 [!DNL Jira] 和 [!DNL Workfront] 专门用于此集成，而不是使用可能附加到用户的现有集成。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注释</b>

如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

在您关联项目之前 [!DNL Workfront] 和 [!DNL Jira]，您必须

* 安装 [!DNL Workfront] 表示 [!DNL Jira]

   有关安装Workfront for Jira的说明，请参阅 [安装Adobe Workfront for Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* 配置 [!DNL Workfront] 为吉拉

   有关为Jira配置Workfront的说明，请参阅 [为Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## 自动链接 [!DNL Workfront] 项目 [!DNL Jira] 问题

As a [!DNL Workfront] 管理员，您可以定义触发器，以在 [!DNL Jira] 每当任务或 [!DNL Workfront]. Workfront和 [!DNL Jira] 项目会变为关联。

完成 [!DNL Workfront] 对于Jira，当在 [!DNL Workfront] 为与触发器匹配，会在 [!DNL Jira].\
创建和更新Workfront项目的Workfront用户不需要 [!DNL Jira] 用于触发在 [!DNL Jira].

有关定义触发器以自动创建Jira问题的更多信息，请参阅  [配置 [!DNL Adobe Workfront] 为吉拉](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>您可以创建 [!DNL Jira] 模板来自动删除项目。 如果模板包含的任务分配满足 [!DNL Jira] 触发器，新任务将生成新 [!DNL Jira] 问题。

自动链接 [!DNL Workfront] 问题 [!DNL Jira] 问题与自动链接 [!DNL Workfront] 任务 [!DNL Jira] 问题。

自动链接 [!DNL Workfront] 任务 [!DNL Jira] 问题：

1. 确保 [!DNL Jira] 系统管理员已配置触发器以自动创建 [!DNL Jira] 问题 [!DNL Workfront] 分配项目，然后登录到 [!DNL Workfront] 具有允许您创建任务的访问级别。

   有关任务访问权限的详细信息，请参阅 [授予对任务的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. 转到项目并选择 **[!UICONTROL 任务]** ![](assets/tasks-icon-in-left-panel-14x14.png) 中。

1. 单击 **[!UICONTROL 新任务]**

   或

   选择现有任务，然后单击 **编辑**.

1. 指定或更新任何可用于任务的字段。
1. 单击 **[!UICONTROL 分配]** 并将任务分配给在 [!DNL Jira] 集成。

1. 单击 **保存更改**.

   将在Workfront中创建新任务。

   在 **[!UICONTROL 更新]** 新任务的区域中，有一条注释，指示已在 [!DNL Jira].

   ![WF_confirmation_that_Jira_issue_was_created.png](assets/wf-confirmation-that-jira-issue-was-created-350x43.png)

1. （可选）单击指向Jira问题的链接以在Jira中将其打开。

   或

   单击 **[!UICONTROL 去吉拉]** 链接 **[!UICONTROL 集成]** 区域 **[!UICONTROL 详细信息]** ，以打开 [!DNL Jira] 问题。

   您的系统或组管理员必须将 [!UICONTROL 集成] 字段，以将其显示在任务或问题标题中。 有关信息，请参阅 [使用布局模板自定义对象标头](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   任意 [!DNL Jira] 用户可以立即开始处理从 [!DNL Workfront] 而他们的更新将转移至 [!DNL Workfront] 无需 [!DNL Workfront] 这样做。

   只有作为 [!DNL Workfront] 在 [!DNL Workfront] 加载项已更新。

   有关在Workfront和Jira之间同步字段的更多信息，请参阅 [为Jira配置Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) 部分  [为Jira配置Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >的 [!DNL Jira] 问题未分配给 [!DNL Jira] 自动从Workfront创建时。

## 手动链接 [!DNL Jira] 问题 [!DNL Workfront] 项目

在中创建项目后 [!DNL Jira] 和 [!DNL Workfront]相互独立，您可以手动链接 [!DNL Jira] 问题 [!DNL Workfront] 任务或问题。\
您无法手动链接 [!DNL Workfront] 项目自 [!DNL Workfront] 到现有 [!DNL Jira] 项目。

>[!NOTE]
>
>如果 [!DNL Jira] 未在 [!DNL Workfront] 集成使用时，您无法将其手动链接到Workfront项目 [!DNL Jira] 内部部署。\
>有关为Workfront到Jira工作流设置触发器的更多信息，请参阅 [自动将Workfront项目链接到Jira问题](#automatically-link-workfront-items-to-jira-issues).

When [!DNL Workfront] 和 [!DNL Jira] 项目已关联，则其中一个项目的某些字段可以在另一个项目上自动更新。\
有关更新链接项目的更多信息，请参阅 [更新Jira和Adobe Workfront之间的链接项目](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

手动链接 [!DNL Jira] 问题 [!DNL Workfront] 项目：

1. （视情况而定）登录到 [!DNL Workfront] 并查找要链接到的问题或任务 [!DNL Jira] 问题。
1. （视情况而定）从项目的地址栏中，复制 **URL** 在Workfront。

   或

   从 [!UICONTROL 详细信息] 面积 ![](assets/details-icon-in-left-panel.png)，复制 **[!UICONTROL 参考编号]** 在Workfront。

   >[!NOTE]
   >
   >您必须具有 [!DNL Workfront] 登录许可证 [!DNL Workfront]. 否则， [!DNL Workfront] 用户必须向您提供此信息。

1. 在 [!DNL Jira]，导航到要手动链接到 [!DNL Workfront] 项目。
1. 在 [!DNL Workfront] 右面板，粘贴 **URL** 或 **[!UICONTROL 参考编号]** 的 [!DNL Workfront] 链接到该项目的项目。\
   ![manually_link_items_Jira_WF.png](assets/new-manually-link-items-jira-631x394.png)

1. 单击 **[!UICONTROL 链接]**.

   这两个项目会链接，并且 [!DNL Workfront] 右侧面板中填充了 [!DNL Workfront] 项目。

   以下 [!DNL Workfront] 字段在中可见 [!DNL Jira]，默认情况下，在 [!DNL Workfront] 右面板：

   * 的 **[!UICONTROL 名称]** 项目：您可以访问 [!DNL Workfront] 项目。
   * **[!UICONTROL 项目名称]**
   * 的 **[!UICONTROL 状态]** 项目的
   * 的 **[!UICONTROL 优先级]** 项目的
   * 创建日期 [!DNL Workfront]
   * 的 **[!UICONTROL 计划小时数]** 项目的
   * 的 **[!UICONTROL 参考编号]**:您可以访问 [!DNL Workfront] 项目 [!UICONTROL 参考编号] 中。

有关如何在右侧面板中显示其他字段的更多信息，请参阅 [在之间配置字段同步 [!DNL Jira] 和 [!DNL Workfront] 项目](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) 部分 [配置 [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). 来自 [!DNL Workfront] 与集成关联的管理员将发布在 **[!DNL Workfront]** 选项卡 [!DNL Jira] 确认新 [!DNL Jira] 项目已创建。 注释包含指向 [!DNL Jira] 问题。

![Jira_confirmation_of_the_Jira_issue_created_Workfront_tab.png](assets/new-jira-confirmation-jira-issue-created-workfront-tab-1096x533.png)

## 取消项目之间的链接 [!DNL Jira] 和 [!DNL Workfront]

之间的链接项目 [!DNL Jira] 和 [!DNL Workfront] 可以手动从中取消链接 [!DNL Jira].\
无法取消链接 [!DNL Workfront] 项目 [!DNL Jira] 对应 [!DNL Workfront].

要取消手动链接的项目，您需要以下访问权限：

* 您是手动链接项目的用户
* 您是 [!DNL Jira] 系统管理员

仅a [!DNL Workfront] 管理员可以取消链接自动链接的项目。

取消链接 [!DNL Jira] 来自 [!DNL Workfront] 项目：

1. 在 [!DNL Jira]，导航到链接到 [!DNL Workfront] 任务或问题。
1. 转到 [!DNL Workfront] 右侧面板，然后单击 **[!UICONTROL 取消链接]** 图标，然后单击 **[!UICONTROL 取消链接]**.\
   ![Jira_WF_unlink_icon.png](assets/new-jira-wf-unlink-icon-631x394.png)\
   之前链接的 [!DNL Jira] 和 [!DNL Workfront] 项目现已取消关联。 将来可能单独更新这些字段、评论或文档的任何字段、评论或文档都不会针对其他应用程序中先前的相应字段、评论或文档进行更新。
