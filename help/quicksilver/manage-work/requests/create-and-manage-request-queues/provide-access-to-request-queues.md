---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 提供对请求队列的访问权限
description: 提供对请求队列的访问权限时，您可以确定组织中谁可以在Adobe Workfront的“请求”区域中查看请求队列。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 提供对请求队列的访问权限

提供对请求队列的访问权限时，您可以确定组织中谁可以在Adobe Workfront的“请求”区域中查看请求队列。

您可以根据用户是项目团队、项目组还是项目公司的一部分，为不同的用户提供对请求队列的访问权限。 您还可以为系统中的每个人提供对请求队列的访问权限。 

对于邀请外部利益相关方加入Workfront并希望限制用户访问特定区域的组织而言，这非常有用 — 在这种情况下，请求队列仅对与公司或项目组关联的用户打开，从而限制了对外部利益相关方的可见性。 向任何人授予访问权限，会使内部和外部利益相关方都能看到该请求。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员

## 先决条件

在“请求”区域中的用户可以使用请求队列之前，您必须使用以下设置创建一个项目：

* 将其指定为请求队列。 有关创建请求队列的更多信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* 将项目的状态更新为“当前”。

## 提供对请求队列的访问

1. 转到要提供对请求队列的访问权限的项目。

   >[!NOTE]
   >
   >“请求”区域中只显示状态为“当前”的项目。

1. 单击 **队列详细信息** 中。 您可能需要单击 **显示更多**，则 **队列详细信息**.
1. 选择 **作为帮助请求队列发布** 将项目指定为请求队列。
1. 从以下选项中进行选择：

   * **任何人**:任何用户都可以查看请求队列并将请求添加到请求队列。
   * **有权查看此项目的人员**：对项目具有“查看”权限的用户可以查看请求并将请求添加到请求队列。 
   * **此项目公司的人员**：与项目的公司关联的用户可以查看和添加请求。 与项目关联的公司列在此选项旁边的括号中。 
   * **此项目组中的人员**：与项目的组关联的用户可以查看和添加请求。 与项目关联的组列在此选项旁边的括号中。

      当多个部门共享Workfront帐户以实现独特的组织目标时，组队列非常有用。 每个部门可能都有自己的队列，其他群组的成员不能看到这些队列。

      有关谁对项目拥有权限的信息，请参阅 [在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
      在编辑项目时，可以将组和公司与项目关联。 有关编辑项目的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 单击&#x200B;**保存**。
