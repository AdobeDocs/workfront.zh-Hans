---
title: 复制和提交请求
description: 复制和提交请求
author: Alina
draft: Probably
feature: Work Management
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '1309'
ht-degree: 2%

---

# 复制和提交请求

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is NWE only - hard code it in classic articles!)</p>
-->

频繁提交类似请求时，您可以复制现有提交的请求。 在这种情况下，您可以复制现有请求，对其进行最小的更改，然后作为新请求重新提交。

## 访问要求

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td> <p>请求或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>有权向请求队列添加请求</p> <p>查看现有请求的或更高权限</p> <p>有关设置请求队列的信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 先决条件

您必须要求您或您组织中以前提交的某个人能够复制并重新提交它。 如果请求属于其他人，则您必须至少拥有“查看”权限，才能复制请求并将其作为新请求提交。

## 有关复制请求并将其作为新请求提交的注意事项

* 您只能复制和提交已提交的请求。 您无法复制起草的请求。
* 您可以复制并提交您最初提交的请求，或者请求他人已提交并且您至少有权访问“查看”。
* 您始终有权复制和提交您自己的请求副本，除非有人删除了您对这些请求的权限。
* 当请求队列的创建者启用 **来自同一公司的人员将继承所有请求的相同权限** 在“队列详细信息”或“编辑项目”区域。 禁用此设置后，只允许原始请求者查看其自己的请求。

   有关更多信息，请参阅以下文章：

   * [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)

* 您可以在将原始请求重新提交为新请求之前，更新其副本。
* 如果在提交原始请求后发生以下更改，则无法再复制并重新提交请求：

   * 请求队列已删除。
   * 已删除队列主题。

      >[!TIP]
      >
      >如果队列主题是请求队列中的唯一主题，您仍然可以复制并提交请求，该请求将保存在请求队列本身下。

   * 请求队列不再作为帮助请求队列发布。 有关信息，请参阅 [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * 如果请求队列没有队列主题，并且原始请求是在2022年1月之前提交的。

   * 与请求队列关联的项目的状态不再为“当前”。

* 如果请求在转换过程中保留，则可以复制并提交已转换请求的副本。 有关更多信息，请参阅 [转换Adobe Workfront中的问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

   >[!TIP]
   >
   >复制的请求未链接到解析对象。

## 复制和提交请求

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **请求**.
1. （视情况而定）如果“已提交”部分默认不显示，请单击 **已提交** 中。
1. 找到要复制并作为新请求提交的请求，然后执行下列操作之一：

   * 选择它，然后单击 **复制并提交为新** 图标 ![](assets/copy-and-submit-as-new-requests-area-nwe.png) 位于已提交请求列表的左上角。
   * 单击 **更多** 菜单 ![](assets/more-icon.png) 在请求名称的右侧，单击 **复制并提交为新**

      或

      右键单击选定的请求，然后单击 **复制并提交为新**.

      ![](assets/request-selected-more-menu-options-nwe-350x191.png)

      >[!TIP]
      >
      >如果您无权创建问题，则会收到一条警告，指出管理员限制您创建请求。

1. （可选）根据需要更新以下信息：

   * **请求类型**:保存复制请求的请求队列。 默认情况下，复制的请求会保存到原始请求的请求队列。
   * **主题组** 和 **队列主题**，如果已选择它们。 可以为您的环境自定义名称或主题组以及队列主题。 默认情况下，复制的请求会保存到原始请求的主题组和队列主题中。

      >[!TIP]
      >
      >如果路径从原始请求的路径发生更改，则请求队列的创建者修改了队列。

1. （可选）更新复制的请求中的任何信息。 根据请求队列创建者在 **新问题字段** 部分 **队列详细信息** 在项目上，您可能会找到以下任一字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>主题</strong> </td> 
      <td>显示原始请求的名称。 如有必要，请更新。 否则，Workfront会将复制的请求命名为 <b>副本 &lt;name of="" original="" request=""&gt;</b>. 这是必填字段。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>描述</strong> </td> 
      <td>显示原始请求的描述。 如有必要，请更新。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>显示原始请求的URL。 如有必要，请更新。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>优先级</strong> </td> 
      <td> <p>指定请求的优先级。 优先级应定义您认为此请求应解决的速度。 默认选项为：</p> 
       <ul> 
        <li>无</li> 
        <li>低</li> 
        <li>正常</li> 
        <li>高</li> 
        <li>紧急</li> 
       </ul> <p>您的Workfront管理员可以修改优先级的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>严重程度</strong> </td> 
      <td> <p>指定请求的严重性。 严重性应定义此请求对您的工作造成的影响，以防其及时得到解决。 默认选项为：</p> 
       <ul> 
        <li>轻微</li> 
        <li>导致混淆</li> 
        <li>有变通方案的问题</li> 
        <li>没有变通方案的问题</li> 
        <li>致命错误</li> 
       </ul> <p>您的Workfront管理员可以修改严重性的名称。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>主要联系人</strong> </td> 
      <td>请求的主要联系人默认为您，因为您是解决与请求相关的任何问题的指点人员。 但是，您可以将其更改为任何其他Workfront用户。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>分配</strong></span> </td> 
      <td> <p>指示应将请求分配给的活动用户、作业角色或团队的名称。 </p> <p> 您可以指定多个用户、作业角色或团队。 </p> <p>根据请求队列的设置方式，您可能只能将请求分配给一种或两种类型的资源，而不是全部三种资源。 </p> <p>我们建议对您的请求队列使用路由规则，以便它们能够被自动路由到相应的资源。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">根据请求队列的设置方式，您可能只能向请求分配一种类型的资源（例如，用户）。 如果路由规则也与请求队列相关联，并且它自动将请求路由到不同类型的资源（例如，团队），则您的请求将分配给您在提交请求时手动指定的实体（用户）和路由规则中指定的资源（团队）。</p> <p style="font-weight: normal;">有关更多信息，请参阅以下文章：</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">创建路由规则</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划小时</strong> </td> 
      <td> <p>估计完成此请求需要多少小时。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划开始日期</strong> </td> 
      <td> <p>应开始处理此请求的日期。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>计划完成日期</strong> </td> 
      <td>您希望解决此请求的日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>状态</strong> </td> 
      <td>新请求的默认状态为“新”。 您的Workfront管理员可能已更改此状态的名称。 您还可以从此下拉菜单中将状态更改为其他内容。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>文档</strong> </td> 
      <td> <p>向请求中添加文档。 附加到原始请求的文档不会转移到复制的请求。</p> <p><b>笔尖</b>

   根据请求队列的设置方式，“文档”部分可能显示在自定义字段之前或之后。</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. （可选）根据需要更新附加的自定义表单中的任何信息。

   >[!TIP]
   >
   >* 附加到原始请求的所有自定义表单以及自定义字段中包含的值都会传输到复制的请求。 这包括包含逻辑的字段。
   >* 您无法从复制的请求中删除自定义表单。


1. 单击 **提交**.

   复制的请求将作为您指定的请求队列中的新请求提交。
