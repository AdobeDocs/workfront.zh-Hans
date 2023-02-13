---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 的 [!DNL Adobe Workfront] 预览沙盒环境
description: 预览沙盒是一个测试环境，可用作实时环境的副本。 Workfront每周末都会刷新一次。 星期五添加到实时环境的数据将在下周一之前显示在预览沙盒中。 所有支持包都有权访问此沙盒。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '1299'
ht-degree: 0%

---

# 的 [!DNL Adobe Workfront] 预览沙盒环境

有两个测试环境 [!DNL Workfront] 是 [!DNL Workfront] 生产环境：

* 预览沙盒

   “预览沙盒”是一个测试环境，用作实时环境的副本，每周末由 [!DNL Workfront]. 星期五添加到实时环境的数据将在下周一之前显示在预览沙盒中。

   所有支持包都有权访问“预览沙盒”。

* 自定义刷新沙盒

   自定义刷新沙盒是一个单独的测试环境，由您手动刷新。 获取“自定义刷新”沙盒需要额外付费。 有关此环境的更多信息，请参阅 [的 [!DNL Adobe Workfront] 自定义刷新沙盒环境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard]支持包</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus]、[!UICONTROL Preferred]和[!UICONTROL Enterprise]支持包</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>预览沙盒</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>自定义刷新沙盒</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## 预览沙盒

“预览”沙盒用作一个环境，在该环境中，组织中的用户可以安全地测试和处理来自生产环境的数据，而不会影响生产环境。

预览沙盒包含您的实际生产数据；但是，它会每周末刷新一次，以便数据最多可比生产环境滞后一周。 自上次刷新后创建的项目将在“预览沙盒”环境中，直到进行以下刷新。

数据从“生产”单向流向“预览”，而不是反向流动。 预览环境的刷新始终由 [!DNL Workfront] 每个周末。 有关刷新的具体日期和时间的更多信息，请转到 [status.adobe.com](https://status.adobe.com/).

预览沙盒还允许 [!DNL Workfront] 要在安全环境中部署新功能，请先将新功能部署到生产环境。 您可以测试新功能并提供 [!DNL Workfront] 通过访问预览沙盒，对其功能提供反馈。 因此，尽管您的数据每周都会刷新，但预览沙盒的代码始终位于生产代码之前。

预览环境非常适合运行培训、测试新功能并确定设置功能。

>[!NOTE]
>
>访问预览沙盒时，请注意屏幕顶部的蓝色横幅。 在此环境中工作时，无法删除横幅。
>
>您正在访问（预览）的环境的名称以及代码的发布版本将显示在横幅上。 单击 **[!UICONTROL 查看新增功能]** 以了解有关该版本的信息。
>
>![](assets/preview-banner-nwe-350x161.png)

## 访问预览沙盒

默认情况下，作为 [!DNL Workfront] 管理员，您有权访问 [!UICONTROL 预览] 沙盒环境。 如果您无法访问 [!UICONTROL 预览] 沙盒环境（如本节所述），请联系您的 [!DNL Workfront] 管理员或我们的客户支持团队。

* [从 [!DNL Workfront] 界面](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [使用URL访问预览沙盒](#accessing-the-preview-sandbox-using-a-url)

### 从 [!DNL Workfront] 界面 {#accessing-the-preview-sandbox-from-the-workfront-interface}

As a [!DNL Workfront] 管理员，您可以通过 [!DNL Workfront] 界面。

要访问预览沙盒，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 系统]** > **[!UICONTROL 首选项]**.

1. 在 **[!UICONTROL 测试环境]** ，单击 **[!UICONTROL 沙盒预览]**.

1. 使用预览凭据登录。

   这些凭据应与生产凭据相同，除非在发生预览刷新后在生产中更改了它们。 仅当发生刷新时才会同步登录。 它们不会自动同步。

### 使用URL访问预览沙盒 {#accessing-the-preview-sandbox-using-a-url}

* [访问群集1、2、3和5上帐户的预览沙盒](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [访问群集4上帐户的预览沙盒（EMEA帐户）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### 访问群集1、2、3和5上帐户的预览沙盒 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

以前，您通过转到 [https://companyname.attasksandbox.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.attasksandbox.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNGTfPKCDnAylzkclNwdSuEXksLFRg).

不再支持此URL，并且尚未将其重定向到预览沙盒环境的新URL。 预览沙盒的新正确URL是： [https://companyname.preview.workfront.com/](https://www.google.com/url?q=https%3A%2F%2Fcompanyname.preview.workfront.com%2F&amp;sa=D&amp;sntz=1&amp;usg=AFQjCNFZQYw9VWjr2tuvQLfSJHneqJj_PQ).

>[!NOTE]
>
>如果您的书签链接到预览沙盒的旧URL，请注意此更改，并更新书签中的URL。

要使用URL登录“预览”沙盒，请执行以下操作：

1. 导航到以下URL: [[!DNL https]://companyname.preview.workfront.com/](https://companyname.preview.workfront.com/)

   如果您是EMEA客户，并且您的帐户位于群集4上，请参阅部分 [访问群集4上帐户的预览沙盒（EMEA帐户）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) 在本文中。

1. 使用预览凭据登录。

   您的预览凭据应与生产凭据相同，除非在发生预览刷新后您在生产中更改了它们。 仅当发生刷新时才会同步登录。 它们不会自动同步。

#### 访问群集4上帐户的预览沙盒（EMEA帐户） {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

要使用URL登录“预览”沙盒，请执行以下操作：

1. 导航到以下URL: `https://companyname.preview.workfront.com/`.

   您还可以通过以下路径访问预览沙盒： [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. 使用预览凭据登录。

   您的预览凭据应与生产凭据相同，除非在发生预览刷新后您在生产中更改了它们。 仅当发生刷新时才会同步登录。 它们不会自动同步。

## 从预览沙盒接收电子邮件

Workfront会禁用“预览沙盒”环境中的所有电子邮件通信。 如果要从预览沙盒环境接收电子邮件通知，则必须在用户设置中启用此功能。 有关在预览沙盒环境中启用电子邮件通知的更多信息，请参阅 [允许从预览沙盒环境发送电子邮件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>对于预览沙盒环境，将始终禁用移动设备应用程序上的报表交付和推送通知。 您和 [!DNL Workfront] 当您访问预览沙盒环境时，管理员可以为移动设备应用程序启用报表交付或推送通知。
>
>有关生产环境的报表交付的更多信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## 单点登录 (SSO)

如果您使用单点登录(SSO)，请与我们的客户支持团队合作，确保正确配置了SSO，以便您能够使用SSO凭据登录到 [!UICONTROL 预览] 沙盒。 如果初始登录失败，请联系您的常规支持联系人或 [!DNL Workfront] 管理员以寻求帮助。

有关单点登录的更多信息，请参阅 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 在预览沙盒中配置单点登录

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入到 [!DNL Adobe Admin Console]. 如果贵组织已载入 [!DNL Adobe Admin Console]，则无需执行任何操作。
>
>有关根据贵组织是否已载入到 [!DNL Adobe Admin Console]，请参阅 [基于平台的管理差异([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe业务平台])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


如果要将预览沙盒配置为与单点登录解决方案配合使用，则可以通过将其与生产环境分开进行配置。 预览沙盒中的SSO配置与生产环境中的SSO配置无关。

当预览沙盒刷新（每个周末）时，SSO信息不会从生产环境中复制，以覆盖预览沙盒配置。

在预览沙盒中配置单点登录的步骤与在生产环境中配置单点登录的步骤类似。

有关配置的更多信息 [!DNL Workfront] 使用单点登录，请参阅 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 预览环境性能和可用性

[!DNL Workfront] 预览环境不适用于性能或负载测试。 而是使用这些环境来验证组织现有工作流的功能。

[!DNL Workfront] 预览环境旨在始终可用。

任何 [!DNL Workfront] 在解决任何生产问题（如果存在）后，在正常工作时间内的预览环境将是第一个优先级。

任何 [!DNL Workfront] 周末（星期六和星期日）的预览环境将得到满足，以便环境在星期一的工作时间内运行。
