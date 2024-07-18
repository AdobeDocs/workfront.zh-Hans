---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Final
description: 2018.3发行版活动
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 Final

以下功能目前在“预览”或Beta中不可用，但将在R1中发布到“生产”环境：

## 从“我的工作区”(Workfront)为验证做出批准决策

现在，当用户将您添加到验证并授予审批者角色或查看者和审批者角色(来自独立的ProofHQ应用程序或使用Workfront中的自动工作流)时，审批请求将显示在“我的工作”区域的审批选项卡上。 然后，您可以直接从Workfront查看验证并做出批准决定。

有关如何使用自动工作流将用户添加到验证的信息，请参阅[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)中的[在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)。

有关如何从“我的工作”区域作出批准决策的信息，请参阅[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)中的[批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md)。 

## 我的工作区域(Workfront)内的验证审批报告

您现在可以基于验证审批对象创建报告。 通过此报告，您可以报告尚未做出决策的用户的“我的工作”区域中的验证审批。

验证审批报告包含以下信息：

* 已提交供审批的文档
* 审批者的姓名
* 校对版本
* 校样 ID
* 校对创建日期

在基于对象创建报告时，您可以访问此审批，如[创建自定义报告](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)中所述。

有关验证审批对象报告的详细信息，请参阅[了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)中的[了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分。

## 使用拖放功能自动生成文档验证的新版本(Workfront)

如果使用拖放方法添加需要校对的文档的新版本，则会自动生成校对。 校对的选项和工作流程与原始校对或以前的版本相同。

以前，当您添加文档的新版本时，新版本上不会自动生成验证，您必须为新版本重新生成验证。

当您使用文档更多菜单上传新版本时，验证不会自动生成。

欲了解更多信息，请参见  中的部分

## 允许所有验证用户直接从Workfront界面(Workfront)访问ProofHQ

现在，您可以让系统中的所有验证用户直接从Workfront界面无缝访问您的ProofHQ Premium帐户。 启用后，所有验证用户都会在全局导航栏中看到ProofHQ图标，将其定向到ProofHQ网站。

默认情况下不启用此选项。 要启用此选项，请联系Workfront技术支持并请求系统中的所有验证用户拥有此访问权限。

有关详细信息，请参阅以下位置的[从Adobe Workfront访问Workfront Proof](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)：  [从Adobe Workfront访问Workfront Proof](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md)。

在此更改之前，只有Workfront管理员才能从Workfront界面直接访问ProofHQ网站。

## 用于传出邮件的TLS安全连接的新选项(Workfront)

当您选择使用自己的电子邮件服务器管理Workfront通信时，您现在可以启用发送邮件以使用TLS安全连接。

在此增强功能之前，您只能通过SSL安全连接启用传出邮件。

有关配置传出邮件的详细信息，请参阅。

## 用于管理预览Sandbox环境中的电子邮件的新字段

Workfront现在禁用来自“预览沙盒”环境和“自定义刷新”环境的所有电子邮件通信。 如果要从“预览沙盒”或“自定义刷新”环境接收电子邮件通知，则必须在用户设置中启用此功能。

有关更多信息，请参阅以下信息：

* [在[Adobe Workfront预览沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)中的Adobe Workfront预览沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。

* [Adobe Workfront自定义刷新沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)中的“从自定义刷新沙盒接收电子邮件”

## Outlook for Office 365 (Workfront)

适用于Outlook 365的Workfront加载项现已可用。 

有关使用该加载项的更多信息，请参阅[将Workfront加载项与Outlook for Office 365一起使用。](https://support.workfront.com/hc/en-us/sections/205046167)

## 在移动设备应用程序(Workfront)中搜索

现在，您可以在移动应用程序中搜索对象，其方式与在Web应用程序中搜索类似。 新的搜索功能首先会查找最近使用的项目列表中的项目，以及之前已下载到移动设备的对象。 最近项目的列表与您在Web应用程序中看到的列表相同。

>[!NOTE]
>
>此功能将在2017年5月的第一个星期提供。

有关移动设备应用程序的更多信息，请参阅中的“在移动设备中搜索”部分。  

## 改进了移动设备应用程序中的帮助：Tutorials(Workfront)

从4月的移动设备版本开始，您将看到新的教程屏幕，以指导您完成移动设备体验。 当您首次登录移动设备应用程序并且首次使用某个功能时，您将看到一个简短教程，其中将说明该功能的工作原理。 第一次使用特定功能时，该教程仅显示一次。

有关移动设备应用程序的更多信息，请参阅。

## 在PDF文档中搜索(ProofHQ)

您现在可以在PDF文档、Office文档和静态网页内执行搜索。

有关更多信息，请参阅  [在验证中搜索内容](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md)。

## 更新了全局导航栏(ProofHQ)

与Workfront集成的ProofHQ Premium帐户现在可以在ProofHQ中看到对全局导航栏的以下改进：

* 新建用户个人资料图片 
* 更新外观

## 在自定义视图(ProofHQ)中包含其他信息

现在，您可以在自定义视图中包含以下附加信息：

* **收件人级别的数据**\
  您可以配置自定义视图以包含以下与收件人级别数据相关的列：角色、位置、电子邮件警报、我的截止日期、添加到验证的日期和收件人搜索。\
  有关详细信息，请参阅[在Workfront Proof证明中创建和管理自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)。
* **校对数据**\
  您可以配置自定义视图以包含以下与验证数据相关的列：注释计数（所有版本）、磁盘大小、验证类型、每个版本的文件数、注释附件数据（磁盘大小、文件名）以及按子文件夹过滤。\
  有关详细信息，请参阅[在Workfront Proof证明中创建和管理自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)。
* **与自动化工作流相关的暂存级别数据**\
  您可以配置自定义视图，使其包括以下与自动化工作流的各个阶段相关的列：SOCD状态、阶段截止日期、活动阶段名称、下一阶段名称、阶段名称和模板。\
  有关详细信息，请参阅[在Workfront Proof证明中创建和管理自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md)。

## 对验证报告（以前称为Analytics）的改进(ProofHQ)

报表功能（以前称为Analytics）包含以下改进：

* 新的默认报表类型：

   * 校对周转时间
   * 延迟审批百分比
   * 验证第一个活动时间
   * 评论和回复的数量

* 打印报表
* 更新外观

## 在预览环境中查看ProofHQ功能(ProofHQ)

发布到ProofHQ的功能将先在预览环境中进行测试，然后再发布到生产环境。

此在生产之前预览功能的新发布工作流将允许您为未来对ProofHQ生产环境的更新做更多准备。

有关ProofHQ预览环境的更多信息，请参阅[预览Sandbox测试环境 — Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md)。
