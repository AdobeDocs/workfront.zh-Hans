---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: 配置 JumpSeat 集成
description: 您可以将 [!DNL JumpSeat] 与 [!DNL Workfront] 集成以创建自定义产品内指南。
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 6%

---

# 配置 JumpSeat 集成

您可以将[!DNL JumpSeat]与[!DNL Workfront]集成以创建自定义产品内指南。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table>
  <tr>
   <td>Adobe Workfront包
   </td>
    <p>工作流 Ultimate</p>
   <td> <p>Prime或Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront许可证
   </td>
   <td>标准
   <p>规划</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>产品
   </td>
   <td>您必须拥有有效的[!DNL JumpSeat]计划。
   </td>
  </tr>
   <tr>
   <td>访问级别配置
   </td>
   <td>您必须是[!DNL Workfront]管理员。
   </td>
  </tr>
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

在开始之前，您必须

* 在[!DNL Workfront]中添加并激活[!DNL JumpSeat]作为应用程序。 有关详细信息，请参阅[如何添加或删除应用程序](https://support.jumpseat.io/article/how-to-add-an-application/)。

>[!IMPORTANT]
>
>如果您在Adobe Unified Experience上，则必须使用以下应用程序URL： `.workfront.adobe.com`。



## 配置[!DNL JumpSeat]集成

我们建议在您的预览环境和生产环境中设置[!DNL JumpSeat]集成。

>[!TIP]
>
>您需要在[!DNL Workfront]中添加和激活两个单独的[!DNL JumpSeat]应用程序 — 一个用于预览，一个用于生产。 有关详细信息，请参阅[如何添加或删除应用程序](https://support.jumpseat.io/article/how-to-add-an-application/)。

要配置[!DNL JumpSeat]集成，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 系统]** > **[!UICONTROL [!DNL JumpSeat]集成]**。
1. 输入您的&#x200B;**[!UICONTROL [!DNL JumpSeat]URL]**，您可以在位于[!DNL JumpSeat]的扩展图标上找到该URL。

>[!BEGINSHADEBOX]

**示例：**

https://{mycompanyname}.jumpseat.io

>>

>[!ENDSHADEBOX]

1. 输入&#x200B;**[!UICONTROL [!DNL JumpSeat]集成令牌]**。 您可以在&#x200B;**[!UICONTROL 中的]**&#x200B;配置[!DNL JumpSeat]页面上找到此项。

   **示例：** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 单击&#x200B;**[!UICONTROL 测试配置]**。
1. 选择您希望该集成是&#x200B;**[!UICONTROL 活动]**&#x200B;还是&#x200B;**[!UICONTROL 非活动]**。

   >[!IMPORTANT]
   >
   >在步骤5中执行的配置测试必须通过，才能激活集成。

   ![JumpSeat集成页面](assets/jumpseat-integration-page.png)

1. 单击&#x200B;**[!UICONTROL 保存]**。

>[!TIP]
>
>有关配置[!DNL JumpSeat]集成的更多信息，请参阅有关[!DNL JumpSeat]JumpSeat+Workfront[的](https://jumpseat.io/landing-page/jumpseat-workfront/)文档。
