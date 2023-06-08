---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 防止重复用户
description: 在Adobe Workfront中创建新用户时，即使电子邮件地址因大小写而异(例如JohnDoe@example.com和johndoe@example.com)，也不能再使用已由其他用户使用的电子邮件地址。 此外，为了准备应对未来的身份验证增强功能，请确保所有用户在Workfront实例中具有唯一的电子邮件地址。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# 防止重复用户

在Adobe Workfront中创建新用户时，即使电子邮件地址因大小写而异(例如JohnDoe@example.com和johndoe@example.com)，也不能再使用已由其他用户使用的电子邮件地址。 此外，为了准备应对未来的身份验证增强功能，请确保所有用户在Workfront实例中具有唯一的电子邮件地址。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建具有唯一电子邮件地址的用户

从2019.4版本开始，在Workfront中创建新用户时，即使电子邮件地址因大小写而异，也不能再使用其他用户已在使用的电子邮件地址。 例如，如果另一个用户的电子邮件地址为JohnDoe@example.com ，则不能创建电子邮件地址为johndoe@example.com的用户。

## 更新Workfront实例中现有用户的电子邮件地址

作为Workfront管理员，您必须更新其匹配电子邮件地址因大小写不同而不同的现有用户。
要修复Workfront实例中的重复电子邮件地址，请执行以下操作：

1. 检查任何重复用户，并确定不再需要哪个用户。

   1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Workfront的右上角)，然后单击 **用户**. ![](assets/users-icon-in-main-menu.png)

   1. 在 **筛选条件** 菜单，选择 **全部**.

   1. 在 **视图** 菜单，选择 **用户登录**.

   1. 在 **分组** 菜单，选择 **无**.

   1. 自定义用户登录视图。

      1. 单击 **视图** > **自定义视图**.

      1. 更换 **ID** 列中的 **电子邮件地址** 列。

      1. 重命名视图并保存它。
   1. 创建新分组。

      1. 单击 **分组** > **新建分组**.

      1. 单击 **切换到文本模式** 页面右上角的。
      1. 粘贴以下文本模式代码：

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. 重命名分组并保存它。



1. 执行以下任一操作：

   * （首选方法）向每个额外帐户的用户电子邮件地址添加+地址。

      如果您组织中的单个用户需要访问1个以上的用户帐户，请选择此选项。 如果您的电子邮件提供商不支持加号寻址，则必须为每个Workfront帐户提供单独的电子邮件帐户。

      例如，John Doe可以为其日常使用帐户拥有一个用户帐户，以及一个用于测试用途的用户帐户：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * 通过将以下文本附加到电子邮件地址，将域更改为使用伪域：

      `.inactive`

      例如，John Doe可以具有以下域： （这些域必须是唯一的。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      您无法再登录到这些帐户，因为密码重置需要有效的电子邮件地址。 只能使用“登录身份”功能访问这些帐户。

   * 删除不需要的用户

      >[!IMPORTANT]
      >
      >仅针对错误创建的帐户或测试帐户选择此选项。 此选项通常仅对登录错误为零或1的帐户执行。 不应删除已定期使用的帐户。



如果您的Workfront实例中的用户具有匹配的电子邮件地址，这些地址仅因大小写而异，则Workfront将在需要更新这些地址和地址时为您提供其他信息和时间表。
