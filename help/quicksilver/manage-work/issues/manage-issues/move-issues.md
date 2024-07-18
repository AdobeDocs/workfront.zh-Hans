---
product-area: projects
navigation-topic: manage-issues
title: 移动问题
description: 您可以在项目和任务之间移动问题。
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
source-git-commit: 6c82c585376b41cff0e57b253b6a214fb00309de
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 1%

---

# 移动问题

您可以在以下对象之间移动问题：

* 从项目到另一个项目
* 从任务到同一项目或其他项目中的另一个任务
* 从任务到项目或到另一个项目
* 从项目到同一项目中的任务或其他项目中的任务

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
   <td> <p>请求或更高版本</p> <p>查看或更高许可证以移动项目问题分区中的问题。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p>查看或更高权限的项目和任务</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>。 有关Workfront管理员如何更改访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理问题的权限</p> <p>Contribute对要将问题移动到的项目的权限，以及添加问题的功能。</p> <p> 有关向问题授予权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a></p> <p>有关请求其他权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 有关移动问题的注意事项

移动包含文档或与请求队列关联的问题时，请考虑以下事项：

* **当问题与请求队列关联时：**&#x200B;当您将问题移动到另一个对象并且该问题与请求队列关联时，移动的问题不再与第一个问题源自的原始队列关联。
* **当文档附加到问题时：**&#x200B;当您将问题移动到另一个对象并且该问题具有附加的文档时，该文档、其版本和验证也移动到新问题。 与文档关联的任何审批都不会移动。
* **当问题链接到文档或文件夹时：**&#x200B;当您移动具有链接到Google Drive等第三方服务的文档或文件夹的问题时，指向文档的链接将随问题一起移动。

## 在列表中移动问题

您可以从问题列表或问题报告中移动一个或多个问题。

1. 转到包含要移动的一个或多个问题的项目。

   或

   转到问题报告。

1. 如果您选择转到项目，请单击左侧面板中的&#x200B;**问题**。
1. 选择要移动的一个或多个问题，然后单击问题列表顶部的&#x200B;**更多菜单**，然后单击&#x200B;**移至**。

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. 继续移动问题，如从步骤2开始的[移动单个问题](#move-a-single-issue)部分中所述。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## 移动单个问题 {#move-a-single-issue}

您可以在查看时移动一个问题。

### 在预览环境中移动单个问题

1. 转到要复制的问题，单击问题名称右侧的&#x200B;**更多**&#x200B;菜单![](assets/more-icon.png)，然后选择&#x200B;**移动**。

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   显示&#x200B;**移动问题**&#x200B;框。

   ![](assets/move-issue-box-nwe-350x280.png)

1. 在&#x200B;**选择目标项目**&#x200B;部分中，指定要将问题移动到的项目的名称。 默认显示当前项目的名称。

   >[!TIP]
   >
   >列表中仅显示100个项目。

1. （视情况而定）如果您无权将问题移动到项目，请单击&#x200B;**请求访问权限**。
1. （视情况而定）如果您有权将问题添加到目标项目上的任务之一，请继续移动选定目标项目上的问题而不请求访问权限。

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >如果所选项目处于未决批准、已完成或终止状态，且Workfront管理员阻止向这些项目添加问题，则会显示类似消息。 有关详细信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

1. （可选）在&#x200B;**选项**&#x200B;部分中，取消选择下表中列出的任何项，以将其从移动的问题中删除。 默认情况下，将选择所有选项。

   >[!IMPORTANT]
   >
   >取消选择“选项”列表中的项目会导致数据丢失。 来自现有问题的信息将被删除并且无法恢复。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">全部选择</td> 
      <td>取消选择此选项可在将问题移动到新位置时，从问题中删除所有信息。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">分配</td> 
      <td>删除分配给问题的用户、工作角色或团队。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">进度</td> 
      <td>删除问题的完成百分比（如果有）。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>文档</p></td> 
      <td> <p>删除文档选项卡中的所有内容，包括文档版本、链接的文档和文件夹。

   <b>注释</b>

   如果您选择不移动存在此问题的文档，这些文档将被删除并放入回收站30天。 管理员可以恢复它们，它们将在移动的问题上恢复。

   如果问题在移动之后被删除，则恢复的文档将放置在恢复这些文档的管理员用户页面的“文档”区域中。
   <br> </p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">权限</td> 
      <td>删除与问题共享的实体。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">更新</td> 
      <td>从问题的更新部分删除注释。</td> 
     </tr> 
    </tbody> 
   </table>


1. （可选）在&#x200B;**选择任务**&#x200B;部分中，选择要将问题移动到的任务。
1. 单击&#x200B;**移动问题**&#x200B;或&#x200B;**移动问题**（如果您在列表中选择了多个问题）。

   移动的问题将添加到指定项目。




