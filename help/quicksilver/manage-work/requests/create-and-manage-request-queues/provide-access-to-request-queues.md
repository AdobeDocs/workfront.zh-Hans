---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: 提供对请求队列的访问权限
description: 提供对请求队列的访问权限时，您可以确定组织中的哪些人可以在Adobe Workfront的请求区域查看请求队列。
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# 提供对请求队列的访问权限

提供对请求队列的访问权限时，您可以确定组织中的哪些人可以在Adobe Workfront的请求区域查看请求队列。

您可以根据请求队列中不同用户是项目团队、项目组或项目公司的一员，为这些用户提供对请求队列的访问权限。 您还可以向系统中的每个人提供对请求队列的访问权限。 

在邀请外部利益相关者加入Workfront并希望限制用户对特定区域的访问权限的组织中，这将很有用，在此情况下，仅对与项目公司或组关联的用户打开的请求队列会限制外部利益相关者的可见性。 将访问权限授予任何人都可以让内部和外部利益相关者看到该请求。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请与Workfront管理员联系

## 先决条件

在请求队列可供请求区域中的用户使用之前，您必须创建具有以下设置的项目：

* 将其指定为请求队列。 有关创建请求队列的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。
* 将项目的状态更新为当前。

## 提供对请求队列的访问权限

1. 转到要提供请求队列访问权限的项目。

   >[!NOTE]
   >
   >只有状态为“当前”的项目才会显示在“请求”区域中。

1. 单击左侧面板中的&#x200B;**队列详细信息**。 您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**队列详细信息**。
1. 选择&#x200B;**Publish作为帮助请求队列**&#x200B;以将项目指定为请求队列。
1. 从以下选项中选择：

   * **任何人**：任何用户都可以查看请求并将其添加到请求队列。
   * **拥有查看此项目访问权限的用户**：拥有项目查看权限的用户可以查看请求并将其添加到请求队列。 
   * **此项目公司中的人员**：与项目公司关联的用户可以查看和添加请求。 与该项目关联的公司列在该选项旁边的括号中。 
   * **此项目组的人员**：与项目组关联的用户可以查看和添加请求。 此选项旁边的括号中列出了与项目关联的组。

     当多个部门共享一个Workfront帐户以实现独特的组织目标时，组队列非常有用。 每个部门可能有自己的队列，其他组的成员应该看不到这些队列。

     有关谁拥有项目权限的信息，请参阅[在Adobe Workfront中共享项目](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)。\
     编辑项目时，组和公司可以与项目相关联。 有关编辑项目的详细信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

1. 单击&#x200B;**保存**。
