---
title: 使用项目协调员协作者
content-type: reference
description: 了解如何使用项目协调器，这是一个开箱即用的AI协作器，可监控项目状态并跟进逾期任务。
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 4%

---
# 使用项目协调员协作者

{{highlighted-preview-article-level}}

项目协调员是一个开箱即用的AI协作者，负责监控您的项目并通知利益相关者有关重要状态信息。

使用项目协调器不需要在Workfront之外配置代理。

有关配置项目协调器的说明，请参阅配置AI协作者一文中的[配置项目协调器](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)。

有关AI协作者的常规信息，请参阅[配置AI协作者](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>选择、Prime或Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[!UICONTROL 标准版]</p></td>
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>您必须具有项目的“管理”权限才能分配项目协调器。</td> 
  </tr>
  </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 项目协调员概述

项目协调员会监视您的项目并帮助使工作按计划进行。 当分配给项目时，会按管理员配置的时间表发送项目更新。 更新可能包括：

* 进度摘要
* 项目运行状况
* 过期或存在风险的任务或审批
* 缺少字段或分配

项目协调员还可以对项目及其任务进行评论。

管理员可配置发送更新的频率、发送时间以及接收更新的人员。

您还可以在项目更新中提及项目协调员，根据需要运行项目协调员。 项目协调员在提到它时运行，即使它没有安排在那个时间运行。

>[!NOTE]
>
>在正式发布之前，项目协调员的行为可能会发生变化。

## 将项目协调员添加到项目

管理员必须首先创建项目协调器，并将&#x200B;**项目协调器**&#x200B;字段添加到布局模板中的项目标头。 然后，该字段显示在项目标题中。

有关详细信息，请参阅[使用布局模板自定义对象标头](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

要将项目协调员分配给项目，请执行以下操作：

1. 转到要为其分配项目协调器的项目。
1. 在项目标题中，单击&#x200B;**项目协调器**&#x200B;字段。
1. 选择要分配的项目协调器。

   该窗口显示所选项目协调器的说明以及项目协调器执行的操作。
1. 单击&#x200B;**应用**。

## 通过提及项目协调员来运行项目协调员

除了其计划的更新外，您还可以随时通过将“项目协调器”@mentioning入项目更新来触发该协调器。 项目协调员一经提及，即刻运行，即使没有计划在此时运行。

提及项目协调员：

1. 转到已分配项目协调器的项目。
1. 打开项目的&#x200B;**更新**&#x200B;区域。
1. 在更新字段中，键入&#x200B;**@**&#x200B;并选择项目协调器。
1. 添加您的消息，然后发布更新。

   项目协调员运行并发布其响应。

>[!NOTE]
>
>必须先为项目分配项目协调器，然后才能使用@mention触发该项目。

## 配置项目协调器

有关配置项目协调器的说明，请参阅配置AI协作者一文中的[配置项目协调器](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator)。
