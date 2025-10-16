---
title: 共享项目组合
description: 如果您有访问项目组合的权限，则可以与其他用户共享项目组合。
author: Courtney
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# 共享项目组合

在分配访问级别时，您的Adobe Workfront管理员可以向您授予查看或编辑项目组合的权限。 您必须拥有计划许可证才能编辑项目组合。 有关详细信息，请参阅[授予项目组合](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)的访问权限。

除了授予您的访问级别外，您还可以从可与您共享特定项目组合的用户那里获得查看或管理这些项目的权限。 有关访问级别和权限的详细信息，请参阅[访问级别和权限如何协同工作](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)。

权限特定于Workfront中的一个项目，并定义用户可以对该项目执行的操作。


## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作或更高</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>查看对要共享对象的访问权限或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看要共享对象的权限或更高</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关共享项目组合的注意事项

除了下面的注意事项外，另请参阅[对象权限共享概述](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)。

>[!NOTE]
>
>Workfront管理员可以为系统中的任何项目为所有用户添加或删除权限，而无需成为这些项目的所有者。

* 默认情况下，项目组合的创建者拥有对其的管理权限。
* 您可以单独共享一个项目组合，也可以同时共享多个项目组合。 共享项目组合与在Workfront中共享其他对象相同。 有关信息，请参阅[共享对象](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)。

* 您只能授予项目组合的“查看”或“管理”权限。
</span>
*当您共享项目组合时，默认情况下，用户将继承与项目组合关联的所有子对象的相同权限。

有关Workfront中对象层次结构的详细信息，请参阅[了解Adobe Workfront中的对象](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)。

* 您可以从Portfolio中删除继承的权限。 有关从对象中删除权限的详细信息，请参阅[从对象中删除权限](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)。

## 共享项目组合

{{step1-to-portfolios}}

1. 在&#x200B;**项目组合**&#x200B;页面上，选择要共享的项目组合。 此时将打开项目组合页面。

1. 在项目组合名称的右侧，单击&#x200B;**共享**。 将打开&#x200B;**共享[Portfolio名称]**&#x200B;对话框。

   ![共享项目组合按钮](assets/share-portfolio-button.png)

1. 在&#x200B;**将项目组合访问权限授予**&#x200B;字段中，开始键入要与其共享项目组合的用户、团队、角色、组或公司的名称，然后在名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >您只能与活跃用户、团队、角色或公司共享项目组合。


1. （可选）选择&#x200B;**具有访问权限**&#x200B;下拉列表并选择项目组合的访问级别：

   * **只有受邀人员才能访问：**&#x200B;只有受邀加入项目组合的用户才能访问（默认）。
   * **系统中的每个人都可以查看**：系统中的所有用户都可以查看项目组合，而无需邀请。

1. 单击用户名右侧的下拉列表，然后选择他们对此项目组合的权限级别：

   * **查看**：用户可以查看和共享项目组合。
   * **管理**：用户拥有对项目组合的完全访问权限，但没有管理权限，这些权限是在访问级别授予的（还包括所有查看权限）。

1. （可选）单击您已授予的权限级别旁边的高级选项图标，以配置项目组合的特定权限。

   ![已配置高级权限选项](assets/advanced-options-icon.png)

1. （可选）要使用链接快速共享项目组合，请单击&#x200B;**复制链接**，然后将其转发给收件人。

1. 单击&#x200B;**保存**。

## 批量共享项目组合

{{step1-to-portfolios}}

1. 在&#x200B;**项目组合**&#x200B;页面上，选中要共享的每个项目组合左侧的框，然后单击页面顶部的&#x200B;**共享**&#x200B;图标![共享](assets/share-icon.png)。 这将打开共享模式窗口。

   ![批量共享项目组合](assets/bulk-share-portfolios.png)

1. 在&#x200B;**将项目组合访问权限授予**&#x200B;字段中，开始键入要与其共享项目组合的用户、团队、角色、组或公司的名称，然后在该名称出现在下拉列表中时单击该名称。

   >[!TIP]
   >
   >您只能与活跃用户、团队、角色或公司共享项目组合。


1. （可选）选择&#x200B;**具有访问权限**&#x200B;下拉列表并选择项目组合的访问级别：

   * **只有受邀人员才能访问：**&#x200B;只有受邀加入项目组合的用户才能访问它们（默认）。
   * **系统中的每个人都可以查看**：系统中的所有用户都可以在没有邀请的情况下查看项目组合。


1. 单击用户名右侧的下拉菜单，并为项目组合选择其权限级别：

   * **查看**：用户可以查看和共享项目组合。
   * **管理**：用户拥有对项目组合的完全访问权限，但没有管理权限，这些权限是在访问级别授予的（还包括所有查看权限）。

1. （可选）单击已授予的权限级别旁边的高级选项图标，以配置项目组合的特定权限。

   ![已配置高级权限选项](assets/advanced-options-icon.png)

1. 单击&#x200B;**保存**。


## Portfolio权限

下表显示在允许用户查看或管理Portfolio时，您可以授予用户哪些权限：

| **操作** | **管理** | **查看** |
|---|---|---|
| 编辑Portfolio详细信息 | ✓ |   |
| 查看Portfolio | ✓ | ✓ |
| 删除Portfolio | ✓ |   |
| 附加自定义表单 | ✓ |   |
| 编辑自定义字段 | ✓ |   |
| 添加或删除程序&#42; | ✓ |   |
| 添加或删除项目&#42; | ✓ |   |
| 批准项目 | ✓ |   |
| Portfolio优化&#42; | ✓ |   |
| 添加文档文件夹&#42; | ✓ | ✓ |
| 添加文档 | ✓ | ✓ |
| 更新/评论 | ✓ | ✓ |
| 共享 | ✓ | ✓ |
| 在系统范围内共享 |   | ✓ |

*这些权限由其他对象（如项目、项目群、文档）的访问级别和权限控制。
