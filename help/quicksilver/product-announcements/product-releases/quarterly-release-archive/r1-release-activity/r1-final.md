---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1最终
description: 以下功能目前在“预览”或“测试版”中不可用，但将发布到R1 - EDIT ME中的“生产”环境。
author: Luke
feature: Product Announcements
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# R1最终

以下功能目前在“预览”或“测试版”中不可用，但将发布到R1的“生产”环境：

## 从我的工作区域(Workfront)做出校样的批准决定

现在，当用户将您添加到校样并授予“审批者”角色或“审批者和审批者”角色(从独立的ProofHQ应用程序或通过在Workfront中使用自动工作流)时，批准请求会显示在“我的工作”区域的“批准”选项卡中。 然后，您可以直接从Workfront查看校样并对校样做出批准决策。

有关如何使用自动工作流将用户添加到校样的信息，请参阅 [在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [在Adobe Workfront中共享验证](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

有关如何从“我的工作”区域做出批准决策的信息，请参阅 [批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [批准工作](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## 报告“我的工作区”内的校对批准(Workfront)

您现在可以基于校样批准对象创建报表。 通过此报表，您可以报告用户“我的工作”区域（其中尚未做出决策）的校样批准情况。

校样批准报告包含以下信息：

* 已提交以供审批的文件
* 审批者的姓名
* 校样版本
* 校对 ID
* 校样创建日期

在基于对象创建报告时，您可以访问此批准，如 [创建自定义报表](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

有关校样批准对象报表的更多信息，请参阅 [了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 部分 [了解Adobe Workfront中的对象](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 使用拖放功能自动生成文档校样的新版本(Workfront)

使用拖放方法添加需要校对的文档新版本时，将自动生成校样。 校样的选项和工作流与原始校样或之前版本相同。

以前，在添加文档的新版本时，校样不会在新版本上自动生成，您必须为新版本重新生成校样。

使用“文档更多”菜单上传新版本时，不会自动生成校样。

有关更多信息，请参阅

## 使所有校对用户能够直接从Workfront界面(Workfront)访问ProofHQ

现在，您可以让系统中所有校样用户都能够直接从Workfront界面无缝访问您的ProofHQ Premium帐户。 启用后，所有打样的用户都会在全局导航栏中看到一个ProofHQ图标，将他们引导至ProofHQ站点。

默认情况下，未启用此选项。 要启用此选项，请联系Workfront技术支持，并请求系统中所有校对用户拥有此访问权限。

有关更多信息，请参阅 [从Adobe Workfront访问Workfront校样](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [从Adobe Workfront访问Workfront校样](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

在进行此更改之前，只有Workfront管理员才能从Workfront界面直接访问ProofHQ站点。

## 新增了外发邮件的TLS安全连接选项(Workfront)

当您选择使用自己的电子邮件服务器管理Workfront通信时，您现在可以启用“外发邮件”以使用TLS安全连接。

在此增强之前，您只能通过SSL安全连接来启用“外发邮件”。

有关配置传出邮件的更多信息，请参阅。

## 在预览沙盒环境中管理电子邮件的新字段

Workfront现在会禁用“预览沙盒”环境和“自定义刷新”环境中的所有电子邮件通信。 如果要从预览沙盒或自定义刷新环境接收电子邮件通知，则必须在用户设置中启用此功能。

有关更多信息，请参阅以下信息：

* [Adobe Workfront预览沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [Adobe Workfront预览沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* 在 [Adobe Workfront自定义刷新沙盒环境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Office 365展望(Workfront)

适用于Outlook 365的Workfront外接程序现已可用。 

有关使用加载项的更多信息，请参阅 [将Workfront外接程序与Outlook for Office 365结合使用。](https://support.workfront.com/hc/en-us/sections/205046167)

## 在移动设备应用程序中搜索(Workfront)

您现在可以在移动设备应用程序中搜索对象，其方式与在Web应用程序中搜索类似。 新的搜索功能首先会查找“最近的项目”列表中的项目，以及之前已下载到移动设备的对象。 “最近项目”列表与您在Web应用程序中看到的列表相同。

>[!NOTE]
>
>此功能将于2017年5月的第一周提供。

有关移动设备应用程序的更多信息，请参阅  

## 改进了移动设备应用程序中的帮助：Tutorials(Workfront)

从4月的移动版本开始，您将看到新的教程屏幕，可引导您完成移动体验。 当您首次登录移动设备应用程序，并且首次使用功能时，您将看到一个简短教程，其中说明了该功能的工作方式。 本教程仅显示一次，这是您首次使用特定功能时显示的一次。

有关移动设备应用程序的更多信息，请参阅。

## 在PDF文档中搜索(ProofHQ)

您现在可以在PDF文档、Office文档和静态网页中执行搜索。

有关更多信息，请参阅  [在校样中搜索内容](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## 更新了全局导航栏(ProofHQ)

现在，与Workfront集成的ProofHQ Premium帐户在ProofHQ内的全局导航栏中有以下改进：

* 新用户配置文件图片 
* 更新了外观

## 在自定义视图(ProofHQ)中包含其他信息

您现在可以在自定义视图中包含以下其他信息：

* **收件人级别数据**\
   您可以配置自定义视图以包含与收件人级别数据相关的以下列：角色、位置、电子邮件警报、我的截止时间、添加到校样的日期和收件人搜索。\
   有关更多信息，请参阅 [在Workfront校样中创建和管理自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **校对数据**\
   您可以配置自定义视图以包含与校样数据相关的以下列：注释计数（所有版本）、磁盘大小、校样类型、每个版本的文件数、注释附件数据（磁盘大小、文件名）以及按子文件夹过滤。\
   有关更多信息，请参阅 [在Workfront校样中创建和管理自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **与自动化工作流相关的阶段级数据**\
   您可以配置自定义视图，以包含与自动化工作流的各个阶段相关的以下列：SOCD状态、阶段截止时间、活动阶段名称、下一阶段名称、阶段名称和模板。\
   有关更多信息，请参阅 [在Workfront校样中创建和管理自定义视图](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## 对校对报表（以前称为Analytics）(ProofHQ)的改进

报表功能（以前称为Analytics）包含以下改进：

* 新的默认报表类型：

   * 证明周转时间
   * 延迟批准百分比
   * 首次活动时间校样
   * 评论和回复数

* 打印报表
* 更新了外观

## 在预览环境(ProofHQ)中查看ProofHQ功能

发布到校样HQ的功能将首先在预览环境中测试，然后再发布到生产环境。

通过这个新的工作流，您可以在生产之前先发布预览功能，为将来更新ProofHQ生产环境做出更多准备。

有关“校样HQ预览”环境的更多信息，请参阅 [预览沙盒测试环境 — Workfront校样](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
