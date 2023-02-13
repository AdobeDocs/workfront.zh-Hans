---
navigation-topic: notifications
title: 允许从预览沙盒环境发送电子邮件
description: 如果要从“预览沙盒”环境接收电子邮件通知，则必须在登录“预览”时在用户设置中启用此功能。
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# 允许从预览沙盒环境发送电子邮件

[!UICONTROL Adobe Workfront] 禁用“预览”和“自定义刷新沙盒”环境中的所有电子邮件通信。 有关预览沙盒环境的信息，请参阅 [Adobe Workfront预览沙盒环境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). 有关自定义刷新沙盒环境的信息，请参阅 [Adobe Workfront自定义刷新沙盒环境](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

如果要从“预览沙盒”环境接收以下电子邮件通知，则在登录“预览”时，必须在用户设置中启用此功能：

* 由事件通知触发的电子邮件通知
* 提醒通知
* 自动延迟或提前提醒通知
* 电子邮件邀请

您可以为自己或您有权编辑的任何用户执行此操作。 有关编辑用户所需访问权限的更多信息，请参阅 [授予用户访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>对于预览沙盒环境，将始终禁用移动设备应用程序上的报表交付和推送通知。 您和 [!DNL Workfront] 当您访问预览沙盒环境时，管理员可以为移动设备应用程序启用报表交付或推送通知。
>
>有关报表投放的信息，请参阅 [报表交付概述](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Request]或更高版本，以更改您自己的设置</p> <p>[!UICONTROL Plan] ，为其他用户编辑设置</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>您必须具有以下任一项：</p> 
    <ul> 
     <li> <p>[!UICONTROL系统管理员]访问级别。</p> <p> 有关此访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p>在访问级别中，必须为[!UICONTROL Users]设置选择[!UICONTROL Edit]。 此外，对于[!UICONTROL用户]设置，在[!UICONTROL微调您的设置]下 <img src="assets/gear-icon-in-access-levels.png"> ，则必须启用[!UICONTROL创建]选项和两个[!UICONTROL用户管理员]选项中的至少一个选项。 </p> <p>如果您使用[!UICONTROL用户管理员（群组用户）]选项，则您必须是用户所属群组的群组管理员。</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>有关访问级别中[!UICONTROL用户]设置的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 启用从预览沙盒环境发送电子邮件的功能

1. 登录到预览沙盒环境。
1. 单击 [!DNL Adobe Workfront]. 然后，单击 **[!UICONTROL 更多]** 菜单和选择 **[!UICONTROL 编辑]**.

   或

   在 [!DNL Workfront] 并单击其名称。 然后，单击 **[!UICONTROL 更多]** 菜单和选择 **[!UICONTROL 编辑]**.

   或

   对于多个用户：单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **[!UICONTROL 用户]** ![](assets/users-icon-in-main-menu.png).  然后，选择多个用户并单击 **[!UICONTROL 编辑]**.

1. 单击 **[!UICONTROL 首选项]**.
1. 选择 **[!UICONTROL 从此测试环境接收电子邮件]**.

   >[!NOTE]
   >
   >如果您在生产环境中，则此选项不可用。

1. 单击 **[!UICONTROL 保存更改]**.
