---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 通过Adobe Admin Console将用户添加到Adobe Workfront Fusion
description: Adobe Workfront Fusion文档已移至新位置。 本文已弃用，但包含指向介绍此功能的新文章的链接。
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 1%

---

# 通过[!DNL Adobe Admin Console]将用户添加到[!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion文档已移至新位置。
>
>本文中的信息现在可在以下文章中找到：
>
>* [通过Adobe Admin Console将用户添加到Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/add-fusion-users-admin-console.html)
>
>请更新任何书签。
>
>本文不再更新，不久将会删除。

>[!IMPORTANT]
>
>此页面上描述的过程仅适用于已载入到[!DNL Adobe Admin Console]的组织。
>
>如果贵组织尚未登记到[!DNL Adobe Admin Console]，请参阅[在 [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md)中将用户添加到组织。
>
>有关因贵组织是否已登记到[!DNL Adobe Admin Console]而不同的过程列表，请参阅[基于平台的管理差异([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md)。

您可以将用户添加到[!DNL Adobe Admin Console]并将其分配给[!DNL Adobe Workfront Fusion]，或将[!DNL Adobe Admin Console]中的现有用户分配给[!DNL Workfront Fusion]。

有关描述[!DNL Adobe Admin Console]中的[!DNL Workfront Fusion]的视频（包括如何添加用户），请参阅Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}上的[[!DNL Fusion] 。

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
   <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] 管理员权限</td> 
   <td>您必须是组织的[!DNL Adobe]产品的[！UICONTROL产品配置管理员]。</td> 
  </tr>
  </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

&#42;&#42;有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## 先决条件

在使用[!DNL Workfront]的[!DNL Admin Console]之前，您应该会收到一封邀请您加入控制台的电子邮件。

1. 如果您是[!DNL Adobe]的新用户，并且已收到一封电子邮件，告知您现在拥有管理贵组织的[!DNL Adobe]软件和服务的管理权限，请单击电子邮件中的按钮以创建[!DNL Adobe]帐户并打开[!DNL Admin Console]。

   或

   如果您已有Adobe帐户，请转到[[!DNL Adobe Admin Console] 页面](https://adminconsole.adobe.com/)。


## 向[!DNL Adobe Admin Console]和[!DNL Workfront Fusion]添加新用户

1. 从[[!DNL Adobe Admin Console] 页面](https://adminconsole.adobe.com/)中，选择顶部导航栏中的&#x200B;**[!UICONTROL 产品]**&#x200B;选项卡，然后选择&#x200B;**[!DNL Workfront Fusion]**&#x200B;产品拼贴。

   Admin Console](assets/fusion-product-admin-console.png)中的![Fusion

1. 在显示的列表中，选择要添加用户的组织。

   Admin Console](assets/fusion-instances-admin-console.png)中的![Fusion实例

1. 在显示的列表中，选择&#x200B;**[!UICONTROL 产品配置文件]**&#x200B;选项卡，单击[!DNL Workfront Fusion] [!UICONTROL 产品配置文件]链接的名称。

   ![Workfront Fusion产品配置文件](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > 不要对[!UICONTROL 产品配置文件]本身进行任何更改。

1. 在列表上方选择&#x200B;**[!UICONTROL 用户]**&#x200B;选项卡，单击&#x200B;**[!UICONTROL 添加用户]**。

1. 在&#x200B;**[!UICONTROL 将用户添加到此产品配置文件]**&#x200B;框中，输入要添加的用户的电子邮件地址或名称，然后在显示的列表中选择该用户。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   已在[!DNL Workfront Fusion]中创建用户。

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. （可选）继续[在 [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)中更改用户的访问级别

## 在Workfront Fusion中更改用户的访问级别

### 将用户的角色更改为管理员

必须在[!DNL Adobe Admin Console]中为用户分配管理员角色。

1. 在您添加用户的[!DNL Workfront Fusion] [!UICONTROL 产品配置文件]页面上，选择&#x200B;**[!UICONTROL 管理员]**&#x200B;选项卡。

1. 单击&#x200B;**[!UICONTROL 添加管理员]**。

1. 在&#x200B;**[!UICONTROL 添加产品配置文件管理员]**&#x200B;框中，输入要添加的用户的电子邮件地址或名称，然后在显示的列表中选择该用户。

1. 单击&#x200B;**[!UICONTROL 保存]**。

   此用户现在是[!DNL Workfront Fusion]中的管理员。

### 将用户的角色更改为[!UICONTROL 成员]、[!UICONTROL 会计师]或[!UICONTROL 应用开发人员]。

[!UICONTROL 成员]、[!UICONTROL 会计师]和[!UICONTROL 应用程序开发人员]角色在[!DNL Workfront Fusion]内处理。

有关说明，请参阅文章[管理 [!DNL Adobe Workfront Fusion] 组织中的用户](../organizations/manage-fusion-users.md)中的[查看或编辑用户角色](../organizations/manage-fusion-users.md#view-or-edit-user-roles)

## 将[!DNL Adobe Admin Console]中的现有用户分配给[!DNL Workfront Fusion]

您可以在Fusion中将现有用户添加到团队。 这在Fusion中处理。

有关说明，请参阅“将用户添加到Adobe Workfront Fusion中的组织或团队”一文中的[将用户添加到团队](/help/quicksilver/workfront-fusion/organizations/add-user-to-an-organization.md#add-a-user-to-a-team)。
