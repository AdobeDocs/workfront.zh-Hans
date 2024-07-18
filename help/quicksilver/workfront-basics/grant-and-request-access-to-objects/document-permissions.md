---
title: 共享文档
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: 当分配访问级别时，您的Adobe Workfront管理员会授予用户查看或编辑文档的访问权限，如授予对文档的访问权限中所述。
author: Alina
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---

# 共享文档

当分配访问级别时，您的Adobe Workfront管理员授予用户查看或编辑文档的访问权限，如[授予对文档的访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)中所述。

Workfront管理员授予用户的访问级别允许用户查看或编辑文档。 除此之外，其他用户还可以向其他人授予查看或管理他们自己上传或有权共享的特定文档的权限。

权限特定于Workfront中的一个项目，并定义您可以对该项目执行的操作。 有关对象权限的信息，请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

默认情况下，将文档上传到Workfront的用户具有文档的管理权限。

有关共享整个文档文件夹的信息，请参阅[共享文档文件夹](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)。

## 有关共享文档的注意事项

除了下面的注意事项外，另请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理员可以为系统中的任何项目为所有用户添加或删除权限，而无需成为这些项目的所有者。

* 共享文档与在Workfront中共享任何其他对象类似。 有关如何在Workfront中共享文档的信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 您可以向文档授予以下权限：

   * 查看
   * 管理

* 您还可以公开或系统范围共享文档。

  >[!CAUTION]
  >
  >建议在与外部用户共享包含机密信息的对象时务必谨慎。 这样，他们便可以查看信息，而无需成为Workfront用户或您组织的一部分。

* 通过在授予文档访问权限字段中添加其电子邮件地址，您可以与没有Workfront帐户的人共享文档。
* 当您共享文档时，用户对所有文档版本和所有文档验证具有相同的访问权限。\
  有关Workfront中校对的更多信息，请参阅[校对](../../review-and-approve-work/proofing/proofing.md)部分。

* 您可以从文档关联的对象继承对文档的权限。 Workfront管理员可以限制访问级别中文档的权限继承。

  有关限制文档继承权限的详细信息，请参阅[创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  您可以手动删除对文档的继承权限。 有关详细信息，请参阅[从对象中删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* 附加的文档仅从其附加的对象继承权限。 如果在对象上创建文件夹并将文档移动到该文件夹中，它会继承该文件夹的权限。 但是，如果您在父对象或祖父对象上创建文件夹，并将文档移动到该文件夹中，则它不会继承该文件夹的权限。

## 文档权限

下表显示了允许用户查看或管理文档时，您可以授予用户哪些权限：

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>操作</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>视图</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">创建</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑文档详细信息</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">删除*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">下载</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">结帐</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加审批者</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">批准文档</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">附上自定义表单</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑自定义字段</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移动到（对象）</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">发送至（集成）</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更新/评论</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">上传新版本</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">删除版本</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看文档</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">预览</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">校对**</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">生成校对**</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移除校对**</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">共享*</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">共享系统范围*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">公开共享文档*</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">与外部电子邮件地址共享</td> 
   <td> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">添加/删除</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">重命名</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">链接（与集成）</td> 
   <td>✓ {\f13 }</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td scope="row">取消链接（与集成）</td> 
   <td>✓ {\f13 }</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;操作由文档和文档文件夹共享。

&#42;&#42;您必须拥有与您的Workfront帐户关联的单独验证许可证才能验证文档。 有关获取验证许可证的信息，请与您的客户经理联系。 有关Workfront中校对的更多信息，请参阅[校对](../../review-and-approve-work/proofing/proofing.md)。
