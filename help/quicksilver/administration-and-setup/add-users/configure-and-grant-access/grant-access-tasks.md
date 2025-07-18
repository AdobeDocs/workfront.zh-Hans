---
title: 授予任务访问权限
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: 作为Adobe Workfront管理员，您可以使用访问级别来定义用户对Workfront中任务的访问权限。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aafa8886-82e2-41c4-8fcb-cbb9df2d55dd
source-git-commit: 09bb41e16da89edd2c2cbfb5a85213045e52394d
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 授予任务访问权限

作为Adobe Workfront管理员，您可以使用访问级别来定义用户对任务的访问权限，如[访问级别概述](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)中所述。

有关使用自定义访问级别管理用户对Workfront中其他对象类型的访问的信息，请参阅[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>规划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 使用自定义访问级别配置用户对任务的访问权限

1. 开始创建或编辑访问级别，如[创建或修改自定义访问级别](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)中所述。
1. 单击任务右侧![](assets/gear-icon-settings.png)查看&#x200B;**或**&#x200B;编辑&#x200B;**按钮上的齿轮图标**，然后在&#x200B;**微调设置**&#x200B;下选择要授予的功能。

   ![微调任务设置](assets/fine-tune-tasks.png)

   >[!NOTE]
   >
   >在为特定类型的对象配置访问级别设置时，该配置不会影响用户对较低排名的对象的访问。 例如，您可以限制用户删除其访问级别中的任务，但这不会限制他们删除级别低于任务的问题。有关对象层次结构的详细信息，请参阅[了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects)一文中的[相互依赖性和对象层次结构](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)部分。

1. （可选）要限制从更高层对象继承的任务权限，请单击&#x200B;**设置其他限制**，然后选择&#x200B;**从项目、任务、问题等中永不继承文档访问权限**。

1. （可选）要为您正在处理的访问级别中的其他对象和区域配置访问设置，请继续[配置对Adobe Workfront的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)中列出的文章之一，如[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)。
1. 完成后，单击&#x200B;**保存**。

   创建访问级别后，可将其分配给用户。 有关详细信息，请参阅[编辑用户配置文件](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 按许可证类型访问任务

有关每个访问级别的用户可以对任务执行哪些操作的信息，请参阅[可用于每个对象类型](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#tasks)的功能一文中的[任务](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)部分。

## 访问共享任务

作为问题的所有者或创建者，您可以通过授予其他用户对该问题的权限来与其共享，如[共享任务](../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md)中所述。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

当您与其他用户共享任何对象时，收件人在该对象上的权限由以下两项共同决定：

* 您授予收件人对象的权限
* 收件人针对对象类型的访问级别设置
