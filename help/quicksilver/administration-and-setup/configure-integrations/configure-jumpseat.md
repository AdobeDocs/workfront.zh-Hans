---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 配置 JumpSeat 集成
description: You can integrate [!DNL JumpSeat] with [!DNL Workfront] to create custom, in-product guidance.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Courtney, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 14%

---

# 配置 JumpSeat 集成

You can integrate [!DNL JumpSeat] with [!DNL Workfront] to create custom, in-product guidance.

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table>
  <tr>
   <td>Adobe Workfront 包
   </td>
    <p>工作流 Ultimate</p>
   <td> <p>Prime or Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront 许可证
   </td>
   <td>标准
   <p>规划</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>产品
   </td>
   <td>You must have an active [!DNL JumpSeat] plan.
   </td>
  </tr>
   <tr>
   <td>访问级别配置
   </td>
   <td>You must be a [!DNL Workfront] administrator.
   </td>
  </tr>
</table>

有关此表中信息的详细信息，请参阅[Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

Before you begin, you must

* Add and activate [!DNL Workfront] as an application in [!DNL JumpSeat]. For more information, see [How To Add Or Delete An Application](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>If you are on the Adobe Unified Experience, you must use the following Application URL: `.workfront.adobe.com`.



## Configure the [!DNL JumpSeat] integration

我们建议在您的预览环境和生产环境中设置[!DNL JumpSeat]集成。

>[!TIP]
>
>You need to add and activate two separate [!DNL Workfront] applications in [!DNL JumpSeat]—one for Preview and one for Production. See [How To Add Or Delete An Application](https://support.jumpseat.io/article/how-to-add-an-application/) for more information.

To configure the [!DNL JumpSeat] integration:

{{step-1-to-setup}}

1. In the left panel, click **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat]Integration]**.
1. Enter your **[!UICONTROL [!DNL JumpSeat]URL]**, which can be found on your extension icon in [!DNL JumpSeat].

>[!BEGINSHADEBOX]

**示例：**

https://{mycompanyname}.jumpseat.io

>>

>[!ENDSHADEBOX]

1. Enter the **[!UICONTROL [!DNL JumpSeat]integration token]**. You can find this on the **[!UICONTROL Configuration]** page in [!DNL JumpSeat].

   **Example:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Click **[!UICONTROL Test configuration]**.
1. 选择您希望该集成是&#x200B;**[!UICONTROL 活动]**&#x200B;还是&#x200B;**[!UICONTROL 非活动]**。

   >[!IMPORTANT]
   >
   >The configuration test performed in step 5 must pass in order to activate the integration.

   ![JumpSeat Integration page](assets/jumpseat-integration-page.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

>[!TIP]
>
>For more information about configuring your [!DNL JumpSeat] integration, see the [!DNL JumpSeat] documentation for [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
