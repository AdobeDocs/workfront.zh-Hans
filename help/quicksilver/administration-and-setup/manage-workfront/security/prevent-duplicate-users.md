---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: 防止重复用户
description: 在Adobe Workfront中创建新用户时，即使电子邮件地址因大小写而异(例如JohnDoe@example.com和johndoe@example.com)，您也无法再使用其他用户已在使用的电子邮件地址。 此外，为了为将来的身份验证增强做好准备，请确保所有用户在Workfront实例中都有唯一的电子邮件地址。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6f5b9e7638a85eca16d722cec6185cd5ed755eca
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# 防止重复用户

在Adobe Workfront中创建新用户时，即使电子邮件地址因大小写而异(例如JohnDoe@example.com和johndoe@example.com)，您也无法再使用其他用户已在使用的电子邮件地址。 此外，为了为将来的身份验证增强做好准备，请确保所有用户在Workfront实例中都有唯一的电子邮件地址。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

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
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 演练

<!--WRITER
<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>
-->

[观看此功能的视频演示。](https://vimeo.com/371505632/2e6938ce06)

## 使用唯一的电子邮件地址创建用户

从2019.4版本开始，在Workfront中创建新用户时，即使电子邮件地址会因大小写而异，您也无法再使用其他用户已在使用的电子邮件地址。 例如，如果另一个用户的电子邮件地址为johndoe@example.com，则不能创建一个电子邮件地址为JohnDoe@example.com的用户。

## 更新您的Workfront实例中现有用户的电子邮件地址

作为Workfront管理员，您必须更新具有匹配电子邮件地址且仅因大小写而异的现有用户。
要修复Workfront实例中重复的电子邮件地址，请执行以下操作：

1. 检查任何重复的用户，并确定不再需要哪个用户。

   1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Workfront的右上角，单击 **用户**. ![](assets/users-icon-in-main-menu.png)

   1. 在 **过滤器** 菜单，选择 **全部**.

   1. 在 **查看** 菜单，选择 **用户登录**.

   1. 在 **分组** 菜单，选择 **无**.

   1. 自定义用户登录视图。

      1. 单击 **查看** > **自定义视图**.

      1. 替换 **ID** 列 **电子邮件地址** 列。

      1. 重命名视图并保存它。
   1. 创建新分组。

      1. 单击 **分组** > **新建分组**.

      1. 单击 **切换到文本模式** 的双曲余切值。
      1. 粘贴以下文本模式代码：

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. 重命名“分组”并保存它。



1. 执行以下任一操作：

   * （首选方法）为每个附加帐户的用户电子邮件地址添加一个+地址。

      如果贵组织中的单个用户需要访问超过1个用户帐户，请选择此选项。 如果电子邮件提供商不支持加号地址，则必须为每个Workfront帐户提供单独的电子邮件帐户。

      例如，John Doe可以为其日常使用帐户提供一个用户帐户，并为测试目的使用一个用户帐户：

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * 通过将以下文本附加到电子邮件地址，可更改域以使用假域：

      `.inactive`

      例如，John Doe可以具有以下域：（这些值必须唯一。）

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      您无法再登录这些帐户，因为密码重置需要有效的电子邮件地址。 只能使用“登录为”功能访问这些帐户。

   * 删除不需要的用户

      >[!IMPORTANT]
      >
      >仅为错误创建的帐户或测试帐户选择此选项。 此选项通常仅对登录次数为零或错误为1的帐户执行。 经常使用的帐户绝不得删除。



如果您在Workfront实例中的用户具有匹配的电子邮件地址，这些地址因用例而异，Workfront将与您联系，提供其他信息以及需要更新这些地址的时间表。
