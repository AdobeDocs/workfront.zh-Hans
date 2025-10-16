---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 防止出现重复用户
description: 在Adobe Workfront中创建新用户时，即使电子邮件地址因大小写而异(例如，JohnDoe@example.com和johndoe@example.com)，也不能再使用其他用户已在使用的电子邮件地址。 此外，为了准备未来的身份验证增强功能，请确保所有用户在Workfront实例中具有唯一的电子邮件地址。
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6b2d93d2573d72e4390761038d8078f47d96d55e
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 防止重复用户

在Adobe Workfront中创建新用户时，即使电子邮件地址因大小写而异(例如，JohnDoe@example.com和johndoe@example.com)，也不能再使用其他用户已在使用的电子邮件地址。 此外，为了准备未来的身份验证增强功能，请确保所有用户在Workfront实例中具有唯一的电子邮件地址。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建具有唯一电子邮件地址的用户

从2019.4版本开始，在Workfront中创建新用户时，即使电子邮件地址因大小写而异，也不能再使用其他用户已在使用的电子邮件地址。 例如，如果另一个用户的电子邮件地址为JohnDoe@example.com ，则不能创建另一个电子邮件地址为johndoe@example.com的用户。

## 更新Workfront实例中现有用户的电子邮件地址

作为Workfront管理员，您必须更新其匹配电子邮件地址因大小写不同而不同的现有用户。
要修复Workfront实例中的重复电子邮件地址，请执行以下操作：

1. 检查任何重复用户，并确定不再需要哪个用户。

   {{step-1-to-users}}

   1. 在&#x200B;**筛选器**&#x200B;菜单中，选择&#x200B;**全部**。

   1. 在&#x200B;**视图**&#x200B;菜单中，选择&#x200B;**用户登录**。

   1. 在&#x200B;**分组**&#x200B;菜单中，选择&#x200B;**无**。

   1. 自定义用户登录视图。

      1. 单击&#x200B;**视图** > **自定义视图**。

      1. 将&#x200B;**ID**&#x200B;列替换为&#x200B;**电子邮件地址**&#x200B;列。

      1. 重命名视图并保存它。

   1. 创建新分组。

      1. 单击&#x200B;**分组** > **新建分组**。

      1. 单击页面右上角的&#x200B;**切换到文本模式**。
      1. 粘贴以下文本模式代码：

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. 重命名分组并保存它。

1. 执行以下任一操作：

   * （首选方法）为每一个其他帐户向用户的电子邮件地址添加一个+地址。

     如果贵组织中的单个用户需要访问1个以上的用户帐户，请选择此选项。 如果您的电子邮件提供商不支持加号寻址，则必须为每个Workfront帐户提供单独的电子邮件帐户。

     例如，John Doe可以有一个用户帐户用于其日常使用帐户，以及一个用户帐户用于测试目的：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * 将以下文本附加到电子邮件地址，以将域更改为使用伪域：

     `.inactive`

     例如，John Doe可能具有以下域：（这些域必须唯一。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     您无法再登录到这些帐户，因为密码重置需要有效的电子邮件地址。 只能使用“登录身份”功能访问这些帐户。

   * 删除不需要的用户

     >[!IMPORTANT]
     >
     >仅针对错误创建的帐户或测试帐户选择此选项。 此选项通常仅对登录错误为零或1的帐户执行。 绝不应该删除已定期使用的帐户。

如果您的Workfront实例中的用户具有匹配的电子邮件地址，这些地址仅因大小写而异，则Workfront将在需要更新这些地址时为您提供其他信息和时间表。
