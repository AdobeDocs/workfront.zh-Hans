---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3集成和移动增强功能
description: 此页面介绍了2019.3版本中所做的所有更改集成和移动设备增强。 该版本在2019年8月19日当周的生产环境中提供。
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3集成和移动增强功能

此页面介绍了2019.3版本中所做的所有更改集成和移动设备增强。 该版本在2019年8月19日当周的生产环境中提供。

有关2019.3中所做所有更改的列表，请参阅[2019.3版本活动概述](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md)。

## 在MS OneDrive集成中支持共享项目

现在，您可以将共享的OneDrive文件和文件夹链接到Workfront对象。 反过来，您可以在Workfront中将文件上传到OneDrive中的共享文件夹。

有关详细信息，请参阅[从外部应用程序链接文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)一文中的[将外部文档链接到Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)、[链接一个或多个外部文件夹](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder)和[更新文档并将文档从Workfront链接到外部云提供商](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents)部分。

有关信息，请参阅文章[从外部应用程序链接文档](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)中的[将外部文档链接到Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)部分。

## 所有Workfront登录均需要域规范

现在，如果尚未在Workfront URL中指定域，则所有Workfront登录都要求用户指定域。 要求提供此信息可让您的Workfront实例更加安全。 此外，如果您实施的Workfront具有多个实例，则此增强功能允许您向实施中的每个Workfront实例添加同一用户。

此更改可能会同时影响用户登录和API集成：

* **用户登录**

  如果您的公司域未包含在Workfront URL中，那么除了用户名和密码字段外，您现在还会在登录屏幕上看到一个新的域字段。

  对于大多数客户，无需进行更改，因为域信息已包含在Workfront URL中。 例如，“*域*.my.workfront.com”。

* **API集成**

  如果您将任何API代码发送到不包含您的域名的地址，则该API代码将不再有效。

有关详细信息，请参阅[登录到Adobe Workfront](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md)。

## 在iOS上使用移动应用程序将任务和问题转化为项目

您现在可以在iOS上的Workfront移动应用程序中，将各个任务和问题转化为项目。

## 使用指纹或面容ID登录到移动设备应用程序

根据您的设备，您可以选择使用指纹或面容ID技术登录到Workfront移动应用程序。 当您登录移动设备应用程序时，系统会询问您是否要使用手机支持的身份验证方法进行登录。

有关如何管理此功能的更多信息，请参阅[适用于iOS的Adobe Workfront](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md)或[适用于Android的Adobe Workfront](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md)。

## 用于在移动设备上自动注销用户的新设置

为了让您和您的公司更加安全，Workfront移动应用程序会在15天不活动后自动注销。 Workfront管理员可以在Web应用程序中的“设置”>“系统”>“首选项”下自定义此时间限制。

有关详细信息，请参阅[配置系统安全首选项](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)。

## 移动设备应用程序登录时需要域

作为一项安全改进，Workfront移动应用程序现在要求您提供域（如果您未使用单点登录凭据登录）。

>[!NOTE]
>
>iOS发布时间：2019年6月12日
>
>可用生产：2019年6月17日

## 在iOS上使用移动设备应用程序删除对象

>[!NOTE]
>
>此功能已在2019年8月19日当周的iOS应用商店中提供。

您现在可以在iOS移动设备应用程序中删除任务、问题和时间表等对象。 您必须对对象具有正确的权限才能将其删除。

## 在移动应用程序中按停止的项目进行筛选

>[!NOTE]
>
>此功能将在2019年8月19日这一周在iOS和Android的应用商店中提供。

我们在移动应用程序的“项目”选项卡上添加了“停止的项目”作为过滤器选项。

## 使用移动应用程序重置密码

如果您忘记了密码，则可以使用Workfront Mobile应用程序重置密码。 点按忘记密码？ 并按照屏幕上的提示操作。 您不能在移动应用程序上重置SSO密码。

## 移动的新外观

我们添加了以下外观和感觉改进，以增强您在Workfront移动设备应用程序中的体验。

* 将以下内容从“详细信息”页面的顶部栏移至屏幕上更突出的区域：

   * 加号图标现在位于屏幕的左下角
   * 现在，用于开始处理项目的复选标记是屏幕中上角的“处理项目”按钮

* 您现在可以通过点按“详细信息”页面底部的显示更多来查看附加的自定义表单。
* 更改了用于提交任务、问题和请求的页面外观。

