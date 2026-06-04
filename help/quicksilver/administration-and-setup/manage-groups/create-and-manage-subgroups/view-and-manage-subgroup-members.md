---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 查看和管理子组成员
description: 查看您管理的组时，可以查看和管理该组子组中的所有用户。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
TQID: https://experienceleague.adobe.com/BbyES980TEgJEigbZQuvzncLvGc1FlM09muH-t4zq44
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 384
ht-degree: 4%

---

# 查看和管理子组成员

查看您管理的组时，可以查看和管理该组子组中的所有用户。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td><p>“任一”</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <img src="assets/gear-icon-settings.png">下至少启用<b>用户管理员</b>选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看和管理组下的子组成员

{{step-1-to-setup}}

1. 单击&#x200B;**组**。

   在显示的列表中，您可以看到您管理的组以及它们具有的任何子组。 Adobe Workfront管理员可以查看所有组。

1. 单击要查看或管理其子组成员的组的名称。
1. 在左侧面板中，单击&#x200B;**子组成员**。

   此左侧面板项目仅在组具有子组时才可用。

1. 执行以下任一操作：

   * 在列表中选择一个成员，然后单击“编辑”![“编辑”图标](assets/edit-icon.png)以修改该人员的用户配置文件。

     有关详细信息，请参阅[编辑用户的配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)或[批量编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)。

   * 选择列表中的任意数量的子组成员，然后单击&#x200B;**将更新发送给用户**&#x200B;以向其用户配置文件添加评论。

     一个或多个用户会收到应用程序内通知以及包含您评论的电子邮件通知。 该注释显示在用户配置文件的更新区域。

     有关详细信息，请参阅[向其他用户发送私信](/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md)。

   * 选择列表中任意数量的成员，然后单击“停用![停用用户](assets/deactivate-user.png)”或“激活![激活用户](assets/activate-user.png)”。

     有关详细信息，请参阅[停用或重新激活用户](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)。

   * 导出![导出](assets/export.png)成员列表。
