---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: 此 [!DNL Adobe Workfront] 预览沙盒环境
description: 预览沙盒是一个测试环境，可用作实时环境的副本。 Workfront每周末都会刷新一次。 在星期五添加到您的实时环境的数据会在下星期一之前显示在您的预览沙盒中。 所有支持包都可以访问此沙盒。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# 此 [!DNL Adobe Workfront] 预览沙盒环境

有两个测试环境 [!DNL Workfront] 是的副本 [!DNL Workfront] 生产环境：

* 预览沙盒

   预览沙盒是一个测试环境，用作实时环境的副本，每个周末更新者 [!DNL Workfront]. 在星期五添加到您的实时环境的数据会在下星期一之前显示在您的预览沙盒中。

   所有支持包都有权访问预览沙盒。

* 自定义刷新沙盒

   自定义刷新沙盒是一个单独的测试环境，由您手动刷新。 获取自定义刷新沙盒需要额外付费。 有关此环境的更多信息，请参阅 [此 [!DNL Adobe Workfront] 自定义刷新沙盒环境](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[！UICONTROL Standard]支持包</strong> </p> </th> 
   <th> <p><strong>[！UICONTROL Plus]、[！UICONTROL Preferred]和[！UICONTROL Enterprise]支持包</strong> </p> </th> 
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

“预览沙盒”用作一个环境，贵组织中的用户可以在其中安全地测试和使用生产环境中的数据，而不会影响生产环境。

预览沙盒包含您的实际生产数据；但是，它每个周末都会刷新，以便数据最多可以在生产环境之后一周。 在上次刷新后创建的项目一直位于预览沙盒环境中，直到下次刷新为止。

数据单向流动，从生产到预览，而不是反向。 始终计划刷新“预览”环境 [!DNL Workfront] 每个周末。

预览沙盒还允许 [!DNL Workfront] 在准备部署到生产环境之前，在安全的环境中部署新功能。 您可以测试新功能并提供 [!DNL Workfront] 通过访问预览Sandbox对其功能提出反馈。 因此，尽管您的数据每周都会刷新，但预览沙盒的代码始终比生产代码先于。

预览环境非常适合运行培训、测试新功能和确定设置功能。

>[!NOTE]
>
>当您访问预览沙盒时，请注意屏幕顶部的蓝色横幅。 当您在此环境中工作时，无法删除横幅。
>
>您正在访问的环境的名称（预览）和代码的发行版本将显示在横幅上。 单击 **[!UICONTROL 查看新增功能]** 以了解有关该版本的信息。
>
>![](assets/preview-banner-nwe-350x161.png)

## 访问预览沙盒

默认情况下，作为 [!DNL Workfront] 管理员，您有权访问 [!UICONTROL 预览] 沙盒环境。 如果您无法访问 [!UICONTROL 预览] 如本节所述的沙盒环境，请联系 [!DNL Workfront] 管理员或我们的客户支持团队。

* [从访问预览沙盒 [!DNL Workfront] 界面](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [使用URL访问预览沙盒](#accessing-the-preview-sandbox-using-a-url)

### 从访问预览沙盒 [!DNL Workfront] 界面 {#accessing-the-preview-sandbox-from-the-workfront-interface}

As a [!DNL Workfront] 管理员，您可以通过以下方式访问预览沙盒 [!DNL Workfront] 界面。

要访问预览沙盒，请执行以下操作：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) （位于的右上角） [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 系统]** > **[!UICONTROL 首选项]**.

1. 在 **[!UICONTROL 测试环境]** 部分，单击 **[!UICONTROL 沙盒预览]**.

1. 使用预览凭据登录。

   这些凭据应与生产凭据相同，除非您在预览刷新后在生产环境中更改了这些凭据。 仅在刷新时同步登录。 它们不会自动同步。

### 使用URL访问预览沙盒 {#accessing-the-preview-sandbox-using-a-url}

* [访问群集1、2、3和5上帐户的预览沙盒](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [访问群集4上帐户的预览沙盒（EMEA帐户）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### 访问群集1、2、3和5上帐户的预览沙盒 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

“预览”沙盒的URL为： `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>如果您有链接到预览Sandbox的旧URL的书签，请记下此更改并更新书签中的URL。

要使用URL登录“预览Sandbox”，请执行以下操作：

1. 导航到此URL： `https://companyname.preview.workfront.com/`.

   如果您是EMEA客户，并且您的帐户位于群集4上，请参阅部分 [访问群集4上帐户的预览沙盒（EMEA帐户）](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) 本文章中。

1. 使用预览凭据登录。

   您的预览凭据应与生产凭据相同，除非您在预览刷新后在生产环境中更改了这些凭据。 仅在刷新时同步登录。 它们不会自动同步。

#### 访问群集4上帐户的预览沙盒（EMEA帐户） {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

要使用URL登录“预览Sandbox”，请执行以下操作：

1. 导航到此URL： `https://companyname.preview.workfront.com/`.

   您还可以通过以下方式访问预览沙盒： [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. 使用预览凭据登录。

   您的预览凭据应与生产凭据相同，除非您在预览刷新后在生产环境中更改了这些凭据。 仅在刷新时同步登录。 它们不会自动同步。

## 从预览沙盒接收电子邮件

Workfront禁用来自“预览Sandbox”环境的所有电子邮件通信。 如果要从“预览沙盒”环境接收电子邮件通知，则必须在用户设置中启用此功能。 有关在预览沙盒环境中启用电子邮件通知的更多信息，请参阅 [启用从“预览Sandbox”环境投放电子邮件](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>“预览”沙盒环境始终禁用移动应用程序上的报告交付和推送通知。 无论您还是 [!DNL Workfront] 当您访问“预览沙盒”环境时，管理员可以为移动设备应用程序启用报告交付或推送通知。
>
>有关生产环境的报告交付的更多信息，请参阅 [报表交付概述](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## 单点登录 (SSO)

如果您使用的是SSO，请与我们的客户支持团队合作，确保已正确配置它，以便您可以使用SSO凭据登录到 [!UICONTROL 预览] 沙盒。 如果您的初始登录失败，请联系您的常规支持联系人或 [!DNL Workfront] 管理员寻求帮助。

有关单点登录的详细信息，请参阅 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 在预览沙盒中配置单点登录

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未载入的组织。 [!DNL Adobe Admin Console]. 如果您的组织已载入 [!DNL Adobe Admin Console]，无需执行任何操作。
>
>对于因贵组织是否已载入到以下版本而不同的过程，请参见 [!DNL Adobe Admin Console]，请参见 [基于平台的管理差异([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe业务平台])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


如果您希望将预览沙盒配置为与单点登录解决方案一起使用，可以通过与生产环境分开配置来实现这一点。 预览沙盒中的SSO配置与生产环境中的SSO配置无关。

当您的预览沙盒（每周末）刷新时，不会从生产环境复制SSO信息以覆盖预览沙盒配置。

在预览沙盒中配置单点登录的步骤与在生产环境中配置单点登录的步骤类似。

有关配置的更多信息 [!DNL Workfront] 使用SSO，请参见 [Adobe Workfront中的单点登录概述](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## 预览环境性能和可用性

[!DNL Workfront] 预览环境不适用于性能或负载测试。 相反，使用这些环境验证您组织现有工作流的功能功能。

[!DNL Workfront] 预览环境旨在始终可用。

对的任何中断 [!DNL Workfront] 在解决任何生产问题（如果存在）之后，立即优先在常规工作时间内预览环境。

对的任何中断 [!DNL Workfront] 将处理周末（星期六和星期日）的预览环境，以便环境在星期一的营业时间运行。
