---
product-area: projects
navigation-topic: manage-projects
title: 需要时间来批准项目
description: 需要时间来批准项目
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 需要时间来批准项目

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

您可以将项目配置为要求针对项目记录的小时数由项目所有者批准。 以这种方式配置小时数后，必须先获得项目所有者的批准，然后才能有资格在帐单记录中使用小时数。\
有关帐单记录的更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>启用此选项不会删除工时单审批者批准工时单时间的能力。 如果项目所有者不批准或拒绝时间，则时间表审批者仍可以批准时间表的时间。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划在项目上需要时间获得批准</p>
   <p>审阅或更高版本以批准在项目上记录的小时数</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目或更高版本的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高级别的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他访问</td> 
   <td> <p>您必须至少满足以下条件之一才能批准项目时间：</p> 
    <ul> 
     <li>您是具有上述指定访问权限的项目所有者。 在这种情况下，如果存在以下任一条件，您可以执行以下操作： 
      <ul>
       <li>如果您对项目具有“管理”权限，则可以批准或拒绝任何其他用户登录项目的小时数。</li>
       <li> 如果您对项目具有“参与”或“查看”访问权限，则只能批准或拒绝您或任何其他报告您的用户记录的小时数。<br></li>
      </ul></li> 
     <li>您拥有计划许可证，并具有对工时单和工时的管理访问权限。 在这种情况下：
      <ul>
       <li>您可以批准或拒绝您对项目至少具有“查看”权限的任何小时。 </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 需要时间来批准项目

要要求项目经理在项目上批准数小时，请执行以下操作：

1. 转到您需要批准的项目，时间长达数小时。
1. 单击 **更多** 图标 ![](assets/more-icon.png) 在项目名称的右侧，单击 **编辑**.\
   此时将显示“编辑项目”对话框。

1. 在 **项目设置** 选择 **需要时间批准此项目**.
1. 单击&#x200B;**保存**。\
   现在，当时间被记录和批准时，这些时间会被锁定，并且无法由在项目或时间表中输入这些时间的用户更改这些时间。 只有Workfront管理员才能调整记录的时间。

## 批准和拒绝项目时间

作为项目经理，您可以批准或拒绝为任务、问题或项目记录的小时数。

在项目级别批准工时不会对记录工时的任何用户的工时单产生任何影响。 例如，项目中的工时数可能由项目经理批准，但工时单仍有待用户经理或工时单审批者批准。 

如果您将项目设置为要求在记录的小时数内进行批准，项目经理必须批准该小时数，以便这些小时数可以包含在项目的开单记录中。 有关创建账单记录的更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md).

要批准或拒绝某个项目的工时，请执行以下操作：

1. 转到项目。
1. 单击 **小时** 的上界。 此名称可能位于 **显示更多** 的上界。

1. 系统将显示问题、任务和项目的记录小时数，该小时数的状态应为 **已提交**.\
   单击小时条目左侧的框以选择要批准的小时。

1. 单击 **批准**.\
   小时的状态将更改为 **已批准**.\
   如果您稍后拒绝批准的小时，小时的状态将更改为 **未批准**.\
   当您在帐单记录中包含已批准的小时数时，小时的状态将更改为 **已计费和已批准**. 无法删除添加到帐单记录的小时数。 有关创建账单记录的更多信息，请参阅文章 [创建帐单记录](../../../manage-work/projects/project-finances/create-billing-records.md)

1. （可选）单击 **拒绝** 以拒绝项目上的时间条目。\
   小时的状态将更改为 **被拒绝**.
