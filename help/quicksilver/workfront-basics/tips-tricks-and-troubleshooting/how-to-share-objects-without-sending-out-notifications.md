---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 如何共享对象而不生成通知
description: 了解如何共享对象并阻止发送有关此更改的通知。 当您批量共享对象时，这尤其有用。
author: Alina
feature: Get Started with Workfront
source-git-commit: b14dd633edec3e9746f7f1412445b74bcd37a676
workflow-type: tm+mt
source-wordcount: '590'
ht-degree: 3%

---


# 如何共享对象而不生成通知

<!--Audited: 12/2024-->

在Adobe Workfront中共享对象时，与您共享该对象的人员会收到有关共享的电子邮件通知。

当有人与您共享对象时收到电子邮件通知对于了解此更改非常重要。 但是，通知过多可能会让用户过于困惑。 如果要一次性与用户共享大量对象，临时禁用通知将有助于避免混淆。

同时启用以下设置时，用户会收到电子邮件通知：

* 系统或组级别启用了以下一个或两个事件通知：

   * “共享对象”到“用户”
   * 系统或组级别上启用了“对象共享到团队”。
* 用户配置文件中启用了以下一个或两个电子邮件通知：

   * 其他人与我共享对象
   * 其他人与我的团队共享对象

如果需要与多个人员（批量）共享多个对象，但不希望他们收到有关此更改的电子邮件通知，请执行以下操作：

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

要共享对象，必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>新许可证： Standard</p> 
   或
   <p>当前许可证：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对要共享对象的访问权限或更高版本</p>
   <p>编辑用户的访问权限</p>
   <p><b>注释</b></p>
   <p> 您必须是系统或组管理员才能检查系统或组的事件通知状态</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看要共享对象的权限或更高</p></td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 共享对象而不生成通知

1. 确保在系统或组级别启用以下&#x200B;**事件通知**：

   * **对象共享到用户**
   * 在系统或组级别&#x200B;**上启用了**&#x200B;与团队的对象共享。

   有关信息，请参阅[为系统中的每个人配置事件通知](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)。

   如果未启用这些事件通知，则不会向用户发送有关共享对象的通知。 如果启用了其中一项或两项功能，请继续执行以下步骤。

{{step-1-to-users}}

1. 选择列表中的多个用户，然后单击&#x200B;**通知** > **其他**。
1. 禁用以下一个或两个通知（取决于从系统或组级别启用的通知）：

   * **其他人与我共享对象**
   * **其他人与我的团队共享对象**

   在禁用通知之前，请确保所有选定的用户都已选择这些通知。 这样，您可以在共享对象后为其所有对象批量重新启用它们。

1. 单击&#x200B;**保存更改**。
1. 转到要共享的对象列表并选择对象，然后单击列表顶部的&#x200B;**共享**&#x200B;图标。

   有关批量共享对象的信息，请参阅[共享对象](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

1. 返回已为其禁用通知的用户列表，然后选择相同的用户。
1. 选择列表中的相同用户，然后单击&#x200B;**通知** > **其他**。
1. 启用以下一个或两个通知（取决于从系统或组级别启用的通知）：

   * **其他人与我共享对象**
   * **其他人与我的团队共享对象**

1. 单击&#x200B;**保存更改**。

   这些对象已共享给选定的用户，但没有一个用户收到有关此更改的任何电子邮件通知。






