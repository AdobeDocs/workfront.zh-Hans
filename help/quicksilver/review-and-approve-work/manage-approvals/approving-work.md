---
product-area: projects
navigation-topic: approvals
title: 批准工作
description: 批准工作
author: Courtney
feature: Work Management
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# 批准工作

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

如果您被设置为审批者，则应定期审核等待审批的工作。

有关创建审批流程的信息，请参阅 [为工作项创建审批流程](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

有关将审批与Workfront中的工作关联的信息，请参阅 [将新审批流程或现有审批流程与工作关联](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

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
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看或更高权限访问与批准关联的对象</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看或更高对与批准关联的对象的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在Adobe Workfront中查找批准

您可以在Workfront的各个区域中查看和管理批准。

有关查看等待审批的项目或您已提交以供审批的项目的详细信息，请参阅 [查看批准](../../review-and-approve-work/manage-approvals/view-approvals.md).

## 从主页区域批准工作

1. 单击 **主页** 图标 ![](assets/home-icon-30x29.png) 在Adobe Workfront的左上角。

   >[!NOTE]
   >
   >您的Workfront管理员可以对环境中的主页图标进行以下更改：
   >
   >   
   >* 将其替换为自定义的图像，以说明您的组织。 在这种情况下，图标将与本文中显示的不同。
   >* 将链接到该页面的页面替换为其他页面。 在这种情况下，单击 **主菜单** ![](assets/main-menu-icon.png) ，然后单击 **主页**.


1. 单击 **过滤器** 下拉菜单。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 选择 **批准**.\
   显示所有需要您批准的工作项目。 

   >[!NOTE]
   >
   >分配给作业角色或组的批准不会显示在“主页”中。 分配给团队的审批将显示在工作列表的“团队请求”分组中。

1. （可选）按照文章中“按日期、项目或优先级分组和排序”一节的说明，更改显示批准的顺序 [在“主页”区域的“工作列表”中显示项目](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. 选择要作出审批决定的项目。

   ![](assets/task-approval-home-350x127.png)

1. 在右侧面板中做出批准决策时，单击其中一个可用选项。 根据您所批准的项目类型，页面的右上角会显示以下选项：

   * **项目：** 单击 **批准** 或 **拒绝**.

   * **任务：** 单击 **批准** 或 **拒绝** .

   * **问题：** 单击 **批准** 或 **拒绝** .

   * **工时单：** 单击 **批准** 或 **拒绝** .

   * **文档：** 单击 **批准**, **拒绝**&#x200B;或 **更改**.\
       查看批准时请考虑以下事项：

      * 当用户与您共享校样时，将在此处显示校样批准，如文章中“共享校样链接”一节中所述 [在Adobe Workfront中共享验证](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * 仅当您的Workfront环境与Workfront Proof Premium帐户集成时，校对批准才会显示在主页区域。 如果无法按此处所述使用校对，请与Workfront管理员联系。
      * 您会收到应用程序内通知，通知您校对批准。\
         有关应用程序内通知的更多信息，请参阅 [查看和管理应用程序内通知](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * 请求批准的用户的名称显示在“主页”区域的缩略图旁边，并带有以下文本：\
         &quot;*用户A* 想得到你的同意&quot;

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

         如果用户名不可用，则会显示以下文本：\
         &quot;校样的新版本已准备就绪，可供查看&quot;
      * 要对校样做出批准决定，请单击 **转到校样**，单击 **完成审阅**，然后单击其中一个可用选项。 批准校样时可用的选项包括： **已批准**, **已批准更改**, **所需更改**&#x200B;和 **不相关**.

      * 在对校样做出决策后，校样会保留在“我的批准”选项卡中，并带有文本“已做决策”，直到您单击 **刷新** 按钮，或者在刷新浏览器页面之前。

         有关查看校样的信息，请参阅 [在Adobe Workfront中审阅校样](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
   * **访问：** 在 **更改访问权限** 下拉菜单，然后单击 **授予访问权限**. 或者，单击 **忽略**.


## 直接从项目、任务或问题批准工作

当项目、任务或问题处于待批准状态时，您可以直接从项目、任务或问题中批准或拒绝批准。 您还可以查看有关审批流程的详细信息。

要直接从项目、任务或问题批准工作，请执行以下操作：

1. 转到需要您批准的项目、任务或问题。

   有关项目、任务或问题的当前审批流程的审批信息显示在项目标题中。

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   以下批准信息可供使用：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td>项目、任务或问题的当前状态。 这是待批准项目的当前状态。 批准流程中的每个阶段后，状态即被批准。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">批准阶段</td> 
      <td>审批流程的各个阶段。 <br>待批准的当前阶段显示为“待批准” 。 已批准的阶段将显示为已批准；尚未批准的阶段将显示为未开始。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **批准** 或 **拒绝**，具体取决于您是要批准还是拒绝批准流程。\
   待批准的批准阶段现已批准，并且批准流程将移至下一个阶段。 所有阶段都获得批准后，状态即被批准。

## 直接从文档批准文档 

1. 转到包含需要您批准的文档的文档区域。
1. 选择文档，然后单击 **批准**, **更改**&#x200B;或 **拒绝**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. （可选）如果已为文档生成校样，则可以在校样界面中批准文档，如 [通过校样批准文档](#approve-a-document-from-a-proof).

## 通过批准通知电子邮件批准文档

根据您的通知设置，您可能会收到电子邮件，通知您其他用户需要您做出批准决定的文档。 当您收到包含 **作出批准决定** 按钮，您可以直接从电子邮件启动批准流程：

1. 在电子邮件中，单击 **作出批准决定** 打开校样的文档详细信息页面。
1. 执行以下任一操作以审阅文档：

   * 查看有关文档的元数据。
   * 如果已创建校样以审阅带有标记和注释的文档，请单击 **打开校样** ![](assets/open-proof-icon-qs.png) 在右上角附近，查看校样。

      <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

      有关查看校样的信息，请参阅 [在Adobe Workfront中审阅校样](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. 单击 **决策** 用于批准、批准更改或拒绝文档的选项。

## 通过校样批准文档 {#approve-a-document-from-a-proof}

您可以在校对查看器中批准文档。 有关更多信息，请参阅 [在校对查看器中对校样做出决策](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) 在文章中 [在校对查看器中对校样做出决策](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
