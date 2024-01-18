---
title: 23.2资源管理方面的改进
description: 23.2资源管理方面的改进
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 23.2资源管理方面的改进

本页介绍了23.2版本对“预览”环境所做的所有资源管理增强功能。 这些增强功能将在23.2版本的生产环境中提供。

有关23.2发行周期中此时可用的所有更改列表，请参阅 [23.2发行版概述](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## 引入“工作时间”字段以准确计算用户容量

>[!NOTE]
>
>预览版本： 2023年2月16日；计划生产版本： 2023年3月2日

为了使资源管理者能够准确地计算用户的可用性，并计算用户投入到实际项目相关工作的时间，我们在Adobe Workfront中引入了“工作时间”概念。

在创建或编辑用户档案时，您可以为每个用户定义“工作时间”字段的值。 有关更多信息，请参阅 [编辑用户配置文件](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

“工作时间”字段表示用户可用于实际工作的相当于全职(FTE)时间的百分比，不包括开销。 工作时间必须为介于0和1之间的小数。 例如，实际工作的20%可用性为0.2。

该字段的默认值为1，表示用户将其整个FTE用于实际的项目相关工作。

作为本次更新的结果，Workfront将使用以下公式计算用户可用性，具体取决于您在“资源管理”首选项区域中的选择：

* 默认计划：
* 用户容量= [（计划小时数 — 计划例外） * FTE — 休息时间] *工作时间
* 用户计划：
* 用户能力=（计划小时数 — 计划例外 — 休息时间）*工作时间。

有关更多信息，请参阅 [配置 [!UICONTROL 资源管理] 偏好设置](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[观看此功能的视频演示](https://video.tv.adobe.com/v/3415608/){target=_blank}
