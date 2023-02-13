---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: 映射用户属性并自动配置新用户
description: 使用单点登录(SSO)，您可以将属性从身份提供者的Active Directory传递到Adobe Workfront用户。 您还可以使用自动配置选项（也称为即时配置或JIT）将新用户添加到Workfront。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 2%

---

# 映射用户属性并自动配置新用户

使用单点登录(SSO)，您可以将属性从身份提供者的Active Directory传递到Adobe Workfront用户。 您还可以使用自动配置选项（也称为即时配置或JIT）将新用户添加到Workfront。

>[!NOTE]
>
>如果贵组织已载入Adobe Admin Console，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。


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

## 映射属性的提示

在映射属性时，请牢记以下几点：

* 始终在“预览”沙盒或“客户刷新”(CR)沙盒中测试。
* 使用管理员帐户和非管理员帐户进行测试，以确认您正确映射属性。
* 每次用户通过单点登录(SSO)登录Workfront时，都会映射属性，而不只是在自动配置期间。

## 映射用户属性并自动配置新用户

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** > **单点登录(SSO)**.

1. 在 **类型** 下拉菜单，单击 **SAML 2.0**.

1. 单击 **映射用户属性**.

   ![](assets/map-user-attributes.png)

1. （可选）如果希望Workfront从Active Directory中自动创建新用户，请单击 **自动配置用户**.

   此功能需要属性映射。

1. 在显示的选项行中，映射您需要的Workfront用户属性。

   您可以映射属性，如地址、经理、作业角色、主页组等。

   属性映射在1:1比率下工作。 例如，您无法设置用户所属的每个组；每个用户只能设置一个。

   >[!IMPORTANT]
   >
   >每个用户都需要以下属性：
   >      
   >* 姓
   >* 名
   >* 电子邮件地址

   >      
   >我们不建议在属性映射中映射访问级别。 如果是这样，请在设置默认值时务必小心，以确保不会无意中删除管理员访问权限。

   下表说明了可用于映射属性的字段：

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront 用户属性</td> 
      <td>选择要映射的属性的名称</td> 
     </tr> 
     <tr> 
      <td role="rowheader">目录属性</td> 
      <td>键入要使用的SSO属性标签。/td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">默认值</td> 
      <td> <p>选择Workfront用户属性后，如果连接期间的值为NULL，则此字段将在系统中填充相应的默认值。 仅当您计划应用属性映射规则时，才在此处键入值（请参阅步骤7）。 默认值会作为这些规则的例外。</td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）单击 **规则** 向属性添加规则。

   1. 在下拉列表中，选择要使用的属性修饰符。
   1. 在右侧的2个字段中，键入目录属性值以及要替换该值的值。

      ![](assets/rule-fields.png)
   您可以单击 **添加规则** 向属性添加更多规则。

1. （可选）要映射更多用户属性，请单击 **添加映射** 重复步骤6-7。
1. 单击&#x200B;**保存**。
