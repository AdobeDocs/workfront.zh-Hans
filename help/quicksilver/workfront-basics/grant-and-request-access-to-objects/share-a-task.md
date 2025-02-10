---
title: 共享任务
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: 当您的Adobe Workfront管理员分配访问级别时，可以授予您查看或编辑任务的权限。 有关授予任务访问权限的详细信息，请参阅授予任务访问权限。
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: 3bd377ba2dec29bb956632cf3e9e3e33afe4305d
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 2%

---

# 共享任务

当您的Adobe Workfront管理员分配访问级别时，可以授予您查看或编辑任务的权限。 有关授予任务访问权限的详细信息，请参阅[授予任务访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)。

除了授予用户的访问级别之外，您还可以授予他们查看、Contribute或管理您有权共享的特定任务的权限。

权限特定于Workfront中的一个项目，并定义您可以对该项目执行的操作。

## 共享任务时的注意事项

除了下面的注意事项外，另请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

* 默认情况下，任务的创建者具有管理权限。
* 您可以单独共享任务，也可以一次批量共享多个任务。\
  共享任务与共享其他对象相同。 有关在Workfront中共享项目的详细信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

* 您可以向任务授予以下权限： 

   * 查看
   * 管理
   * 参与\
     ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* 共享任务时，默认情况下，用户将继承与该任务关联的所有子对象的相同权限。 例如，他们对附加到任务的子任务、问题和文档继承相同的权限。\
  有关Workfront中对象层次结构的详细信息，请参阅  [了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

  Workfront管理员可以指定文档是否应从用户访问级别更高的对象继承权限。 有关限制文档继承权限的详细信息，请参阅[创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

* 您可以从任务中删除继承的权限。\
  有关从对象中删除继承权限的详细信息，请参阅  [从对象中删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 共享任务的方法

您可以通过以下方式共享任务：

* 手动逐个或批量执行。 手动共享任务与在Workfront中共享任何其他对象类似。

  有关在Workfront中共享对象的更多信息，请参阅  [共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

* 通过执行以下操作，自动执行：

   * 指定任务的任何父对象的权限：项目、项目群或项目组合。 任务从其父对象继承权限。 有关查看对象的继承权限的信息，请参阅[查看对象的继承权限](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md)。
   * 在用于创建任务所在项目的模板上，将实体添加到项目共享。 有关从模板共享项目的信息，请参阅[共享模板](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

   * 在编辑项目时，指定项目中所有任务的权限。 有关基于用户对项目的权限管理项目上任务的访问权限的信息，请参阅[编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)一文中的[](../../manage-work/projects/manage-projects/edit-projects.md#access)部分。

  >[!TIP]
  >
  >如果您未指定在将用户分配给项目中的任务时希望用户具有哪些任务权限，则默认情况下，这些用户将获得他们在项目中的相同权限。

## 任务权限

下表显示了在允许用户查看、Contribute或管理任务时您可以授予用户哪些权限：

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>操作</strong> </th> 
   <th><strong>管理</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>视图</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">添加任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加前置任务</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加问题</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">删除任务</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>常规任务编辑<br></p> </td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更改任务状态</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑任务限制</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">添加文档</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">复制任务*</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">移动任务*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">记录小时数</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">修改计划日期</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">接受分配</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">进行分配</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">附上自定义表单</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑自定义字段</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">创建批准流程</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">批准任务</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">编辑财务*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加/编辑费用</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看财务状况</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">更新/评论</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">共享</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">在系统范围内共享</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
 </tbody> 
</table>

&#42;由访问级别和项目权限控制。
