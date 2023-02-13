---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 提交 [!DNL Adobe Workfront] 请求 [!DNL Salesforce] 对象
description: 安装后 [!DNL Adobe Workfront] 表示 [!DNL Salesforce], you can submit [!DNL Workfront] 请求 [!DNL Salesforce] 机会和帐户。 经典和闪电体验框架中均存在此功能。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# 提交 [!DNL Adobe Workfront] 请求 [!DNL Salesforce] 对象

安装后 [!DNL Adobe Workfront for Salesforce]，您可以提交 [!DNL Workfront] 请求 [!DNL Salesforce] 机会和帐户。 此功能同时存在于 [!DNL Classic] 和 [!DNL Lightning Experience] 框架。

## 访问要求

您必须具有以下访问权限才能使用本文中描述的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 计划*</p></td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 许可证*</p></td> 
   <td> <p>[!UICONTROL计划]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

提交 [!DNL Workfront] 来自 [!DNL Salesforce] 机会或帐户确保您在环境中具有以下功能：

* 您的 [!DNL Workfront] 管理员已安装 [!DNL Workfront for Salesforce].\
   有关安装的详细信息 [!DNL Workfront for Salesforce]，请参阅 [安装 [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* 您的 [!DNL Workfront] 管理员已添加 [!DNL Workfront] 的 [!UICONTROL 机会] 和 [!UICONTROL 帐户] 页面布局。\
   有关添加 [!DNL Workfront] 到页面布局的部分，请参阅 [配置 [!DNL Adobe Workfront] 部分 [!DNL Salesforce] 用户](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 您拥有 [!DNL Workfront] 帐户，您可以从登录到该帐户 [!DNL Workfront] 部分。\
   登录后，您可以看到 [!UICONTROL 新请求] 选项卡，您可以在此处开始输入请求。

## 提交 [!DNL Workfront] 请求 [!DNL Salesforce]

1. 在Salesforce中，转到Opportunity或Account 。
1. 转到 [!DNL Workfront] 中。
1. 在 **[!UICONTROL 新请求]** 选项卡，在 **[!UICONTROL 选择请求类型]** 下拉菜单。

   您可以看到您有权在Workfront中查看的相同请求队列。

1. 开始为您的请求填写可用字段。

   从提交请求 [!DNL Salesforce] 等同于在 [!DNL Workfront] Web应用程序。

   >[!NOTE]
   >
   >使用 [!DNL Workfront] 插件 [!DNL Salesforce] 暂时不可用。

   继续执行 [创建和提交 [!DNL Adobe Workfront] 请求](../../manage-work/requests/create-requests/create-submit-requests.md).

1. 单击 **[!UICONTROL 提交]**.

## 查看 [!DNL Workfront] 请求

1. 转到 [!DNL Salesforce].
1. 转到 **[!DNL Workfront]** 中。

   >[!NOTE]
   >
   >根据 [!DNL Workfront] 管理员配置了此部分，可能具有不同的名称。

1. 选择 **[!UICONTROL 已提交的请求]** 选项卡。

   您可以在此选项卡中查看您或其他人从此机会或帐户提交的所有请求。在Web应用程序中提交到此请求队列的请求不会显示在 [!DNL Salesforce].

   >[!NOTE]
   >
   >在Web应用程序中，提交到此请求队列的请求不会显示在Salesforce的此列表中。

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   您可以查看有关已提交请求的以下信息：

   * 请求名称(在 [!UICONTROL 主题] column)
   * 参考号
   * 请求类型
   * 状态
   * 日期提交
   * 按名称请求
   * 分配给名称\

      此信息在 [!DNL Workfront]，则此列表中也会更新该内容。

1. （可选）单击请求的名称以在中将其打开 [!DNL Workfront].

1. （可选）单击 **[!UICONTROL 转到[!DNL Salesforce]]** 访问问题源自Workfront以下区域的Opportunity或Account :

   * 在 [!UICONTROL 详细信息] 部分
   * 单击 [!UICONTROL 打开摘要] ![](assets/summary-panel-icon.png) 中。
   * 在问题标题中，当 [!UICONTROL 集成] 字段。 您的系统或组管理员必须将 [!UICONTROL 集成] 字段，以查看问题标题中的转到Salesforce链接。 有关更多信息，请参阅 [使用布局模板自定义对象标头](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >的 [!UICONTROL 转到Salesforce] 链接对所有 [!DNL Workfront] 可以查看问题的用户。 您必须具有 [!DNL Salesforce] 帐户 [!DNL Salesforce] 记录问题的机会或帐户。
