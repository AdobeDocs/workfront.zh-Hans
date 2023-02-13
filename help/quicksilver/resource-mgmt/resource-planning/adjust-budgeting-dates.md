---
product-area: resource-management
navigation-topic: resource-planning
title: 在资源计划器中调整预算日期
description: 如果您发现在资源计划员中预算资源后资源存在超额分配，则可以通过将预算小时数、FTE或成本移至另一个时间范围来探索假设方案。 然后，根据这些情景中的发现结果，您可以调整预算的工时、FTE或成本。
author: Alina
feature: Resource Management
exl-id: bc49d45a-73a5-4b02-9054-9c9dbb54224d
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 1%

---

# 在资源计划器中调整预算日期

如果您发现在资源计划员中预算资源后资源存在超额分配，则可以通过将预算小时数、FTE或成本移至另一个时间范围来探索假设方案。 然后，根据这些情景中的发现结果，您可以调整预算的工时、FTE或成本。

如果资源的预算小时数、FTE或成本高于其可用小时数、FTE或成本，则会显示超额分配。 这会生成负净值。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>专业及更高级别</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对资源管理的访问权限，包括对资源计划员中“编辑优先级”和“预算小时数”的访问权限</p> <p>编辑对财务数据、项目和用户的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理要预算信息的项目的权限，并能够管理财务</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 调整预算日期

1. 转至资源计划员并选择 **按项目查看**.

   >[!NOTE]
   >
   >只有在按项目查看资源计划员时，您才可以使用“调整预算日期”选项。

1. 将鼠标悬停在项目名称上，然后单击 **更多** 菜单。
1. 单击 **调整预算日期**.\
   随即会显示项目分配时间轴。\
   如果存在预算冲突，则当前预算小时数的时间范围以橙色突出显示；如果不存在冲突，则以蓝色突出显示。

   ![](assets/rp-adjust-budgeting-dates-with-no-done-button-350x63.png)

1. 将突出显示的时间范围拖放到另一个时间，以了解所选项目的预算冲突不在何处。 当您找到净值为正的时间范围时，突出显示的时间范围将变为蓝色。
1. 单击项目分配时间轴右上角的“x”以将其关闭。
1. 从项目的现有时间轴中删除已预算的小时数，并将其添加到显示最可用时间轴。
1. 单击&#x200B;**保存**。
1. （视情况而定，可选）如果没有预算冲突的时间范围在项目时间线之外，请单击项目名称以访问项目。
1. （视情况而定）单击 **编辑项目**，然后编辑 **计划开始日期** 或 **计划完成日期** 修改项目的时间表，而不会与预算冲突。\
   有关编辑项目的更多信息，请参阅文章 [编辑项目](../../manage-work/projects/manage-projects/edit-projects.md).

1. （视情况而定）单击 **保存更改**.
1. 返回到资源计划员，并在没有预算冲突的时间范围内重新输入预算小时数、FTE或成本。
1. 单击&#x200B;**保存**。
