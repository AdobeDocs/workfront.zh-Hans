---
navigation-topic: notifications
title: 启用从预览Sandbox环境的电子邮件投放
description: 如果您希望从预览Sandbox环境接收电子邮件通知，则必须在登录预览时在用户设置中启用此功能。
author: Courtney, Becky
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# 启用从预览Sandbox环境的电子邮件投放

[!UICONTROL Adobe Workfront]将禁用来自“预览”和“自定义刷新沙盒”环境的所有电子邮件通信。 有关预览沙盒环境的信息，请参阅[Adobe Workfront预览沙盒环境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)。 有关自定义刷新沙盒环境的信息，请参阅[Adobe Workfront自定义刷新沙盒环境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。

如果您希望从预览Sandbox环境接收以下电子邮件通知，则必须在登录预览时在用户设置中启用此功能：

* 事件通知触发的电子邮件通知
* 提醒通知
* 自动延迟或提前提醒通知
* 电子邮件邀请

您可以为自己或您有权编辑的任何用户执行此操作。 有关编辑用户所需访问权限的详细信息，请参阅[授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)。

>[!NOTE]
>
>对于“预览Sandbox”环境，始终禁用移动应用程序上的报表交付和推送通知。 当您访问“预览Sandbox”环境时，您和[!DNL Workfront]管理员都不能为移动设备应用程序启用报告交付或推送通知。
>
>有关报告传递的信息，请参阅[报告传递概述](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> 
   <p>参与者或更高版本以更改您自己的设置</p> <p>用于编辑其他用户的设置的标准</p> 
   或
   <p> 请求或更高版本以更改您自己的设置</p> <p>计划编辑其他用户的设置</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>[!UICONTROL 系统管理员]访问级别。</p> </li> 
     <li> <p>在访问级别中，必须为[!UICONTROL 用户]设置选择[!UICONTROL 编辑] 。 对于[!UICONTROL 用户]设置，在[!UICONTROL 微调设置] <img src="assets/gear-icon-in-access-levels.png">下，必须启用[!UICONTROL 创建]选项以及两个[!UICONTROL 用户管理]选项中的至少一个。 </li> 
     <li>如果您使用[!UICONTROL 用户管理员（组用户）]选项，您必须是用户所属组的组管理员。</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 从预览Sandbox环境启用电子邮件投放

1. 登录到预览Sandbox环境。
1. 单击[!DNL Adobe Workfront]右上角的配置文件图片。 然后，单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单并选择&#x200B;**[!UICONTROL 编辑]**。

   或

   在[!DNL Workfront]中搜索用户并单击其名称。 然后，单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单并选择&#x200B;**[!UICONTROL 编辑]**。

   或

   对于多个用户：单击Workfront右上角的&#x200B;**[!UICONTROL 主菜单]**&#x200B;图标![主菜单图标](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 用户]** ![用户图标](assets/users-icon-in-main-menu.png)。  然后，选择多个用户并单击&#x200B;**[!UICONTROL 编辑]**。

1. 单击&#x200B;**[!UICONTROL 首选项]**。
1. 选择&#x200B;**[!UICONTROL 从此测试环境接收电子邮件]**。

   >[!NOTE]
   >
   >如果您在生产环境中，则此选项不可用。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。
