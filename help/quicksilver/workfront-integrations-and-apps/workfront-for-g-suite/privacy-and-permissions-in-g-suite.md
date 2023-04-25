---
product-area: workfront-integrations
keywords: google，doc，document，sheet，幻灯片
navigation-topic: workfront-for-g-suite
title: Workfront for G Suite中的隐私和权限
description: Workfront for G Suite中的隐私和权限
author: Becky
feature: Workfront Integrations and Apps
exl-id: abb8ffa1-1da6-46dd-a929-18b17014839a
source-git-commit: bd9fb14b99886f4a514c4d37ad9d93be7a051858
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Workfront for G Suite中的隐私和权限

由于客户隐私很重要，因此Adobe Workfront不会存储或收集因第三方授权Google插件应用程序而导致的任何可识别客户数据。 Workfront for G Suite将使用从Google API收到的信息并将其传输到任何其他应用程序时，将遵循 [Google API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy)，包括“有限使用”要求。

我们需要以下权限，以便Workfront for G Suite插件能够发挥最大价值：

* **运行加载项时查看电子邮件**:Workfront for G Suite插件可将电子邮件转换为Workfront中的新任务，并自动使用电子邮件的主题和正文填充任务的标题和描述，从而可以为用户节省无数小时的重复工作。 插件还允许将您的电子邮件作为新评论发布到Workfront。 当加载项运行以传递此值时，插件需要查看您的电子邮件。
* **作为Gmail加载项/非敏感**:需要Workfront for G Suite加载项的权限才能在Gmail环境中正常运行。 此插件需要Gmail环境才能正常工作，因此需要 `Run as a Gmail add-on / non-sensitive` 权限。
* **运行加载项时查看电子邮件元数据**:为了改进工作流，Workfront for G Suite插件会确认电子邮件是否为Workfront通知，并标识Workfront通知的类型（新工作请求、批准请求、新评论等）。 插件需要 `View your email message metadata when the add-on is running` 提供此值的权限。
* **插件需要“作为日历加载项运行”/“不敏感”**:Workfront for G Suite插件可连接到您的日历，以便您可以查看任务对计划的影响情况。 插件需要 `Run as a Calendar add-on / non-sensitive` 执行此操作的权限。
* **连接到外部服务权限：** 最终，插件需要连接到Workfront API，而API是插件价值的支柱。 Workfront API是Google外部的一项服务，因此插件需要 `Connect to an external service permission` 以使插件正常工作。

有关Adobe Workfront致力于客户隐私的更多信息，请参阅 [Workfront的隐私声明](https://www.adobe.com/content/dam/cc/en/legal/terms/enterprise/pdfs/Privacy-Notice-and-Privacy-Shield-Statement-Adobe-Workfront.pdf).

有关更多信息，请参阅 [Google API服务用户数据策略](https://developers.google.com/terms/api-services-user-data-policy).
