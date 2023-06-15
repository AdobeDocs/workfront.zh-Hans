---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 通过Adobe Admin Console将用户添加到Adobe Workfront Fusion
description: 您可以将用户添加到Adobe Admin Console并将其分配给Adobe Workfront Fusion，也可以将Adobe Admin Console中的现有用户分配给Workfront Fusion。
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 392eee3c7b1aacf92d7877f07a8154924f3926a0
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# 将用户添加到 [!DNL Adobe Workfront Fusion] 通过 [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于已载入的组织。 [!DNL Adobe Admin Console].
>
>如果您的组织尚未载入 [!DNL Adobe Admin Console]，请参见 [在中将用户添加到组织 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>对于因贵组织是否已载入到以下版本而不同的过程，请参见 [!DNL Adobe Admin Console]，请参见 [基于平台的管理差异([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

您可以将用户添加到 [!DNL Adobe Admin Console] 并将它们分配给 [!DNL Adobe Workfront Fusion]，或在中分配现有用户 [!DNL Adobe Admin Console] 到 [!DNL Workfront Fusion].

观看视频，了解 [!DNL Workfront Fusion] 在 [!DNL Adobe Admin Console]，包括如何添加用户，请参阅 [[!DNL Fusion] 在Adobe IMS上](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[！UICONTROL Workfront Fusion for Work Automation and Integration] </p> <p>[！UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] 管理员权限</td> 
   <td>您必须是以下项的[！UICONTROL产品配置管理员] [!DNL Adobe] 产品。</td> 
  </tr>
  </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

&#42;&#42;有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## 先决条件

使用之前 [!DNL Admin Console] 对象 [!DNL Workfront]，您应会收到一封邀请您使用控制台的电子邮件。

1. 如果您是初次使用 [!DNL Adobe] 并且您已经收到一封电子邮件，告知您现在拥有管理权限 [!DNL Adobe] 软件和服务，请单击电子邮件中的按钮以创建 [!DNL Adobe] 帐户并打开 [!DNL Admin Console].

   或

   如果您已有Adobe帐户，请转到 [[!DNL Adobe Admin Console] 页面](https://adminconsole.adobe.com/).


## 将新用户添加到 [!DNL Adobe Admin Console] 和 [!DNL Workfront Fusion]

1. 从 [[!DNL Adobe Admin Console] 页面](https://adminconsole.adobe.com/)，选择 **[!UICONTROL 产品]** 选项卡，然后选择 **[!DNL Workfront Fusion]** 产品拼贴。

   ![Admin Console中的融合](assets/fusion-product-admin-console.png)

1. 在显示的列表中，选择要添加用户的组织。

   ![Admin Console中的融合实例](assets/fusion-instances-admin-console.png)

1. 在显示的列表中，使用 **[!UICONTROL 产品配置文件]** 选项卡中，单击 [!DNL Workfront Fusion] [!UICONTROL 产品配置文件] 链接。

   ![Workfront Fusion产品配置文件](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > 请勿对 [!UICONTROL 产品配置文件] 本身。

1. 使用 **[!UICONTROL 用户]** 选项卡上，单击 **[!UICONTROL 添加用户]**.

1. 在 **[!UICONTROL 将用户添加到此产品配置文件]** 框中，输入要添加的用户的电子邮件地址或名称，然后在显示的列表中选择该用户。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   用户创建于 [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. （可选）继续访问 [在中更改用户的访问级别 [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## 在Workfront Fusion中更改用户的访问级别

### 将用户的角色更改为管理员

必须在以下位置为用户授予管理员角色： [!DNL Adobe Admin Console].

1. 在 [!DNL Workfront Fusion] [!UICONTROL 产品配置文件] 添加用户的页面，选择 **[!UICONTROL 管理员]** 选项卡。

1. 单击 **[!UICONTROL 添加管理员]**.

1. 在 **[!UICONTROL 添加产品配置文件管理员]** 框中，输入要添加的用户的电子邮件地址或名称，然后在显示的列表中选择该用户。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   此用户现在是中的管理员 [!DNL Workfront Fusion].

### 将用户的角色更改为 [!UICONTROL 会员]， [!UICONTROL 会计师]，或 [!UICONTROL 应用程序开发人员].

[!UICONTROL 会员]， [!UICONTROL 会计师]、和 [!UICONTROL 应用程序开发人员] 在内部处理角色 [!DNL Workfront Fusion].

有关说明，请参阅 [查看或编辑用户角色](../organizations/manage-fusion-users.md#view-or-edit-user-roles) 在文章中 [管理 [!DNL Adobe Workfront Fusion] 您组织中的用户](../organizations/manage-fusion-users.md)

## 在中分配现有用户 [!DNL Adobe Admin Console] 到 [!DNL Workfront Fusion]

1. 按照文章的“编辑用户详细信息”部分中所述，开始编辑用户 [单独管理用户](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) 在 [!DNL Adobe Admin Console] 文档。

1. 添加 **[!DNL Adobe Workfront Fusion]** 分配给用户的产品。
