---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 配置JumpSeat集成
description: 您可以集成 [!DNL JumpSeat] 替换为 [!DNL Workfront] 创建自定义的产品内指南。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# 配置JumpSeat集成

您可以集成 [!DNL JumpSeat] 替换为 [!DNL Workfront] 创建自定义的产品内指南。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划*</strong></td> 
   <td> <p>[！UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td>[！UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>产品</strong></td> 
   <td>您必须拥有有效的 [!DNL JumpSeat] 计划。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p> 您必须是 [!DNL Workfront] 管理员。 有关的信息 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 先决条件

在开始之前，您必须

* 添加并激活 [!DNL Workfront] 作为应用程序 [!DNL JumpSeat]. 有关更多信息，请参阅 [如何添加或删除应用程序](https://support.jumpseat.io/article/how-to-add-an-application/).

## 配置 [!DNL JumpSeat] 集成

我们建议设置 [!DNL JumpSeat] “预览”和“生产”环境中的集成。

>[!TIP]
>
>您需要添加和激活两个单独的 [!DNL Workfront] 中的应用程序 [!DNL JumpSeat] — 一个用于预览，一个用于生产。 请参阅 [如何添加或删除应用程序](https://support.jumpseat.io/article/how-to-add-an-application/) 以了解更多信息。

配置 [!DNL JumpSeat] 集成：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]**.
1. 在左侧面板中，单击 **[!UICONTROL 系统]** > **[!UICONTROL [!DNL JumpSeat]集成]**.
1. 输入您的 **[!UICONTROL [!DNL JumpSeat]URL]**，有关更多详细信息，请参阅扩展图标 [!DNL JumpSeat].

   **示例：** [!DNL https]：//{mycompanyname}.jumpseat.io

1. 输入 **[!UICONTROL [!DNL JumpSeat]集成令牌]**. 您可以在 **[!UICONTROL 配置]** 页面位置 [!DNL JumpSeat].

   **示例：** 2到10美元BevsKeQ8....OYR.LurSg2U64O

1. 单击 **[!UICONTROL 测试配置]**.
1. 选择您是否希望集成 **[!UICONTROL 活动]** 或 **[!UICONTROL 不活动]**.

   >[!IMPORTANT]
   >
   >在步骤5中执行的配置测试必须通过，才能激活集成。

   ![JumpSeat集成页面](assets/jumpseat-integration-page.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

>[!TIP]
>
>有关配置的详细信息 [!DNL JumpSeat] 集成，请参见 [!DNL JumpSeat] 文档 [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
