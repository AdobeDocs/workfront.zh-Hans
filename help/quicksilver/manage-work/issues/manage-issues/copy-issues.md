---
product-area: projects
navigation-topic: manage-issues
title: 复制问题
description: 您可以复制问题或请求，并将其保存在同一或其他项目上。 您还可以将问题从任务复制到其他项目。
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# 复制问题

您可以复制问题或请求，并将其保存在同一或其他项目上。 您还可以将问题从任务复制到其他项目。

您可以从以下对象复制问题：

* 从一个项目到同一个项目（在同一个项目中复制）
* 从任务到同一任务（如果在同一任务上，则重复）
* 从项目到其他项目
* 从任务到项目

>[!TIP]
>
>“问题”和“请求”在Workfront中可互换使用。 您可以记录项目和任务中的问题，以指明需要解决的未预见工作。 您还可以提交被记录为指定为请求队列的项目问题的请求。

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
   <td> <p>请求或更高版本</p> <p>复制项目“问题”部分中的问题的审阅或更高许可证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限访问项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>对要将问题复制到的项目具有“添加问题”功能的参与权限。</p> <p> 有关授予问题权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 与文档或请求队列相关的问题的注意事项

在复制包含文档或与请求队列关联的问题时，请考虑以下事项：

* **当问题与请求队列关联时：** 将问题复制到另一个对象时，如果问题与请求队列相关联，则复制的问题不再与第一个问题源自的原始队列相关联。
* **将文档附加到问题时：** 当将问题复制到另一个对象并且该问题附加了文档时，文档及其版本也将移至新问题。 与文档关联的任何校样或批准都不会移动。
* **将问题链接到文档或文件夹时：** 在复制包含文档或文件夹的问题时，如果该文档或文件夹已链接到第三方服务(如Google Drive)，则指向文档的链接将转移到复制的问题。 

## 复制列表中的问题

您可以从问题列表或问题报表中复制一个或多个问题。

1. 转到包含要复制的问题的项目。

   或

   转到问题报表。

1. 如果您选择转到项目，请单击 **问题** 中。
1. 选择要复制的问题，然后单击 **“更多”菜单** 在问题列表顶部，单击 **复制到**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. 继续复制问题，如一节中所述 [复制单个问题](#copy-a-single-issue) 从步骤2开始。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:&nbsp;ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## 复制单个问题 {#copy-a-single-issue}

您可以在查看问题时复制一个问题。

1. 转到要复制的问题，然后单击 **更多** 菜单 ![](assets/more-icon.png) 在问题名称的右侧， **复制** 。

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   的 **复制问题** 框中。

   ![](assets/copy-issue-box-nwe-350x285.png)

1. 在 **选择目标项目** 部分，指定要将问题复制到的项目名称。 默认情况下，将显示当前项目的名称。

   >[!TIP]
   >
   >列表中仅显示100个项目。

1. （视情况而定）单击 **请求访问** 如果您无权将问题复制到项目。
1. （视情况而定）如果您有权向目标项目中的任务之一添加问题，请继续将问题复制到选定的目标项目，而无需请求访问权限。

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >如果选定的项目处于待批准、已完成或已停止状态，则当Workfront管理员阻止向这些项目添加问题时，会显示类似的消息。 有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. （可选）在 **选项** 部分，取消选择下表中列出的任何项目，以将其从新问题中删除。 默认情况下，将选择所有选项。

   >[!NOTE]
   这仅影响复制的问题，而不影响原始问题。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">分配</td> 
      <td>删除分配给问题的用户、作业角色或团队。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>删除问题的完成百分比（如果有）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">文档</td> 
      <td><span style="line-height: 1.5;">删除“文档”选项卡中的所有内容，包括文档版本、链接的文档和文件夹。</span> <br>默认情况下，文档校样和批准无法复制到另一个问题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td>删除与其共享问题的实体。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>从问题的“更新”部分删除注释。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">自定义数据</td> 
      <td>从有关问题的自定义表单中删除信息，以及与与问题附加的文档关联的自定义表单上的信息（如果这些信息也与问题一起复制）。 自定义表单将保留在问题和文档中，但有关表单的信息将不会传递到新问题中。 </td> 
     </tr> 
    </tbody> 
   </table>

1. （可选）在 **选择任务** 部分，选择要移动问题的任务。
1. 单击 **复制问题** 或 **复制问题** 如果您在列表中选择了多个问题。

   复制的问题将添加到指定的项目中。

 
