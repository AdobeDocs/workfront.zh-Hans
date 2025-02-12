---
title: 导入用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 通过从网络目录服务（如Active Directory或其他LDAP目录）同步用户，您可以将用户导入Adobe Workfront站点，也可以使用电子表格导入文件导入用户。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# 导入用户

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Add users" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

-->

您可以使用电子表格导入文件导入用户。

创建新用户之前，首先请确保已创建了要与该用户关联的所有对象。 例如，如果您尚未创建计划，则无法将计划分配给新用户，并且用于将计划与新用户相关联的字段不会显示在“新用户”屏幕中。

## 访问要求

+++ 展开以查看本文中功能的访问要求。

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
   <td><p>新增：标准</p><p>或</p><p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须具备以下条件之一：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>您的访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，在<b>微调您的设置</b> <img src="assets/gear-icon-in-access-levels.png">下启用了<b>创建</b>和两个<b>用户管理</b>选项中的至少一个。 </p> <p>在以下两个选项中，如果启用了<b>用户管理员（组用户）</b>，则您必须是该用户所属的组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用电子表格导入文件导入用户

{{step-1-to-users}}

1. 单击&#x200B;**新建用户**&#x200B;下拉箭头，然后单击&#x200B;**导入用户**。

1. 在显示的&#x200B;**导入用户**&#x200B;框中，下载样例文件，然后更新样例文件以包含您自己的用户个人信息。

   每一行都包含以下字段：

   * **名字**
   * **姓氏**
   * **电子邮件地址**

     电子邮件地址必须是唯一的。

   * **访问级别**

     访问级别区分大小写。

   * **SSO登录ID**

     仅当您系统中启用了SSO时，此字段才包含在内。 您必须在此字段中为每个用户添加联合ID。 从“人员”选项卡创建用户时，如果要允许用户不使用SSO登录，可以设置该用户的密码。 但是，导入功能不允许将SSO登录ID留空。

   * 确保用户的电子邮件地址之前或之后不存在额外的空格。

   完成行的处理时，它应该如下所示：

   ![importing-new-users.png](assets/importing-new-users.png)

1. 将文件保存到工作站上的某个位置。
1. 在&#x200B;**导入用户**&#x200B;框中单击&#x200B;**选择文件**。

1. 导航到并选择您保存的文件。
1. （可选）选择&#x200B;**向此用户发送邀请电子邮件**&#x200B;选项，以便向该用户发送电子邮件邀请，通知他们已创建Workfront帐户，并提示他们设置密码。

   如果要设置用户的密码，请取消选择此选项。

1. 单击&#x200B;**导入**。

   屏幕顶部会显示一条确认消息，指出用户已成功导入。
