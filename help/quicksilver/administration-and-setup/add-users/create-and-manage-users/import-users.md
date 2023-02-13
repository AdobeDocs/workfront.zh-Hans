---
title: 导入用户
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以通过从网络目录服务（如Active Directory或其他LDAP目录）同步用户，将用户导入Adobe Workfront站点，也可以使用电子表格导入文件导入用户。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3dd99d01-a32f-4af8-90e3-f8c0e9027651
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

# 导入用户

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>有关在Adobe Admin Console中编辑用户配置文件的说明，请参阅文章中的“添加用户”部分 [批量上传用户](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) 或联系Adobe Admin Console管理员。
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

您可以使用电子表格导入文件导入用户。

在创建新用户之前，首先确保已创建要与该用户关联的所有对象。 例如，如果尚未创建计划，则无法将计划分配给新用户，并且用于将计划与新用户关联的字段不会显示在新用户屏幕中。

## 访问要求

您必须具备以下条件才能执行本文中的步骤：

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
   <td> <p>您必须具有以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 有关信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>. </p> </li> 
     <li> <p><b>用户</b> 在配置为 <b>编辑</b> 访问，使用 <b>创建</b> 至少两个中的一个 <b>用户管理员</b> 在 <b>优化设置</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>在这两个选项中，如果用户 <b>管理员（群组用户）</b> 启用后，您必须是用户所属的组的组管理员。</p> <p>有关 <b>用户</b> 在访问级别中设置，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">授予用户访问权限</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 使用电子表格导入文件导入用户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **用户** ![](assets/users-icon-in-main-menu.png).

1. 单击 **新用户** 下拉箭头，然后单击 **导入用户**.

1. 在 **导入用户** 框中，下载样例文件，然后更新样例文件以包含您自己的用户个人信息。

   每行包含以下字段：

   * **姓**
   * **名**
   * **电子邮件地址**

      电子邮件地址必须唯一。

   * **访问级别**

      访问级别区分大小写。

   * **SSO 登录 ID**

      仅当系统中启用了SSO时，才会包含此字段。 您必须在此字段中为每个用户添加联合ID。 当您从“人员”选项卡创建用户时，如果您希望允许用户在没有单点登录(SSO)的情况下登录，则可以为用户设置密码。 但是，导入功能不允许将SSO登录ID留空。

   * 确保用户电子邮件地址之前或之后不存在额外空格。

   完成行后，应该如下所示：

   ![importing-new-users.png](assets/importing-new-users.png)

1. 将文件保存到工作站上的某个位置。
1. 单击 **选择文件** 在 **导入用户** 框中。

1. 导航到并选择保存的文件。
1. （可选）选择 **向此用户发送邀请电子邮件** 选项向用户发送电子邮件邀请，通知他们已创建Workfront帐户并提示他们设置密码。

   如果要为用户设置密码，请取消选择此选项。

1. 单击 **导入**.

   您会在屏幕顶部收到一条确认消息，指出用户已成功导入。
