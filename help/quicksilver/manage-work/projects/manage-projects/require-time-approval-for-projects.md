---
product-area: projects
navigation-topic: manage-projects
title: 项目需要批准时间
description: 项目需要批准时间
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# 项目需要批准时间

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

您可以将项目配置为要求针对项目记录的小时数由项目所有者批准。 如果以这种方式进行配置，则必须先由项目所有者批准小时数，然后才能将其用于帐单记录。\
有关开票记录的详细信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)。

>[!NOTE]
>
>启用此选项不会移除时间表批准者批准时间表上时间的能力。 如果项目所有者不批准或拒绝时间，时间表批准者仍然可以批准时间表上的时间。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>需要时间才能批准项目的计划</p>
   <p>查看或更高版本以批准项目记录的小时数</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目或更高版本的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高版本的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他访问权限</td> 
   <td> <p>要批准项目时间，您必须至少满足以下条件之一：</p> 
    <ul> 
     <li>您是具有上述指定访问权限的项目所有者。 在这种情况下，如果存在以下条件之一，您可以执行以下操作： 
      <ul>
       <li>如果您拥有项目的管理权限，则可以批准或拒绝任何其他用户登录项目的小时数。</li>
       <li> 如果您拥有项目的Contribute或查看权限，则只能批准或拒绝您或报告您的任何其他用户记录的小时数。<br></li>
      </ul></li> 
     <li>您拥有对时间表和小时数的管理访问权限的计划许可证。 在本例中：
      <ul>
       <li>您可以批准或拒绝您至少具有查看权限的项目上的任何小时数。 </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 项目需要批准时间

要要求项目经理审批项目小时，请执行以下操作：

1. 转到要请求批准小时数的项目。
1. 单击项目名称右侧的&#x200B;**更多**&#x200B;图标![](assets/more-icon.png)，然后单击&#x200B;**编辑**。\
   此时将显示编辑项目对话框。

1. 在&#x200B;**项目设置**&#x200B;部分中，选择&#x200B;**需要时间来批准此项目**。
1. 单击&#x200B;**保存**。\
   现在，当时间被记录并批准时，这些小时将被锁定，并且无法在项目或时间表中输入这些小时数的用户无法对其进行更改。 只有Workfront管理员可以调整记录时间。

## 批准和拒绝项目的时间

作为项目经理，您可以批准或拒绝为任务、问题或项目记录的小时数。

在项目级别批准小时数不会影响任何记录小时数的用户的工时表。 例如，项目中的小时数可能由项目经理批准，但时间表仍然有待用户的经理或时间表批准者批准。 

如果您将项目设置为要求审批记录的小时数，则项目经理必须审批该小时数，以便将其包含在项目的开票记录中。 有关创建开票记录的更多信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)。

要批准或拒绝项目的小时数，请执行以下操作：

1. 转到项目。
1. 单击左侧面板中的&#x200B;**小时**&#x200B;区域。 此区域可能位于&#x200B;**显示更多**&#x200B;区域下。

1. 为问题、任务和项目显示记录的小时数，其状态应为&#x200B;**已提交**。\
   单击小时条目左侧的框以选择要批准的小时。

1. 单击&#x200B;**批准**。\
   小时数状态更改为&#x200B;**已批准**。\
   如果您稍后拒绝批准的小时数，小时数的状态将更改为&#x200B;**未批准**。\
   当您在开票记录中包含批准的小时数时，小时数的状态将更改为&#x200B;**已开票和已批准**。 无法删除添加到开票记录的小时数。 有关创建开票记录的更多信息，请参阅文章[创建开票记录](../../../manage-work/projects/project-finances/create-billing-records.md)

1. （可选）单击&#x200B;**拒绝**&#x200B;以拒绝项目上的时间条目。\
   小时数状态更改为&#x200B;**已拒绝**。
