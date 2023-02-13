---
title: 共享任务
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront管理员在分配访问级别时，可以授予您查看或编辑任务的权限。 有关授予对任务的访问权限的更多信息，请参阅授予对任务的访问权限。
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 4%

---

# 共享任务

Adobe Workfront管理员在分配访问级别时，可以授予您查看或编辑任务的权限。 有关授予任务访问权限的更多信息，请参阅 [授予对任务的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

除了授予用户的访问级别之外，您还可以授予他们查看、参与或管理您有权共享的特定任务的权限。

权限特定于Workfront中的一个项目，并定义可以对该项目执行哪些操作。

## 共享任务时的注意事项

除了以下注意事项外，另请参阅 [对象共享权限概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* 默认情况下，任务的创建者具有该任务的“管理”权限。
* 您可以单独共享任务，也可以一次批量共享其中多个任务。\
   共享任务与共享其他对象相同。 有关在Workfront中共享项目的更多信息，请参阅 [共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 您可以为任务授予以下权限： 

   * 查看
   * 管理
   * 参与\
      ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* 默认情况下，在您共享任务时，用户将继承与任务关联的所有子对象的相同权限。 例如，他们继承了与任务相关的子任务、问题和文档的相同权限。\
   有关Workfront中对象层次结构的更多信息，请参阅  [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   Workfront管理员可以指定文档是否应继承用户访问级别中较高对象的权限。 有关限制文档继承权限的更多信息，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* 您可以从任务中删除继承的权限。\
   有关从对象中删除继承权限的更多信息，请参阅  [从对象删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## 任务共享方法

您可以通过以下方式共享任务：

* 单独或批量手动操作。 手动共享任务与在Workfront中共享任何其他对象类似。

   有关在Workfront中共享对象的更多信息，请参阅  [共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* 自动执行以下操作：

   * 指定任务任何父对象的权限：项目、项目群或项目组合。 任务会从其父对象继承权限。 有关查看对象继承权限的信息，请参阅 [查看对象的继承权限](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * 在用于创建任务所在项目的模板上将实体添加到项目共享。 有关从模板共享项目的信息，请参阅 [共享模板](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * 在编辑项目时，指定对项目中所有任务的权限。 有关根据用户对项目的权限管理对项目任务的访问权限的信息，请参阅 [](../../manage-work/projects/manage-projects/edit-projects.md#access) 章节 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md).
   >[!TIP]
   >
   >如果未指定在将用户分配到项目中的任务时您希望用户具有的任务权限，则默认情况下，他们将获得与他们在项目中拥有的权限相同的权限。

## 任务权限

下表显示了在允许用户查看、参与或管理任务时，可以向其授予哪些权限：

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>操作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>参与</strong> </th> 
   <th><strong>查看</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">添加任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加前置任务</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加问题</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">删除任务</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>常规任务编辑<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更改任务状态</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑任务约束</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">添加文档</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">复制任务*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">移动任务*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">记录小时数</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">修改计划日期</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">接受分配</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">进行分配</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">附上自定义表单</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑自定义字段</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">创建审批流程</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">批准任务</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">编辑财务状况*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加/编辑费用</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看财务状况</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">更新/评论</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">共享</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">在系统范围内共享</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;由项目的访问级别和权限控制。
