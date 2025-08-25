---
title: 配置 [!DNL Workfront] 和 [!DNL Frame.io] 集成
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 作为 [!DNL Adobe Workfront] 管理员，您可以将 [!DNL Workfront] 与 [!DNL Frame.io] 集成，并为您的组织提供无缝查看和批准资产的方式。
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
hide: true
hidefromtoc: true
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# 配置[!DNL Workfront]和[!DNL Frame.io]集成

Workfront管理员通过在“设置”区域中配置默认Frame.io帐户，然后在Workfront中指定Frame.io用户，来启用Workfront与Frame.io之间的集成。 这使项目协调员能够使用Workfront项目以及审阅和批准工作流来计划和启动工作。


## 访问要求

>[!IMPORTANT]
>
>此功能仅适用于已载入[!DNL Adobe Admin Console]的组织。

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table>
  <tr>
   <td>[!DNL Adobe Workfront] 计划</td>
   <td>任何</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] 许可证
   </td>
   <td><p>当前： [!UICONTROL 计划]</p>
   <p>新文档： [!UICONTROL Standard]</p></td>
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

## 配置默认[!DNL Frame.io]帐户[!BADGE 即将推出]{type=Informative}

设置默认[!DNL Frame.io]帐户后，在[!DNL Workfront]中创建的所有项目都将在Frame.io中创建镜像项目。

>[!IMPORTANT]
>
>此功能即将推出。 目前，Frame.io帐户由Workfront团队手动添加。 请联系您的Adobe客户代表寻求帮助。

## 使用Workfront组配置单个Frame.io帐户

您可以使用不同于默认帐户的单个Frame.io帐户连接单个Workfront组。

要在Workfront组中配置单个Frame.io帐户，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组**。
1. 选择现有组，或单击&#x200B;**创建组**。
1. 在左侧面板中，单击&#x200B;**连接到Frame.io**。
1. 输入API开发人员令牌。
1. 单击&#x200B;**启动连接**。
1. （视情况而定）如果您是多个Frame.io帐户的管理员，请选择要使用的帐户。

## 启用Frame.io用户

经常使用Frame.io的Workfront用户应标记为Frame.io用户。 Workfront管理员可以在Workfront用户配置文件中指定Frame.io用户。

>[!TIP]
>
>我们建议使经常使用创意工具并上传资源的用户能够作为Frame.io用户进行审阅和批准。

在Workfront中将用户标记为Frame.io用户并将其添加到项目中时：

* 它们将作为协作者添加到Frame.io中。<!--do we need to be more explicit about a frame license being provisioned for them?-->
* 他们可以将Frame.io中的资源发送到Workfront以进行正式审查和批准。
* 他们可以从Workfront的单向同步文件夹中查看信息。 [!BADGE 即将推出]{type=Informative}

要启用Frame.io用户：

{{step-1-to-users}}

1. 选择一个或多个用户，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。
1. 在“访问”部分中，启用“添加到Frame.io中的项目”复选框，然后在下拉菜单中选择&#x200B;**是**。
   ![添加到框架项目](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >如果未选中此框，则用户将保留对过去工作分配的访问权限，并且会添加到以后的Frame.io项目中。<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
