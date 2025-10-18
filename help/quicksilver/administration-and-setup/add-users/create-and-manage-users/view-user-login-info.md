---
title: 查看用户登录信息
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: 通过指示您希望在用户列表视图或用户报表中包含此信息，您可以查看用户登录Workfront的频率以及上次登录的时间。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# 查看用户登录信息

通过指示您希望在用户列表视图或用户报表中包含此信息，您可以查看用户登录Adobe Workfront的频率以及上次登录的时间。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p><p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>您必须具备以下任一项：</p> 
    <ul> 
     <li> <p>系统管理员访问级别。 </li> 
     <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## Workfront如何记录登录信息

Workfront记录以下有关登录系统的用户的信息：

* **登录计数**： Workfront计算每24小时登录到应用程序一次的用户。 如果一位用户使用不同的浏览器、计算机或移动设备多次登录，则Workfront会将一天内发生的所有登录次数计算为一次登录。 登录计数包括从创建用户时开始的信息。
* **上次登录日期**：用户上次登录的日期。 来自任何浏览器、移动设备或其他应用程序的每次登录日期都记录在此字段中。

以下列任一方式登录Workfront均会计为Workfront的登录：

* Workfront Web应用程序
* Workfront移动设备应用程序(iOS或Android设备)
* 任何受支持的Workfront与其他第三方应用程序(如Slack)的集成
* Workfront与其他第三方应用程序之间的任何自定义集成。
* WORKFRONT API

  >[!NOTE]
  >
  >通过Workfront API登录到Workfront仅适用于尚未登记到Adobe Business Platform的组织。

## 在用户列表或报告中显示使用情况信息

您可以在用户列表视图或用户报告中显示“登录计数”和“上次登录日期”字段。\
有关创建报告的详细信息，请参阅[创建自定义报告](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)。

要在用户列表的视图中显示使用信息，请执行以下操作：

1. 转到Workfront中的用户列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 单击屏幕右下角附近的&#x200B;**添加列**。
1. 在&#x200B;**显示在此列**&#x200B;字段中，开始键入&#x200B;**登录计数**，然后当它出现在&#x200B;**用户**&#x200B;下的列表中时将其选中。

1. 再次单击&#x200B;**添加列**。
1. 在&#x200B;**显示在列**&#x200B;字段中，开始键入&#x200B;**上次登录日期**，然后当它出现在&#x200B;**用户**&#x200B;下的列表中时将其选中。

1. （可选）单击&#x200B;**高级选项**，然后从下拉菜单中选择&#x200B;**字段格式**&#x200B;以在列中包含上次登录的时间或星期几。

1. 单击&#x200B;**保存视图**。\
   该视图包含有关用户登录次数和上次登录时间的信息。
