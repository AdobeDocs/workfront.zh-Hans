---
title: 授予对费率卡的访问权限
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以定义用户对其访问级别在Workfront中访问财务数据的权限。
author: Becky and Lisa
feature: System Setup and Administration
role: Admin
exl-id: b21e65d3-3c9f-4f3d-95d3-de4c09199622
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 5%

---

# 授予对费率卡的访问权限

作为Adobe Workfront管理员，您可以按照[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述，定义用户通过访问级别对信息卡进行评级的访问权限。

有关费率卡的信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>标准</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 授予对费率卡的访问权限的注意事项

授予用户访问Workfront中评级卡的权限时，请考虑以下事项：

* 用户必须具有对费率卡、项目和财务数据的编辑权限，才能将费率卡附加到项目。
* 无权访问费率卡和编辑财务数据的用户无法将费率卡附加到项目，但他们可以编辑项目中来自其他来源的其他记帐费率。

## 使用自定义访问级别配置用户访问以评级卡片

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击费率卡右侧![](assets/gear-icon-settings.png)查看&#x200B;**或**&#x200B;编辑&#x200B;**按钮上的齿轮图标**，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

   ![微调速率卡访问](assets/rate-card-access-fine-tune.png)

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，例如[授予对任务的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 访问共享费率卡

通过授予其他用户权限可以与其共享费率卡，如[共享费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/share-rate-cards.md)中所述。

当您与其他用户共享任何对象时，收件人在该对象上的权限由以下两项共同决定：

* 您授予收件人对象的权限
* 收件人针对对象类型的访问级别设置
