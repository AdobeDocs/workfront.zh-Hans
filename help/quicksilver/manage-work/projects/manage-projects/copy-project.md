---
product-area: projects
navigation-topic: manage-projects
title: 复制项目
description: 您可以复制项目，而不是从头开始创建项目。 您一次只能复制一个项目。 无法批量复制项目。
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 5%

---

# 复制项目

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

<!-- Audited: 5/2025 -->

您可以从现有项目复制项目，而不是从头开始创建项目，这样有助于节省时间。

请注意，您不能批量复制项目。

>[!IMPORTANT]
>
>绝不会将以下项从现有项目复制到新项目：
>
>* 问题
>* 记帐费率
>* 开票记录
>* 注释
>* 小时
>* 跨项目前置任务
>* 预算小时
>
>始终将以下项从现有项目复制到新项目：
>
>* 任务
>* 模板
>* 风险
>* 队列设置信息
>* Portfolio和程序
>* 记分卡
>* 任务默认信息(任务默认审批流程、任务默认自定义Forms)
>
> 原始项目的任务日期将复制到新项目中。 您必须更改项目的开始日期或完成日期（取决于其计划模式）以更新任务日期。 任务限制可能会阻止您更改项目的日期。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。
您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront包</p> </td>  
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证</p> </td> 
   <td> <p>标准</p> 
   <p>规划</p>
      </td> 
  </tr> 
     <td>访问级别配置 </td> 
   <td> <p>编辑对项目的访问权限，并具有创建和复制项目的功能</p> </td> 
  </tr>

<td> <p>对象权限 </p> </td> 
   <td> <p>查看项目的权限或更高版本</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td> <p>New: Standard </p> 
   <p>Or</p>
   <p>Current: Plan </p>
   
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configurations </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>View permissions or higher to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## 复制单个项目

复制项目也会将原始项目中的一些信息复制到新项目中。 您还可以指定在复制过程中不应将哪些项复制到新项目。

要复制项目，请执行以下操作：

{{step1-to-projects}}

1. 从项目列表中选择要复制的项目，然后单击项目名称右侧的&#x200B;**更多**&#x200B;图标![更多菜单](assets/more-icon.png)。

   或

   转到项目列表或报告并选择项目，然后单击列表顶部的&#x200B;**更多**&#x200B;图标![更多菜单](assets/more-icon.png)。

1. 在&#x200B;**更多**&#x200B;下拉菜单中，单击&#x200B;**复制**。 出现&#x200B;**项目名称[的]**&#x200B;副本对话框。

1. （可选）更新&#x200B;**项目名称**。 默认情况下，新名称为&#x200B;**副本[原始项目名称]**。

   ![复制项目框](assets/copy-of-project-box.png)

1. 选择&#x200B;**状态**。 默认情况下，原始项目的状态为选中。

1. （可选）取消选择不想复制到新项目的项。 下表描述了取消选择项目时发生的情况：


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部选择</td> 
      <td> <p>选择所有选项并清除新项目中列出的所有字段和对象。 </p>

   <p> 取消选择此选项将取消选择所有项。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">任务</td> 
      <td>删除所有项目和任务分配。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>删除所有任务的进度，将其显示为新任务。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义数据</td> 
      <td> <p>删除项目上自定义表单中的信息，以及与以下项目关联的自定义表单上的信息：</p> 
       <ul> 
        <li>任务</li> 
        <li>费用</li> 
        <li> 文档</li> 
       </ul> 
      <p>自定义表单仍然附加到任务、费用、文档和项目，但表单自定义字段中的信息不会复制到新项目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td> <p>删除“文档”选项卡中的所有内容，包括文档版本、链接的文档和文件夹。</p> <p>默认情况下，文档验证和审批无法复制到其他项目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任务</td> 
      <td> <p>删除项目上任务之间的所有前置任务关系。 </p> <p>

   跨项目前置任务从不转移到新项目，无论是否选择此选项。 </p> </td>
   </tr>

<tr> 
      <td role="rowheader">预算小时</td> 
      <td> <p>从复制的项目中删除项目业务案例的资源计划区域中预算的小时数。</p> 
    <p>
   绝不会将使用方案规划器的预算小时数复制到新项目，因为新项目未链接到方案规划器中的方案。 有关详细信息，请参阅使用场景规划器<a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">的业务案例中的</a>预算资源</p>
   </tr></td>
    <tr> 
      <td role="rowheader">财务信息</td> 
      <td> <p>删除以下区域中的信息： </p> 
       <ul> 
        <li>项目的“财务”子选项卡</li> 
        <li> 业务案例中的计划收益</li> 
        <li>来自所有任务的财务信息<br></li> 
       </ul> <p>有关项目财务子选项卡的详细信息，请参阅<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">管理项目财务区域的信息</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td>删除与任务或项目关联的所有批准。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> 删除与任务或项目关联的提醒通知。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>删除与任务或项目关联的费用。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td> 删除对任务或项目上所有用户的权限。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**复制项目**。 将创建复制的项目。
