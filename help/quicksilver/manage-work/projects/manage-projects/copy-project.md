---
product-area: projects
navigation-topic: manage-projects
title: 复制项目
description: 您可以复制项目，而不是从头开始创建项目。 您一次只能复制一个项目。 您无法批量复制项目。
author: Alina
feature: Work Management
exl-id: 1bb133a8-eb76-46b8-969f-37f57f9453b4
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 5%

---

# 复制项目

<!--
<(LINKED TO THE PRODUCT IN THE COPY PROJECT BOX)</p>
-->

您可以复制项目，而不是从头开始创建项目。 您一次只能复制一个项目。 您无法批量复制项目。

>[!IMPORTANT]
>
>以下项目永远不会从现有项目复制到新项目：
>
>* 问题
>* 记帐费率
>* 开票记录
>* 注释
>* 小时
>* 跨项目前置任务
>* 预算小时
>
>以下项目始终会从现有项目复制到新项目：
>
>* 任务
>* 模板
>* 风险
>* 队列设置信息
>* Portfolio和计划
>* 记分卡
>* 任务默认信息(任务默认审批流程、任务默认自定义Forms)
>


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
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront许可证*</p> </td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>访问级别配置*</strong> </td> 
   <td> <p>编辑对具有创建功能的项目的访问权限 <span>和复制</span> 项目</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>对象权限</strong> </p> </td> 
   <td> <p>查看项目的权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 复制单个项目

复制项目还会将原始项目中的某些信息复制到新项目。 您还可以指定在复制过程中不应将哪些项目复制到新项目。

复制项目：

1. 转到要复制的项目，然后单击 **更多** 图标 ![](assets/qs-more-menu.png) 项目名称的权限

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   或

   转到项目列表或报表并选择一个项目，然后单击 **更多** 图标 ![](assets/qs-more-menu.png) 列表顶部。

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. 单击 **复制**.

1. 更新新项目的名称。

   默认情况下，新名称为 **副本 `<Original project name>`.**

   ![](assets/copy-project-box-nwe-350x276.png)

1. 选择 **状态** 的URL。

   默认情况下， **状态** 与原始项目的匹配。

1. （可选）取消选择您不希望复制到新项目的项目。 下表说明了取消选择这些项目时会发生的情况：


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部选择</td> 
      <td> <p>选择所有选项并清除新项目中列出的所有字段和对象。</p> <p><b>笔尖</b>

   取消选择 <strong>全选</strong> 取消选择所有项目。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">分配</td> 
      <td>删除所有项目和任务分配</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>删除所有任务的进度，它们显示为“新”。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义数据</td> 
      <td> <p>从项目的自定义表单中删除信息，以及与以下项目关联的自定义表单信息：</p> 
       <ul> 
        <li>任务</li> 
        <li>费用</li> 
        <li> 文档</li> 
       </ul> <p><b>注释</b>

   自定义表单仍附加在任务、费用、文档和项目中，但表单自定义字段中的信息不会复制到新项目中。 </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td> <p>删除“文档”选项卡中的所有内容，包括文档版本、链接的文档和文件夹。</p> <p>默认情况下，文档校样和批准无法复制到其他项目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有前置任务</td> 
      <td> <p>删除项目任务之间的所有前置关系。 </p> <p><b>笔尖</b>

   无论是否选择了跨项目前置项，都不会将其转移到新项目。 </p> </td>
   </tr>

<tr> 
      <td role="rowheader">预算小时</td> 
      <td> <p>从复制的项目中删除在项目业务案例的“资源计划”区域中预算的小时数。</p>

<b>注释</b>

使用方案计划员编入预算的小时数永远不会复制到新项目，因为新项目未与方案计划员中的方案关联。 有关更多信息，请参阅 <a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md">使用方案计划员在业务案例中预算资源</a>
</tr></td>
    <tr> 
      <td role="rowheader">财务信息</td> 
      <td> <p>删除以下区域中的信息： </p> 
       <ul> 
        <li>项目的财务子选项卡</li> 
        <li> 商业案例中的计划效益</li> 
        <li>所有任务的财务信息<br></li> 
       </ul> <p>有关项目“财务”子选项卡的详细信息，请参阅 <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">在项目财务区管理信息</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">批准流程</td> 
      <td>删除与任务或项目关联的所有批准。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> 删除与任务或项目关联的提醒通知。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费用</td> 
      <td>删除与任务或项目相关的费用。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td> 删除所有用户对任务或项目的权限。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **复制** 创建项目副本。

   这会创建一个与您复制的项目类似的新项目。

   您可以开始更改新复制的项目，如审核任务分配或调整时间轴。
