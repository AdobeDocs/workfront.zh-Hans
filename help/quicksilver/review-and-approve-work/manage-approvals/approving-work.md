---
product-area: projects
navigation-topic: approvals
title: 审批工作
description: 审批工作
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 7366e3dd37b686a3566ca6d39e28eb6762c6d1ff
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---

# 审批工作

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

如果您被设置为批准者，您应定期查看等待批准的工作。

有关创建审批流程的信息，请参阅[为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)。

有关将审批与Workfront中的工作关联的信息，请参阅[将新的或现有的审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td> <p>审核或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问与审批关联的对象</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看与审批关联的对象的权限或更高的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

+++

## 在Adobe Workfront中查找批准

您可以在Workfront的各个区域查看和管理审批。

有关查看等待审批的项或您自己已提交审批的项的更多信息，请参阅[查看审批](../../review-and-approve-work/manage-approvals/view-approvals.md)。

## 批准主页区域的工作

1. 单击右上角的&#x200B;**[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png)，然后单击&#x200B;**[!UICONTROL 主页]**。
1. （视情况而定）单击&#x200B;**自定义**&#x200B;以添加&#x200B;**我的审批**&#x200B;小组件。
1. （视情况而定）单击&#x200B;**筛选器**&#x200B;下拉菜单，然后选择&#x200B;**全部**&#x200B;以查看分配给您的审批和委托给您的审批。

   >[!NOTE]
   >
   >分配给工作角色或组的审批不显示在主页中。 分配给团队的审批将显示在每个团队成员的“我的审批”小部件中。


1. 选择要在其中作出批准决策的项目。

   ![](assets/my-approvals-widget.png)

1. 在右侧面板中作出批准决策时，单击其中一个可用选项。 根据要批准的项目类型，以下选项将显示在页面的右上角：

   <table>
   <tr>
      <td>
      <p><strong>访问权限</strong></p>
      </td>
      <td>
      <p><strong>工作项</strong></p>
      </td>
      <td>
      <p><strong>文档</strong></p>
      </td>
      <td>
      <p><strong>校样</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>授权</li>
      <li>忽略</li>
      </ul>
      如果需要，您可以在<b>更改访问权限</b>下拉菜单中调整访问级别。
      </td>
      <td>
         <ul>
         <li>批准</li>
         <li>拒绝</li>
         </ul>
      您可以通过单击决策按钮中的下拉菜单来在决策中保留评论。
      </td>
      <td>
   已指定为审批者
         <ul>
         <li>批准</li>
         <li>批准（附加更改）</li>
         <li>需要工作</li>
         </ul>
   已分配为审阅者
         <ul>
         <li>完成我的审阅</li>
         </ul>
      此列中的选项仅适用于新文档审批。 旧文档审批与工作项审批显示相同。 
      </td>
      <td>
         <ul>
         <li>前往校对</li>
         </ul>
         您在验证查看器中做出决定。 有关审阅校样的信息，请参阅<a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">在Adobe Workfront中审阅校样</a>。
      </td>
   </tr>
   </table>

作出决定后，批准将从“我的批准”构件中删除。


## 直接批准项目、任务或问题中的工作

当项目、任务或问题正在等待审批时，您可以直接从项目、任务或问题批准或拒绝审批。 您还可以查看有关批准流程的详细信息。

要直接批准项目、任务或问题中的工作，请执行以下操作：

1. 转到需要您审批的项目、任务或问题。

   有关项目、任务或问题的当前审批流程的审批信息显示在项目的标题中。

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   以下批准信息可用：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td>项目、任务或问题的当前状态。 这是待审批项目的当前状态。 在批准流程中的每个阶段都获得批准后，状态才会被批准。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">审批阶段</td> 
      <td>审批流程的各个阶段。 <br>待批准的当前阶段显示为“待批准”。 已批准的阶段显示为已批准；尚未批准的阶段显示为未启动。</td> 
     </tr> 
    </tbody> 
   </table>

1. 根据您是要批准或拒绝批准流程，单击&#x200B;**批准**&#x200B;还是&#x200B;**拒绝**。\
   待审批的审批阶段现在已审批，审批流程将移至下一个阶段。 在所有阶段都获得批准后，状态即为“已批准”。

## 直接从文档审批文档

1. 转到文档区域，其中包含需要您审批的文档。
1. 选择文档，然后单击&#x200B;**批准**、**更改**&#x200B;或&#x200B;**拒绝**。\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. （可选）如果已为文档生成验证，则可以在验证界面中批准文档，如[从验证中批准文档](#approve-a-document-from-a-proof)中所述。

## 通过审批通知电子邮件审批文档

根据您的通知设置，您可能会收到电子邮件，通知您其他用户需要您做出批准决策的文档。 当您收到包含&#x200B;**作出批准决定**&#x200B;按钮的电子邮件时，可以直接从电子邮件启动批准流程：

1. 在电子邮件中，单击&#x200B;**作出批准决定**&#x200B;以打开验证的文档详细信息页面。
1. 执行以下任一操作以查看文档：

   * 查看有关文档的元数据。
   * 如果已创建用于审阅带标记和注释的文档的验证，请单击右上角附近的&#x200B;**打开验证** ![](assets/open-proof-icon-qs.png)并审阅该验证。

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     有关审阅校样的信息，请参阅[在Adobe Workfront中审阅校样](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)。

1. 单击右上角的&#x200B;**决策**&#x200B;选项以批准、审批并更改，或拒绝文档。

## 从验证审批文档 {#approve-a-document-from-a-proof}

您可以在验证查看器中批准文档。 有关详细信息，请参阅[在校对查看器中做出校对决定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)一文中的[在校对查看器中做出校对决定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。
