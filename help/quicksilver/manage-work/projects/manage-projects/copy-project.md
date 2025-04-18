---
product-area: projects
navigation-topic: manage-projects
title: 复制项目
description: 您可以复制项目，而不是从头开始创建项目。 您一次只能复制一个项目。 无法批量复制项目。
author: Alina
feature: Projects, Work Management
role: User
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 4%

---

# 复制项目

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

您可以复制项目，而不是从头开始创建项目。 您一次只能复制一个项目。 无法批量复制项目。

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
> 项目上原始任务的日期复制到新项目。 您必须更改项目的开始日期或完成日期（取决于其计划模式）以更新任务的日期。 任务限制可能会阻止您更改项目的日期。

## 访问要求

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Copy</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>View permissions or higher to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront计划*</p> </td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>编辑对能够创建<span>和复制</span>项目的项目的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>查看项目的权限或更高版本</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 复制单个项目

复制项目也会将原始项目中的一些信息复制到新项目中。 您还可以指定在复制过程中不应将哪些项复制到新项目。

要复制项目，请执行以下操作：

1. 转到要复制的项目，然后单击项目名称右侧的&#x200B;**更多**&#x200B;图标![更多菜单](assets/qs-more-menu.png)

   ![更多下拉列表](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报告并选择项目，然后单击列表顶部的&#x200B;**更多**&#x200B;图标![更多菜单](assets/qs-more-menu.png)。

   ![更多菜单已展开](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 单击&#x200B;**复制**。

1. 更新新项目的名称。

   默认情况下，新名称为`<Original project name>`的&#x200B;**副本。**

   ![复制项目框](assets/copy-project-box-nwe-350x276.png)

1. 为新项目选择&#x200B;**状态**。

   默认情况下，**状态**&#x200B;与原始项目的状态匹配。

1. （可选）取消选择不想复制到新项目的项。 下表描述了取消选择项目时发生的情况：


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部选择</td> 
      <td> <p>选择所有选项并清除新项目中列出的所有字段和对象。</p> <p><b>提示</b>

   取消选择<strong>全选</strong>将取消选择所有项。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">任务</td> 
      <td>删除所有项目和任务分配</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>删除所有任务的进度，这些任务显示为“新建”。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义数据</td> 
      <td> <p>删除项目上自定义表单中的信息，以及与以下项目关联的自定义表单上的信息：</p> 
       <ul> 
        <li>任务</li> 
        <li>费用</li> 
        <li> 文档</li> 
       </ul> <p><b>注释</b>

   自定义表单仍然附加到任务、费用、文档和项目，但表单自定义字段中的信息不会复制到新项目。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td> <p>删除文档选项卡中的所有内容，包括文档版本、链接的文档和文件夹。</p> <p>默认情况下，文档验证和审批无法复制到其他项目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任务</td> 
      <td> <p>删除项目上任务之间的所有前置任务关系。 </p> <p><b>提示</b>

   跨项目前置任务从不转移到新项目，无论是否选择此选项。 </p> </td>
   </tr>

<tr> 
      <td role="rowheader">预算小时</td> 
      <td> <p>从复制的项目中删除项目业务案例的资源计划区域中预算的小时数。</p>

<b>注释</b>

绝不会将使用方案规划器的预算小时数复制到新项目，因为新项目未链接到方案规划器中的方案。 有关详细信息，请参阅使用场景规划器</a>的业务案例中的<a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">预算资源
</tr></td>
    <tr> 
      <td role="rowheader">财务信息</td> 
      <td> <p>删除以下区域中的信息： </p> 
       <ul> 
        <li>项目的财务子选项卡</li> 
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

1. 单击&#x200B;**复制**&#x200B;以创建项目副本。

   这将创建一个新项目，该项目与您复制的项目类似。

   您可以开始更改新复制的项目，如审核任务分配或调整时间线。
