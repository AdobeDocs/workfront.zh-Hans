---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 的 [!DNL Adobe Workfront] 自定义刷新沙盒环境
description: “自定义刷新”沙盒是一个环境，您可以在该环境中使用生产环境中的数据进行测试和工作。 它还非常适用于运行培训和确定设置功能。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1534'
ht-degree: 0%

---

# 的 [!DNL Adobe Workfront] 自定义刷新沙盒环境

“自定义刷新”沙盒是一个环境，您可以在该环境中使用生产环境中的数据进行测试和工作。 它还非常适用于运行培训和确定设置功能。

>[!NOTE]
>
>这与预览沙盒不同，预览沙盒也是一个测试环境，用于复制您的 [!DNL Workfront] 生产环境。
>
>* 新功能在生产中可用之前，会先在预览沙盒中引入。
>* 新功能在生产中可用之前，不会在“自定义刷新”沙盒中引入。
>
>  此外，获取预览沙盒不需要的自定义刷新沙盒也需要额外费用。
>
>  有关预览沙盒的更多信息，请参阅 [的 [!DNL Adobe Workfront] 预览沙盒环境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] 计划</td> 
   <td> <p>[!UICONTROL Business]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] 许可证</p> </td> 
   <td> <p>[!UICONTROL计划] </p> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">支持包</td> 
   <td> <p>[!UICONTROL Plus]、[!UICONTROL Preferred]或[!UICONTROL Enterprise]</p> <p>标准支持包没有访问“自定义刷新”沙盒的权限，但有权访问“预览”沙盒。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 刷新自定义刷新沙盒

自定义刷新沙盒包含您的实际生产数据，在您计划刷新数据之前，不会刷新该数据。 您可以安排随时刷新，这非常方便，每周频繁一次。

>[!NOTE]
>
>* 您无法安排当天的刷新。 例如，如果今天是6月1日，则您计划刷新的最早日期为6月2日。
>* 自定义刷新沙盒始终具有与生产环境相同的产品功能。 但是，当您刷新“自定义刷新沙盒”时，它仅保留登录屏幕背景颜色的品牌。 登录屏幕和导航栏徽标将重置为 [!DNL Workfront] 默认值，以及您在刷新之前修改的任何品牌图像都不会显示。
>




<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## 从生产环境访问自定义刷新沙盒 {#access-the-custom-refresh-sandbox-from-your-production-environment}

As a [!DNL Workfront] 管理员，您可以从生产环境访问“自定义刷新沙盒”。

>[!NOTE]
>
>如果您的帐户位于群集4（EMEA群集）上，则无法从生产环境访问您的自定义刷新沙盒。 有关在群集4上拥有帐户时如何访问自定义刷新沙盒的更多信息，请参阅 [访问群集4（EMEA帐户）上帐户的自定义刷新沙盒](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [访问群集4（EMEA帐户）上帐户的自定义刷新沙盒](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

要访问自定义刷新沙盒，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 系统]** >**[!UICONTROL 首选项]**.

1. 在 **[!UICONTROL 测试环境]** ，单击 **[!UICONTROL 沙盒1]** 或 **[!UICONTROL 沙盒2]**.

   您的支持包指定您是否有权访问一个或两个“自定义刷新”沙箱。

1. 使用您的自定义刷新沙盒凭据登录。

   自定义刷新沙盒凭据与生产凭据相同，除非自上次刷新自定义刷新沙盒以来您更改了生产凭据。 仅当发生刷新时才会同步登录。 它们不会自动同步。

   “自定义刷新”沙盒在屏幕顶部的横幅中显示版本以及上次刷新日期。 生产中的所有信息都可用，并可在刷新完成后使用。

## 使用URL访问自定义刷新沙盒 {#access-the-custom-refresh-sandbox-using-a-url}

任何用户都可以使用URL访问“自定义刷新”沙盒。

* [访问群集1、2、3和5上帐户的自定义刷新沙盒](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [访问群集4（EMEA帐户）上帐户的自定义刷新沙盒](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### 访问群集1、2、3和5上帐户的自定义刷新沙盒 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

根据您的支持包，您应该有权访问一个或两个自定义刷新沙箱。

要使用URL访问您的自定义刷新沙盒，请执行以下操作：

1. 如果您只有一个“自定义刷新”沙盒，请导航到此URL:

   https://companyname.sb01.workfront.com（旧URL）:https://cr1.attasksandbox.com/.)

   或者，如果您有两个自定义刷新沙盒，除了上述URL之外，您还可以转到以下URL以访问您的第二个自定义刷新沙盒：

   https://companyname.sb02.workfront.com（旧URL）:https://cr2.attasksandbox.com/)

1. 在登录屏幕上，使用“自定义刷新”沙盒凭据登录。
1. 自定义刷新沙盒凭据与生产凭据相同，除非自上次刷新自定义刷新沙盒以来您已更改了生产凭据。 仅当发生刷新时才会同步登录。 它们不会自动同步。

### 访问群集4（EMEA帐户）上帐户的自定义刷新沙盒 {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

如果 [!DNL Workfront] 帐户位于群集4（EMEA群集）上，则只能使用URL访问“自定义刷新”沙盒。 要了解您的帐户所在的群集，请联系我们的客户支持团队。

根据您的支持包，您应该有权访问一个或两个自定义刷新沙箱。

要使用URL访问您的自定义刷新沙盒，请执行以下操作：

1. 如果您只有一个“自定义刷新”沙盒，请导航到此URL:

   https://companyname.sb01.workfront.com（旧URL）:https://cr3.attasksandbox.com)

   或

   如果您有两个“自定义刷新”沙箱，请转到以下任一URL:

   https://companyname.sb01.workfront.com（旧URL）:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com（旧URL）:https://cr4.attasksandbox.com)

1. 在登录屏幕上，使用“自定义刷新”沙盒凭据登录。

   自定义刷新沙盒凭据与生产凭据相同，除非自上次刷新自定义刷新沙盒以来您已更改了生产凭据。 仅当发生刷新时才会同步登录。 它们不会自动同步。

## 计划刷新自定义刷新沙盒

>[!IMPORTANT]
>
>刷新的持续时间取决于刷新的数据的大小。 在刷新过程中，务必不要以任何方式使用自定义刷新沙盒环境（包括API调用和集成），因为这样会阻止沙盒刷新成功完成。 [!DNL Workfront] 将在自定义刷新沙盒环境开始之前禁用该环境，但您必须结束任何活动会话以确保沙盒刷新成功。

计划自定义刷新沙盒的刷新后，可通过单击 [!UICONTROL 取消] 的双曲余切值。 您还可以重新安排以后的时间。

>[!NOTE]
>
>您无法计划自动沙盒刷新。

要计划刷新客户刷新沙盒，请执行以下操作：

1. 登录到自定义刷新沙盒。
1. 单击 **[!UICONTROL 计划]** 在屏幕顶部的横幅中，从日历中选择日期。
1. 选择希望进行刷新的日期，然后单击 **[!UICONTROL 计划刷新]**.

## 从自定义刷新沙盒切换到生产

1. 登录到自定义刷新沙盒。

   有关访问自定义刷新沙盒的更多信息，请参阅 [从生产环境访问自定义刷新沙盒](#access-the-custom-refresh-sandbox-from-your-production-environment) 或 [使用URL访问自定义刷新沙盒](#access-the-custom-refresh-sandbox-using-a-url).

1. 单击 **[!UICONTROL 转到生产]** 在屏幕顶部的横幅中。

   请记住，在沙盒中完成的工作将不显示在 [!UICONTROL 生产] 环境中，因为数据传输是单向的，从生产环境传输到自定义刷新沙盒，而不是反向传输。

## 从自定义刷新沙盒接收电子邮件

[!DNL Workfront] 禁用来自“自定义刷新沙盒”环境的所有电子邮件通信。 如果要从“自定义刷新沙盒”环境接收电子邮件通知，则必须在用户设置中启用此功能。 有关在“自定义刷新沙盒”环境中启用电子邮件通知的更多信息，请参阅 [允许从预览沙盒环境发送电子邮件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>对于自定义刷新沙盒环境，将始终禁用移动设备应用程序上的报表交付和推送通知。 您和 [!DNL Workfront] 当您访问“自定义刷新沙盒”环境时，管理员可以为移动设备应用程序启用报表交付或推送通知。\
>有关生产环境的报表交付的更多信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。有关移动设备应用程序上生产环境的推送通知的更多信息，请参阅中的部分。

## 在自定义刷新沙盒中配置单点登录

如果要将自定义刷新沙盒配置为与单点登录解决方案配合使用，则可以通过将其与生产环境分开配置来实现这一点。 自定义刷新沙盒中的SSO配置与生产环境中的SSO配置无关。\
刷新自定义刷新沙盒时，不会从生产环境复制SSO信息，以覆盖自定义刷新沙盒配置。

在自定义刷新沙盒中配置单点登录的步骤与在生产环境中配置单点登录的步骤类似。\
有关配置的更多信息 [!DNL Workfront] 使用单点登录，请参阅 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>如果贵组织的 [!DNL Workfront] 实例已通过Adobe IMS启用。 如需详细信息，请咨询您的网络或IT管理员。

## 预期用途和可用性

[!DNL Workfront] 自定义刷新沙盒环境不适用于性能或负载测试。 而是使用这些环境来验证组织现有工作流的功能。

[!DNL Workfront] 自定义刷新沙盒环境将始终可用。 在正常工作时间内，对Workfront自定义刷新沙盒环境的任何停机将是在解决任何生产问题（如果存在）后立即的首要任务。 周末（星期六和星期日）的Workfront自定义刷新沙盒环境的任何中断都将得到解决，以便该环境在星期一的工作时间内运行。
