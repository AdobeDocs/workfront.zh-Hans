---
title: 分享一份文档
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: 您的Adobe Workfront管理员在分配访问权限等级时，授权用户查看或编辑文档，详见“授予文档访问权限”。
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 7f8c9b9f63770d6364f0eb1b9c23e4648dacaf93
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 5%

---

# 分享一份文档

Workfront 管理员控制谁可以在设置中的访问层级区域查看或编辑文档。 更多信息请参见 [“授予文件](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)访问权”。

用户还可以分享他们已上传或访问的文档，赋予他人查看和管理的权限。

* 权限适用于单个项目，并定义个人可以采取的作。
* 上传文档的人会自动获得全部控制权（管理权限）。
* 要分享整个文件夹，请参见 [“共享文档文件夹](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md)”。

>[!NOTE]
>
>如果你的 Workfront 实例使用 Adobe 企业存储，你无法共享单个文档。 相反，你是在项目层面授予访问权限。 请记住，分享项目可能会获得敏感项目信息，比如财务状况，具体取决于所选权限等级。



## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 许可</td> 
   <td> <p>标准</p> 
   <p>工作版或更高版本</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">接入层配置</td> 
   <td> <p>查看你想分享的对象的访问权限或更高权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看你想共享对象的权限或更高权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++



## 共享文档

默认情况下，将文档上传到Workfront的用户具有文档的管理权限。

{{step1-to-documents}}

1. 在&#x200B;**文档**&#x200B;页面上，将鼠标悬停在要共享的文档上，然后单击显示的&#x200B;**文档详细信息**&#x200B;链接。 **文档详细信息**&#x200B;页面打开。

   ![文档详细信息链接](assets/document-details-link.png)

1. 单击文档名称右侧的&#x200B;**更多**&#x200B;图标![更多图标](assets/more-icon.png)，然后单击&#x200B;**共享**。 将打开&#x200B;**共享[文档名称]**&#x200B;对话框。

   ![共享文档](assets/share-a-document-350x160.png)

1. 在&#x200B;**将文档访问权限授予**&#x200B;字段中，开始键入要与其共享该文档的用户、团队、角色、组或公司的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享文档。


1. （可选）选择&#x200B;**具有访问权限**&#x200B;下拉列表并选择文档的访问级别：

   * **只有受邀人员才能访问：**&#x200B;只有受邀访问文档的用户才能访问文档（默认）。
   * **系统中的每个人都可以查看**：系统中的所有用户都可以查看文档，而无需邀请。

1. （可选）若要将文档设为公用，请单击齿轮图标![选择齿轮图标](assets/gear-icon.png)，然后单击与&#x200B;**同行的框以将此文件设为外部用户公用**。 **复制公共链接**&#x200B;按钮显示在对话框底部。

1. 单击用户名右侧的下拉菜单并为该文档选择其权限级别：

   * **查看**：用户可以查看并分享文档。
   * **管理**：用户拥有对文档的完全访问权限，但没有管理权限，这些权限在访问级别被授予（还包括所有查看权限）。

1. （可选）单击您授予的权限级别旁边的高级选项图标，以配置文档的特定权限。

   ![已配置高级权限选项](assets/advanced-options-icon.png)

1. （可选）要关闭文档子对象的继承权限，请单击&#x200B;**关闭**&#x200B;与&#x200B;**继承权限**&#x200B;内联。

1. （视情况而定）要复制允许您与外部用户共享文档的公共链接，请单击&#x200B;**复制公共链接**。

   >[!CAUTION]
   >
   >我们建议您在与外部用户分享包含机密信息的文件时要谨慎。 这让他们无需成为Workfront用户或组织成员，也能查看信息。

1. 单击&#x200B;**保存**。

## 批量分享文档

{{step1-to-documents}}

1. 在&#x200B;**文档页面的**“所有文档&#x200B;**”标签中，按住**&#x200B;键盘上的Command **（Mac）或** Ctrl **（Windows），然后点击你想分享**&#x200B;的每个文档。

1. 在页面顶部，点击&#x200B;**“分享**”图标![](assets/share-icon.png)分享“图标。共享模式打开。

   ![共享图标](assets/share-documents-in-bulk.png)

1. 在&#x200B;**将文档访问权限授予**&#x200B;字段中，开始键入要与其共享文档的用户、团队、角色、组或公司的名称，然后在名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >您只能与活动用户、团队、角色或公司共享文档。


1. （可选）选择&#x200B;**具有访问权限**&#x200B;下拉列表并选择文档的访问级别：

   * **只有受邀人员才能访问：**&#x200B;只有受邀访问文档的用户才能访问文档（默认）。
   * **系统中的每个人都可以查看**：系统中的所有用户都可以查看文档，而无需邀请。

1. 单击用户名右侧的下拉菜单，然后选择他们对文档的权限级别：

   * **查看**：用户可以查看和共享文档。
   * **管理**：用户拥有对无管理权限的文档的完全访问权限，这些权限是在访问级别授予的（还包括所有查看权限）。

1. （可选）单击您已授予的权限级别旁边的高级选项图标，以配置文档的特定权限。

   ![已配置高级权限选项](assets/advanced-options-icon.png)

1. 单击&#x200B;**保存**。

## 与Adobe企业存储的文档共享

Workfront 正在向 Adobe 企业存储解决方案转型，以提供与 Adobe Creative Cloud 产品的更高连接性。 现有客户将分阶段迁移至新模式。 欲了解更多关于Adobe企业存储优势的信息，请访问 [Adobe企业存储概览](/help/quicksilver/review-and-approve-work/esm-overview.md)。

如果你的 Workfront 实例使用 Adobe 企业存储，你不能直接分享单个文档。 相反，你必须在项目层面授予访问权限。

>[!IMPORTANT]
>
>分享项目还可能让用户访问敏感项目信息，如财务状况，具体取决于你选择的权限等级。
>
>分享前请务必仔细查看权限设置。

## 文档权限

权限是针对 Workfront 中某项特定作的，并定义了对该项可以采取的作。 有关对象权限的信息，请参见 [对象](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)共享权限概览。

下表显示了允许用户查看或管理文档时可以授予的权限：

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>行动</strong> </p> </th> 
   <th> <p><strong>管理</strong> </p> </th> 
   <th> <p><strong>查看</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">创建</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑文档详情</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">删除*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">下载</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">结帐</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">添加审批者</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">批准文档</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">附上自定义表单</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">编辑自定义字段</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移动到（对象）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">发送到（集成）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">更新/评论</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">上传新版本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">删除版本</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">查看文档</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">预览</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">校对**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">生成证据**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">移除校对**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">共享*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">全系统共享*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">公开分享文件*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">用外部邮箱分享</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">添加/删除</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">重命名</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">链接（带集成）</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Unlink（带集成）</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; 作由文档和文档文件夹共享。

&#42;&#42; 你必须为Workfront账户绑定单独的校样许可证，才能校对文件。 联系你的客户经理，申请校样许可。 关于Workfront校样的更多信息，请参见[校样。](../../review-and-approve-work/proofing/proofing.md)

## 关于共享文档的考虑

除了以下考虑外，还可参见 [对象](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)共享权限概述。

>[!NOTE]
>
>Workfront管理员可以为系统中的任何项目为所有用户添加或删除权限，而无需成为这些项目的所有者。

* 共享文档与在Workfront中共享任何其他对象类似。 有关如何在Workfront中共享文档的信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。
* 您可以向文档授予以下权限：

   * 视图
   * 管理

* 您还可以公开或系统范围共享文档。

  >[!CAUTION]
  >
  >建议在与外部用户共享包含机密信息的对象时务必谨慎。 这让他们无需成为Workfront用户或组织成员，也能查看信息。

* 你可以在“授予文档访问权限”字段中添加他们的电子邮件地址，与没有 Workfront 账户的人分享文档。
* 当你分享文档时，用户拥有所有文档版本和所有文档校样的访问权限。\
  关于Workfront打样的更多信息，请参见 [打样](../../review-and-approve-work/proofing/proofing.md) 部分。

* 你可以从与文档关联的对象中继承其权限。 你的Workfront管理员可以限制访问级别文档的权限继承。

  关于限制文档继承权限的更多信息，请参见 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)。

  你可以手动移除文档继承权限。 更多信息请参见 [“移除对象权限”](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)

* 附加文档仅继承其附着对象的权限。 如果你在对象上创建文件夹并把文档移到文件夹里，它会继承该文件夹的权限。 但是，如果你在父对象或祖父对象上创建文件夹并将文档移入该文件夹，它不会继承该文件夹的权限。