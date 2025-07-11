---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: ' [!DNL Adobe Workfront] 自定义刷新沙盒环境'
description: 自定义刷新沙盒是一种您可以使用生产环境中的数据进行测试和工作的环境。 此外，它还是运行培训和确定设置功能的理想选择。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 7549c9699a86b6f87e5562efd7e586be282c5619
workflow-type: tm+mt
source-wordcount: '1763'
ht-degree: 0%

---

# [!DNL Adobe Workfront]自定义刷新沙盒环境

自定义刷新沙盒是一种您可以使用生产环境中的数据进行测试和工作的环境。 此外，它还是运行培训和确定设置功能的理想选择。

>[!NOTE]
>
>这与预览沙盒不同，预览沙盒也是复制[!DNL Workfront]生产环境的测试环境。
>
>* 在沙盒在生产中可用之前，先在预览沙盒中引入新功能。
>* 在自定义刷新沙盒中引入新功能后，这些功能才可在生产中使用。
>
>  此外，获取预览Sandbox不需要的自定义刷新Sandbox会额外产生成本。
>
>  有关预览沙盒的更多信息，请参阅[预览Sandbox环境 [!DNL Adobe Workfront] ](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 计划</td> 
   <td> <p>[！UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 许可证</p> </td> 
   <td> <p>[！UICONTROL计划] </p> <p>您必须是[!DNL Workfront]管理员。 有关[!DNL Workfront]管理员的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">支持包</td> 
   <td> <p>[！UICONTROL Plus]、[！UICONTROL Preferred]或[！UICONTROL Enterprise]</p> <p>标准支持包无权访问自定义刷新沙盒，但有权访问预览沙盒。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 刷新自定义刷新沙盒

自定义刷新沙盒包含您的实际生产数据，在您计划它刷新之前，它不会刷新。 您可以随时安排刷新时间，方便您使用，每周刷新一次。

>[!NOTE]
>
>* 您不能计划当天的刷新。 例如，如果今天是6月1日，则您可以计划刷新的最早日期是6月2日。
>* 根据用户的群集（美国的群集在夜间进行刷新），计划的刷新在夜间某个时间发生。 由于队列中的其他客户以及刷新了多少数据，因此特定时间不可预测。 如果队列有许多大客户，则刷新可能要到当天晚些时候或第二天才能运行。
>* 您的自定义刷新沙盒始终具有与生产环境相同的产品功能。 但是，当您刷新自定义刷新沙盒时，它仅保留登录屏幕背景颜色的品牌。 登录屏幕和导航栏徽标将重置为[!DNL Workfront]默认值，并且在刷新之前修改的任何品牌推广图像都不会显示。
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 从生产环境访问自定义刷新沙盒 {#access-the-custom-refresh-sandbox-from-your-production-environment}

作为[!DNL Workfront]管理员，您可以从生产环境访问“自定义刷新沙盒”。

>[!NOTE]
>
>如果您的帐户位于集群4 （EMEA集群）上，则无法从生产环境中访问自定义刷新沙盒。 有关在群集4上拥有帐户时如何访问自定义刷新沙盒的详细信息，请参阅[访问群集4上帐户的自定义刷新沙盒（EMEA帐户）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [访问群集4上帐户的自定义刷新沙盒（EMEA帐户）](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)。

要访问您的自定义刷新沙盒，请执行以下操作：

1. 单击&#x200B;**[!UICONTROL 右上角的]**&#x200B;主菜单![图标](assets/main-menu-icon.png)主菜单图标[!DNL Adobe Workfront]，然后单击&#x200B;**[!UICONTROL 设置]**![齿轮设置图标](assets/gear-icon-settings.png)。

1. 单击&#x200B;**[!UICONTROL 系统]** >**[!UICONTROL 首选项]**。

1. 在&#x200B;**[!UICONTROL 测试环境]**&#x200B;部分中，单击&#x200B;**[!UICONTROL 沙盒1]**&#x200B;或&#x200B;**[!UICONTROL 沙盒2]**。

   您的支持包指定您有权访问一个还是两个自定义刷新沙盒。

1. 使用自定义刷新沙盒凭据登录。

   您的自定义刷新沙盒凭据与生产凭据相同，除非自上次刷新自定义刷新沙盒以来您更改了生产凭据。 只有在刷新时才会同步登录。 它们不会自动同步。

   自定义刷新沙盒在屏幕顶部的横幅中显示版本以及上次刷新日期。 刷新完成后，生产中的所有信息都可用并准备就绪。

## 使用URL访问自定义刷新沙盒 {#access-the-custom-refresh-sandbox-using-a-url}

任何用户都可以使用URL访问自定义刷新沙盒。

* [访问群集1、2、3和5上帐户的自定义刷新沙盒](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [访问群集4（EMEA帐户）上的帐户的自定义刷新沙盒](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### 访问群集1、2、3和5上帐户的自定义刷新沙盒 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

根据您的支持包，您应该可以访问一两个自定义刷新沙盒。

要使用URL访问自定义刷新沙盒，请执行以下操作：

1. 如果您只有一个自定义刷新沙盒，请导航到此URL：

   `https://companyname.sb01.workfront.com` （旧URL：`https://cr1.attasksandbox.com/`。）

   或者，除了上述URL之外，如果您有两个自定义刷新沙盒，则还可以转到以下URL以访问第二个自定义刷新沙盒：

   `https://companyname.sb02.workfront.com` （旧URL：`https://cr2.attasksandbox.com/`）

1. 在登录屏幕上，使用自定义刷新沙盒凭据登录。
1. 自定义刷新沙盒凭据与生产凭据相同，除非自自定义刷新沙盒上次刷新后更改了生产凭据。 只有在刷新时才会同步登录。 它们不会自动同步。

### 访问群集4（EMEA帐户）上的帐户的自定义刷新沙盒 {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

如果[!DNL Workfront]帐户位于群集4 （EMEA群集）上，则只能使用URL访问自定义刷新沙盒。 要了解您的帐户所在的群集，请与我们的客户支持团队联系。

根据您的支持包，您应该可以访问一两个自定义刷新沙盒。

要使用URL访问自定义刷新沙盒，请执行以下操作：

1. 如果您只有一个自定义刷新沙盒，请导航到此URL：

   `https://companyname.sb01.workfront.com` （旧URL：`https://cr3.attasksandbox.com`）

   或

   如果您有两个自定义刷新沙盒，请转到以下任一URL：

   `https://companyname.sb01.workfront.com` （旧URL：`https://cr3.attasksandbox.com`）

   `https://companyname.sb02.workfront.com` （旧URL：`https://cr4.attasksandbox.com`）

1. 在登录屏幕上，使用自定义刷新沙盒凭据登录。

   自定义刷新沙盒凭据与生产凭据相同，除非自自定义刷新沙盒上次刷新后更改了生产凭据。 只有在刷新时才会同步登录。 它们不会自动同步。

## 安排自定义刷新沙盒的刷新

>[!IMPORTANT]
>
>刷新的持续时间取决于要刷新的数据的大小。 在刷新过程中，务必要不要以任何方式（包括API调用和集成）使用自定义刷新沙盒环境，因为这将阻止沙盒刷新成功完成。 [!DNL Workfront]将在自定义刷新沙盒环境开始之前禁用该环境，但您必须结束任何活动会话以确保沙盒刷新成功。

在计划刷新自定义刷新沙盒后，您可以通过单击页面顶部的[!UICONTROL 取消]来取消它。 您也可以稍后重新计划该日期。

>[!NOTE]
>
>您无法计划自动沙盒刷新。

要计划客户刷新沙盒的刷新，请执行以下操作：

1. 登录到您的自定义刷新沙盒。
1. 在屏幕顶部的横幅中单击&#x200B;**[!UICONTROL 计划]**，然后从日历中选择一个日期。
1. 选择要进行刷新的日期，然后单击&#x200B;**[!UICONTROL 计划刷新]**。

## 从自定义刷新沙盒切换到生产

1. 登录到您的自定义刷新沙盒。

   有关访问自定义刷新沙盒的详细信息，请参阅[从生产环境访问自定义刷新沙盒](#access-the-custom-refresh-sandbox-from-your-production-environment)或[使用URL访问自定义刷新沙盒](#access-the-custom-refresh-sandbox-using-a-url)。

1. 在屏幕顶部的横幅中单击&#x200B;**[!UICONTROL 转到生产环境]**。

   请记住，在沙盒中完成的工作在[!UICONTROL 生产]环境中不可见，因为数据传输是单向的，从生产环境传输到自定义刷新沙盒，而不是反向传输。

## 从自定义刷新沙盒接收电子邮件

[!DNL Workfront]禁用来自自定义刷新沙盒环境的所有电子邮件通信。 如果要从“自定义刷新沙盒”环境接收电子邮件通知，则必须在用户设置中启用此功能。 有关在自定义刷新沙盒环境中启用电子邮件通知的更多信息，请参阅[从预览沙盒环境中启用电子邮件投放](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md)。

>[!NOTE]
>
>对于“自定义刷新沙盒”环境，移动应用程序上的报表交付和推送通知始终处于禁用状态。 当您访问“自定义刷新沙盒”环境时，您和[!DNL Workfront]管理员都不能为移动设备应用程序启用报告交付或推送通知。\
>有关生产环境的报表投放的更多信息，请参阅[报表投放概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。有关生产环境的移动应用程序推送通知的更多信息，请参阅中的部分。

## 在自定义刷新沙盒中配置单点登录

如果要将自定义刷新沙盒配置为使用单点登录解决方案，您可以将其与生产环境分开配置来完成此操作。 自定义刷新沙盒中的SSO配置与生产环境中的SSO配置无关。\
在刷新自定义刷新沙盒时，不会从生产环境中复制SSO信息以覆盖自定义刷新沙盒配置。

在自定义刷新沙盒中配置单点登录的步骤与在生产环境中配置单点登录的步骤类似。\
有关使用SSO配置[!DNL Workfront]的更多信息，请参阅[Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)。

>[!NOTE]
>
>如果您组织的[!DNL Workfront]实例已在Adobe IMS中启用，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

## 项目时间线的自动重新计算

重新计算时间表使经理能够了解项目之外的力量对项目时间表的影响。 项目时间线是指项目的计划和预计日期。

作为Workfront管理员，您可以配置Workfront何时自动重新计算项目时间表。 Workfront可以每晚或在项目范围更改时重新计算项目时间线，或同时重新计算两者。

有关信息，请参阅[配置项目的时间表重新计算](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md)。

对于自定义刷新沙盒环境，将禁用夜间重新计算，并且不会自动重新计算项目时间线。 您必须手动重新计算自定义刷新沙盒环境的项目时间线。 有关信息，请参阅[重新计算项目时间表](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md)。


## 预期用途和可用性

* [!DNL Workfront]自定义刷新沙盒环境不适用于性能或负载测试。 相反，使用这些环境验证组织现有工作流的功能性。

* 涉及文档的工作流应侧重于流程，而不是负载测试。 沙盒环境中不支持大文件。

* [!DNL Workfront]自定义刷新沙盒环境旨在始终可用。 在解决任何生产问题（如果存在）之后，在常规工作时间内对Workfront自定义刷新沙盒环境的任何中断都将成为首要任务。 将解决周末（周六和周日）对Workfront自定义刷新沙盒环境的任何中断，以便该环境在星期一的营业时间运行。

* 验证在自定义刷新沙盒环境中不可用。
