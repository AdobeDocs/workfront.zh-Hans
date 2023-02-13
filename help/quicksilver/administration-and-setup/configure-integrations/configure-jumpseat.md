---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 配置JumpSeat集成
description: 您可以集成 [!DNL JumpSeat] with [!DNL Workfront] 创建自定义的产品内指南。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# 配置JumpSeat集成

您可以集成 [!DNL JumpSeat] with [!DNL Workfront] 创建自定义的产品内指南。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>产品</strong></td> 
   <td>您必须具有活动 [!DNL JumpSeat] 计划。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p> 你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 先决条件

在开始之前，您必须

* 添加和激活 [!DNL Workfront] 作为 [!DNL JumpSeat]. 有关更多信息，请参阅 [如何添加或删除应用程序](https://support.jumpseat.io/article/how-to-add-an-application/).

## 配置 [!DNL JumpSeat] 集成

我们建议设置 [!DNL JumpSeat] 集成。

>[!TIP]
>
>您需要添加并激活两个单独的 [!DNL Workfront] 应用程序 [!DNL JumpSeat] — 一个用于预览，一个用于生产。 请参阅 [如何添加或删除应用程序](https://support.jumpseat.io/article/how-to-add-an-application/) 以了解更多信息。

配置 [!DNL JumpSeat] 集成：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]**.
1. 在左侧面板中，单击 **[!UICONTROL 系统]** > **[!UICONTROL [!DNL JumpSeat]集成]**.
1. 输入 **[!UICONTROL [!DNL JumpSeat]URL]**.

   **示例：** [!DNL https]://{mycompanyname}.jumpseat.io

1. 输入 **[!UICONTROL [!DNL JumpSeat]集成令牌]**. 您可以在 **[!UICONTROL 配置]** 页面 [!DNL JumpSeat].

   **示例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 单击 **[!UICONTROL 测试配置]**.
1. 选择是否希望集成 **[!UICONTROL 活动]** 或 **[!UICONTROL 不活动]**.

   >[!IMPORTANT]
   >
   >必须通过在步骤5中执行的配置测试，才能激活集成。

   ![JumpSeat集成页面](assets/jumpseat-integration-page.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。
