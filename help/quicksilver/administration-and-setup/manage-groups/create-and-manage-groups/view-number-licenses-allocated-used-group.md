---
title: 查看组中已分配和使用许可证的数量
description: 作为Adobe Workfront管理员，您可以查看您的组及其子组中当前使用的各个许可证类型的计数。 当您需要评估是否重新分发许可证时，此功能非常有用。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8d1870ea-3f9e-4358-8e14-3dcfc3805637
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 查看组中已分配和使用许可证的数量

作为Adobe Workfront管理员，您可以查看您的组及其子组中当前使用的各个许可证类型的计数。 当您需要评估是否重新分发许可证时，此功能非常有用。

如果您管理的组之上有任何组，则其管理员也可以为您的组执行此操作。 Workfront管理员也是如此（适用于任何组）。

>[!IMPORTANT]
>
>仅当用户的主组是特定组时，该组的许可证才被计入该组。

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
   <td><p>标准</p>
       <p>规划</p></td>
  </tr>
  <tr> 
   <td>访问级别配置</td> 
   <td>您必须是组的组管理员或系统管理员。</td>
  </tr>
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看组中使用的许可证数量

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**组** ![组](assets/groups-icon.png)。

1. 单击组的名称。
1. 在显示的页面上，在右上角附近的标题区域中，查看&#x200B;**个正在使用的许可证**&#x200B;区域，以查看当前正在使用的&#x200B;**计划**&#x200B;和&#x200B;**工作**&#x200B;许可证的数量。

   如果您查看的是顶级组，而Workfront管理员为组定义了每种许可证类型的最大数量，则也会显示这些数量。 例如，在以下组中，最多10个用户可以拥有计划许可证，15个用户可以拥有工作许可证：

   ![已分配的许可证](assets/licenses-used-allocated.png)

   有关Workfront管理员如何为组定义分配许可证的最大数量的信息，请参阅[管理系统中的可用许可证](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md#set)一文中的[设置主组许可证的最大数量](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)部分。

   >[!NOTE]
   >
   >如果您正在查看的组是子组，则只能查看正在使用的许可证数量，而不能查看为该组分配的最大许可证数量。 这是因为Workfront管理员没有为子组定义许可证最大计数。
   >
   >![在子组](assets/subgroup-used-licenses-only.png)中使用了许可证
   >

1. 要单独清点组内当前使用的每种许可证类型（包括审阅和请求），请单击&#x200B;**正在使用的许可证正下方的文本区域：**

   ![单击以查看更多](assets/click-text-to-see-more.png)

   显示的框为所有四种Workfront许可证类型提供了相同的信息：计划、工作、审阅和请求。 在框底部，您可以看到此组或其某个子组的成员正在使用的许可证总数：

   ![更多许可证信息](assets/more-license-info.png)

   对于“查看和请求”许可证，“最大值”列始终显示“无限制”。
