---
product-area: resource-management
navigation-topic: resource-planning
title: 在资源规划程序中调整预算日期
description: 如果您在资源规划程序中预算资源后发现资源过度分配，则可以通过将预算小时数、FTE或成本移至另一个时间范围来探索假设分析方案。 然后，您可以根据这些方案中的发现调整预算小时数、FTE或成本。
author: Lisa
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# 在资源规划程序中调整预算日期

如果您在资源规划程序中预算资源后发现资源过度分配，则可以通过将预算小时数、FTE或成本移至另一个时间范围来探索假设分析方案。 然后，您可以根据这些方案中的发现调整预算小时数、FTE或成本。

当资源的预算小时数、FTE或成本高于其可用小时数、FTE或成本时，可能会出现过度分配。 这将生成负净值。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
    <td><p>新建：任何</p>
       <p>或</p>
       <p>当前： Pro或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>新增：标准</p>
       <p>或</p>
       <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对资源管理的访问权限，包括访问资源规划者中的编辑优先级和预算小时数</p> <p>编辑对财务数据、项目和用户的访问权限</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要为其预算信息的项目的权限，并具有管理财务的能力</p></td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 调整预算日期

1. 转到资源规划者，然后选择&#x200B;**按项目查看**。

   >[!NOTE]
   >
   >只有在您按项目查看资源规划者时，才能使用调整预算日期选项。

1. 将鼠标悬停在项目名称上，然后单击&#x200B;**更多**&#x200B;菜单。
1. 单击&#x200B;**调整预算日期**。\
   此时将显示项目分配时间线。\
   如果存在预算冲突，则当前预算小时数的时间范围以橙色突出显示；如果没有冲突，则以蓝色突出显示。

   ![调整预算日期](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. 将突出显示的时间范围拖放到另一个时间，以了解所选项目在预算方面没有冲突的位置。 当找到一个净值为正的时间范围时，突出显示的时间范围将变为蓝色。
1. 单击项目分配时间线右上角的“x”以将其关闭。
1. 从项目的现有时间线中删除预算小时数，并将它们添加到显示最可用的时间线中。
1. 单击&#x200B;**保存**。
1. （有条件，可选）如果不存在预算冲突的时间范围在项目的时间表之外，请单击项目名称以访问该项目。
1. （有条件且可选）单击&#x200B;**编辑项目**，然后编辑&#x200B;**计划开始日期**&#x200B;或&#x200B;**计划完成日期**，以修改时间范围内的项目时间线，且无预算冲突。\
   有关编辑项目的详细信息，请参阅文章[编辑项目](../../manage-work/projects/manage-projects/edit-projects.md)。

1. （有条件，可选）单击&#x200B;**保存更改**。
1. 返回到资源规划者并在时间范围内重新输入预算小时数、FTE或成本，而不发生预算冲突。
1. 单击&#x200B;**保存**。
