---
product-area: workfront-integrations
keywords: google，doc，文档，工作表，幻灯片
navigation-topic: workfront-for-g-suite
title: 适用于Google Workspace的Workfront中的隐私和权限
description: 适用于Google Workspace的Workfront中的隐私和权限
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: 58543982fef6e7ba2d05787dc023a2099e47bbc7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 适用于Google Workspace的Workfront中的隐私和权限

>[!IMPORTANT]
>
>为了提供更稳定和可扩展的集成，我们正在使用Workfront自动化与集成(Fusion)转向一种现代、灵活的集成方法。 在此过渡过程中，以下适用于Google Workspace的Workfront功能在&#x200B;**2026年2月28日**&#x200B;之后将不可用：
>
>* 从Workfront访问Google Workspace功能
>
>* 从Gmail或Google日历网站面板查看和管理Workfront任务
>
>为了满足贵组织与Google Workspace的集成需求，我们建议使用Workfront自动化和集成。
>
>有关Workfront自动化和集成的概述，请参阅[Adobe Workfront Fusion概述](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview)。
>
>有关Google Workspace的Workfront自动化和集成模块的特定功能的信息，请参阅[Gmail模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)和[Google日历模块](https://experienceleague.adobe.com/zh-hans/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)。

由于客户隐私很重要，因此Adobe Workfront不会存储或收集通过Google插件应用程序的第三方授权产生的任何标识性客户数据。 Workfront for Google Workspace使用从Google API收到的信息并将其传输到任何其他应用程序将遵循[Google API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy)，包括“有限使用”要求。

我们需要以下权限，以便适用于Google Workspace的Workfront插件可以提供其最大价值：

* **当加载项运行时，查看您的电子邮件**： Workfront for Google Workspace插件可将电子邮件转换为Workfront中的新任务，并使用电子邮件的主题和正文自动填充该任务的标题和描述，从而使用户节省无数小时的重复工作。 插件还允许将您的电子邮件作为新评论发布到Workfront。 插件需要在加载项运行时查看您的电子邮件以传递此值。
* **作为Gmail加载项运行/不敏感**： Workfront需要权限才能在Gmail环境中运行Google Workspace加载项。 此插件需要Gmail环境才能正常运行，因此它需要`Run as a Gmail add-on / non-sensitive`权限。
* **当加载项运行时，查看您的电子邮件元数据**：为了改进工作流，Workfront for Google Workspace插件将确认电子邮件是否为Workfront通知，并识别Workfront通知的类型（新工作请求、审批请求、新评论等）。 插件需要`View your email message metadata when the add-on is running`权限才能传递此值。
* **插件需要作为日历加载项运行/不敏感**： Workfront for Google Workspace插件连接到您的日历，以便您能够查看任务对计划的影响。 插件需要`Run as a Calendar add-on / non-sensitive`权限才能执行此操作。
* **连接到外部服务权限：**&#x200B;最终，插件需要连接到Workfront API，这是插件值的骨干。 Workfront API是Google外部的服务，因此插件需要`Connect to an external service permission`才能使插件正常工作。

有关Adobe Workfront致力于客户隐私的更多信息，请参阅[Workfront隐私声明](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf)。

有关详细信息，请参阅[Google API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy)。
