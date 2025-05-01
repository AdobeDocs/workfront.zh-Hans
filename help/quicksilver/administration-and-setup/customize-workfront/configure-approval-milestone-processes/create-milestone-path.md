---
title: 创建里程碑路径
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: 作为Adobe Workfront管理员，您可以创建里程碑路径，这些路径随后可以应用于系统中的任何项目。 您对此区域中的里程碑路径所做的更改会影响整个Workfront系统。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 6e2e337969fccba88ea7089fe9a6d9db605343f7
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 3%

---

# 创建里程碑路径

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

作为Adobe Workfront管理员，您可以创建里程碑路径，这些路径随后可以应用于系统中的任何项目。 您对此区域中的里程碑路径所做的更改会影响整个Workfront系统。

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
   <td>规划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 里程碑和里程碑路径

您可以将项目中的关键任务与预定义的里程碑关联。 此功能可为经理和其他利益相关者提供项目进展情况的高级概述。

所有预定义里程碑的总和称为里程碑路径。

构建里程碑路径的第一步是确定里程碑步骤并确定里程碑。 由于您可以将里程碑路径关联到多个项目，因此里程碑步骤必须是任何项目的常规阶段或阶段。

有关如何将里程碑路径与项目关联以及里程碑与任务关联的更多信息，请参阅[将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。

## 创建里程碑路径

{{step-1-to-setup}}

1. 单击&#x200B;**进程** > **里程碑路径**。
1. 单击&#x200B;**新建里程碑路径。**
1. 在&#x200B;**基本信息**&#x200B;区域中指定以下信息：

   <table style="table-layout:auto">
    <tr>
      <td>创建里程碑路径</td>
       <td>输入里程碑路径的名称。</td>
    </tr>
    <tr>
      <td>描述</td>
      <td>输入描述以定义里程碑路径。</td>
    </tr>
    <tr>
       <td>为活动</td>
      <td>如果希望里程碑路径处于活动状态，请选中此复选框。 其他用户可以在创建或编辑项目时找到此路径并将其附加到项目。 无法将非活动里程碑路径附加到项目。 默认情况下启用此功能。</td>
    </tr>
    <tr>
      <td>组</td>
      <td>选择列出的组，以允许这些组中的用户查看此里程碑路径并将其应用于其项目。 默认情况下，进入里程碑路径的用户的主组处于选中状态。</td>
    </tr>
   </table>

1. 在&#x200B;**里程碑**&#x200B;区域中指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td>键入每个里程碑的描述性名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>键入里程碑的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">颜色</td> 
      <td> <p>选择要与里程碑关联的颜色。 </p> <p>如果不选择颜色，系统将选择里程碑路径中使用的最后一种颜色。 我们建议您为每个里程碑选择唯一的颜色。 颜色用于可视化和报表目的。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**添加里程碑**&#x200B;并根据需要继续添加里程碑，直到路径完成。

1. 单击&#x200B;**创建里程碑路径**&#x200B;以保存更改。

   您的里程碑路径已准备好与项目关联。

   有关如何将里程碑路径与项目关联以及将里程碑与任务关联的更多信息，请参阅[将里程碑与任务关联](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md)。


1. （可选）单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export-icon.png)，然后从以下格式中选择以将里程碑路径列表导出到文件：

   * PDF
   * Excel
   * Excel (xlsx)
   * 制表符分隔

1. （可选）在里程碑列表中选择一个里程碑，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)以编辑里程碑信息。
1. （可选）在里程碑列表中选择一个里程碑，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete-icon.png)将其删除。
1. 单击&#x200B;**是，将其删除**。
该里程碑已被删除并且无法恢复。 与里程碑关联的任何项目信息以及与里程碑路径关联的任何任务信息也会被删除。


## 在项目报告中查看里程碑路径详细信息

您可以在项目报告中查看里程碑路径的详细信息。

必须先将里程碑路径与项目关联，然后才能在项目报告中查看其详细信息。

有关将里程碑路径关联到项目的信息，请参阅[编辑项目](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md)。

{{step1-to-reports}}

1. 单击&#x200B;**新建报告**，然后单击&#x200B;**项目**。
1. 单击&#x200B;**添加列**。
1. 在&#x200B;**显示在此列**&#x200B;的区域中，开始输入&#x200B;**里程碑路径**，然后在显示时单击&#x200B;**里程碑路径名称**。
1. （可选）单击&#x200B;**筛选器**&#x200B;并将以下筛选器添加到报表中： **项目里程碑路径ID不为空**。

   该过滤器可确保只显示与报告中的里程碑路径关联的项目。

1. 单击&#x200B;**保存+关闭**。
1. 为报告添加名称，然后单击&#x200B;**应用**。

   此时将显示项目报告。 与每个项目关联的里程碑路径将显示在报告的最后一列。
1. 单击报表最后一列中的里程碑路径的名称。

   此时将显示里程碑路径的详细信息。

   项目报告中的![里程碑路径详细信息](assets/milestone-details-from-project-report.png)

   里程碑路径详细信息页面显示以下信息：

   * 里程碑路径名称、ID和描述
   * 里程碑路径组
   * 里程碑名称、描述、颜色和颜色图标

1. （可选）单击&#x200B;**返回**&#x200B;以返回项目报告。



