---
title: 查看用户登录信息
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 您可以通过以下方式查看用户登录Workfront的频率以及上次登录的时间：指示您希望在用户列表视图或用户报表中包含此信息。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# 查看用户登录信息

您可以通过以下方式查看用户登录Adobe Workfront的频率以及上次登录的时间：指示您希望在用户列表视图或用户报表中包含此信息。

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
   <td> <p>计划 </p>   </td> 
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

## Workfront如何记录登录信息

Workfront记录有关用户登录到系统的以下信息：

* **登录计数**:Workfront会将登录应用程序的用户计为每24小时一次。 如果一个用户使用不同的浏览器、计算机或移动设备多次登录，则Workfront会将一天内发生的所有登录计为一次登录。 登录计数包括从创建用户时开始的信息。
* **上次登录日期**:用户登录的上次日期。 任何浏览器、移动设备或其他应用程序的每次登录日期都记录在此字段中。

通过以下任何方式登录Workfront即计为登录Workfront:

* Workfront Web应用程序
* Workfront移动设备应用程序(iOS或Android设备)
* 任何支持的Workfront与其他第三方应用程序(Slack、Jira)的集成
* Workfront与其他第三方应用程序之间的任何自定义集成。
* Workfront API

   >[!NOTE]
   >
   >通过Workfront API登录Workfront仅适用于尚未载入Adobe业务平台的组织。

## 在用户列表或报表中显示使用信息

您可以在用户列表视图或用户报表中显示“登录计数”和“上次登录日期”字段。\
有关创建报表的更多信息，请参阅 [创建自定义报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

要在用户列表视图中显示使用信息，请执行以下操作：

1. 转到Workfront中的用户列表。
1. 从 **查看** 下拉菜单，选择 **新建视图**.

1. 单击 **添加列** 屏幕右下角附近。
1. 在 **在此列中显示** 字段，开始键入 **登录计数**，然后在下面的列表中显示时选择它 **用户**.

1. 单击 **添加列** 再次。
1. 在 **在列中显示** 字段，开始键入 **上次登录日期**，然后在下面的列表中显示时选择它 **用户**.

1. （可选）单击 **高级选项**，然后选择 **字段格式** 从下拉菜单中，将上次登录的时间或日期包含在列中。

1. 单击 **保存视图**.\
   该视图包含有关用户登录次数和上次登录时间的信息。
