---
title: 将费率卡附加到项目
description: 在项目附上费率卡后，按地点及其关联记帐费率列出的所有角色都将添加到项目中。
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# 将费率卡附加到项目

{{highlighted-preview-article-level}}

费率卡根据位置存储每个工作角色的多个计费费率。 您可以让位于巴黎的Designer和位于纽约的第二个Designer担任工作角色，每个角色具有不同的计费率。 但是，费率卡上的工作角色不需要位置。 费率卡上工作角色（以及可能的地点）的计费费率还可以包括有效日期。

在项目附上费率卡后，按地点及其关联记帐费率列出的所有角色都将添加到项目中。

>[!NOTE]
>
>附加费率卡会覆盖项目上的任何现有记帐费率。

您可以直接在项目中从费率卡编辑记帐费率。 这不会影响默认费率卡上存储的费率。

有关创建费率卡的信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)。

有关覆盖项目的工作角色记帐费率和计算项目收入的一般信息，请参阅[覆盖工作角色记帐费率和计算项目收入的概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目和财务数据的访问权限</p> <p>工作角色的管理访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理具有管理财务权限的项目权限 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将费率卡附加到项目

1. 转到项目。
1. 单击左侧面板中的&#x200B;**记帐费率**。 您可能需要先单击&#x200B;**显示更多**。
1. 单击&#x200B;**添加记帐费率>附加费率卡**。

   将打开“附加费率卡”页。 有关详细信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md)。

1. 选择要添加到项目的费率卡，然后单击&#x200B;**附加**。

   费率卡及其所有工作角色费率将添加到计费费率列表。

   ![将评价卡添加到项目](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >在记帐费率列表中，您可以删除一个或多个来自费率卡的工作角色。 从项目中删除工作角色记帐费率不会将其从默认费率卡中删除。
