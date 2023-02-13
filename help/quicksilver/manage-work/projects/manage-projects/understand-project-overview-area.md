---
content-type: overview
product-area: projects
navigation-topic: manage-projects
title: 在项目概述区域中管理信息
description: 在项目概述区域中管理信息
author: Alina
feature: Work Management
exl-id: 6113bc62-18f2-4558-bc2f-986b1e7d1a83
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 4%

---

# 在项目概述区域中管理信息

<!--
<p>(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

您可以通过访问“项目详细信息”部分的“概述”区域来查看或编辑项目信息。 在此区域中，可以查看或编辑的字段数量有限。 有关编辑项目所有信息的信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td role="rowheader"> <p role="rowheader">Adobe Workfront许可证*</p> </td> 
   <td> <p>审阅或更高版本</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>查看对项目或更高版本的访问权限</p> <p>如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看项目或更高级别的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 访问概述部分

1. 转到要查看其概述部分的项目。
1. 单击 **项目详细信息** 中。
1. 的 **概述** 部分应首先作为项目详细信息的一部分显示，并且默认应该展开

   或

   单击 **编辑** 图标 ![](assets/edit-icon.png) 在“详细信息”部分的右上角，单击 **概述**. 此时将打开概述区域进行编辑。

   >[!NOTE]
   >
   >根据Workfront管理员配置布局模板的方式，概述部分可能不会最先列出，在这种情况下，该部分会折叠。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. （视情况而定）如果某个项目中有一个特定字段需要更新，但该字段未显示在此部分中，请单击 **“更多”菜单** ![](assets/more-icon.png) 项目名称旁边，然后 **编辑** 查看更多项目字段。

   有关编辑项目的更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

1. 编辑或查看下表中显示在 **概述** 中。\
   要编辑任何可编辑的字段，请单击该字段，或单击 **+添加** 向空字段添加信息。

   >[!NOTE]
   >
   >根据Workfront管理员配置布局模板的方式，可能不会显示所有字段。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader"><b>字段</b></td> 
      <td><b>描述</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader">描述</td> 
      <td>描述此项目的用途。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td>在此字段中插入任何URL。 它可以是Workfront URL或任何其他URL。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">优先级</td> 
      <td>用作项目的指定优先级或重要性。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td> <p>项目状态。 </p> <p>提示：除非所有任务和问题都已完成，否则无法完成项目。 如果将“项目”的“完成模式”设置为“自动”，则无法手动完成项目。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">条件类型</td> 
      <td>确定管理器是设置项目的条件，还是设置了Workfront。 有关“项目条件”的信息，请参阅文章 <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">项目条件和条件类型概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">时间表模式</td> 
      <td>设置项目的计划方式。 例如，项目是从开始日期还是从完成日期开始计划。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划开始日期和时间</td> 
      <td> 项目计划启动时。 当项目计划从开始日期开始时，项目经理会手动设置此设置。 Workfront会根据项目中任务的持续时间，在项目从完成日期开始计划时自动设置此日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划完成日期和时间</td> 
      <td> 项目计划完成时。 当项目计划从完成日期开始时，项目经理会手动设置此设置。 Workfront会根据项目中任务的持续时间，在项目从开始日期开始计划时自动设置此日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">项目组合</td> 
      <td>与项目关联的项目组合。 必须先创建项目组合，然后才能将其添加到项目中。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">项目群</td> 
      <td>与项目组合关联的项目。 必须先创建项目，然后才能将其添加到项目中。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">组</td> 
      <td> <p>与项目关联的组。</p> <p>您可以通过将鼠标悬停在正确的组上并单击信息图标来确保选择正确的组 <img src="assets/info-icon.png"> 显示在其旁边的。 此时会显示工具提示，其中列出了有关群组的信息，例如群组上的群组层次结构及其管理员。</p> <p> <img src="assets/group-details-widget-350x351.png" style="width: 350;height: 351;"> </p> 
      默认情况下，除非您指定其他组，否则在创建项目时，以下组之一会自动与项目关联：
        <ul> 
         <li> <p><span>从“项目”区域创建项目时，项目创建者的“主页组”会与项目关联。</span> </p> </li> 
         <li> <p><span>从“设置”区域的组主页创建项目时，该组会自动与项目关联。</span> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">公司</td> 
      <td>与项目关联的公司。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">项目所有者 </td> 
      <td>这是项目的所有者。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">项目赞助者</td> 
      <td> <p>这是项目的主要利益相关方。 这通常是监督和支持项目的高管，或者是预算责任人。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">资源管理器</td> 
      <td> <p>这是可以管理项目中用户资源的人员。 </p> <p>有关资源管理器的信息，请参阅文章 <a href="../../../manage-work/projects/planning-a-project/designate-resource-managers-for-projects-and-templates.md" class="MCXref xref">为项目或模板指定资源管理器 </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >在更新“项目所有者”、“项目赞助商”和“资源管理器”字段时，请注意头像、用户的主要角色或其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。


1. 查看概述部分中的以下字段。 您无法编辑以下字段：

   | 字段 | 描述 |
   |---|---|
   | 参考号 | 这是一个自动生成的字段，它始终为每个项目提供唯一值。 |
   | 预计开始日期 | 这是基于已完成的工作和剩余工作开始工作的“实时”日期。 |
   | 预计完成日期 | 这是一个“实时”日期，根据已完成任务的进度和对“新”或“正在进行”状态任务的进度更新，完成项目的时间。 |
   | 计划小时 | 项目计划的小时数。 这些小时是每个任务的总计划小时数。 |
   | 实际小时数 | 项目登录的小时数。 这些小时是项目、任务或项目问题上记录的总小时数。 |
   | 计划持续时间 | 项目将跨度的时间，基于任务的最早计划起始日期与项目任务的最新计划完成日期之间的时间范围。 |
   | 实际持续时间 | 项目实际跨度的时间，基于任务的最早实际开始日期与项目上任务的最新实际完成日期之间的时间范围。 |
   | 输入日期 | 项目创建的日期和时间。 |
   | 输入者 | 创建项目的用户的名称。 |
   | 上次更新日期 | 上次更新项目的日期和时间。 |
   | 上次更新者 | 上次更新项目的用户的名称。 |
   | 模板 |   |


1. 如果您的公司为Adobe Workfront方案计划员购买了附加许可证，并且项目已通过链接的方案发布信息，则在“方案计划员”区域中查看以下方案信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><b>字段</b></td> 
      <td><b>描述</b> </td> 
     </tr>
     <tr> 
      <td role="rowheader"><span>计划持续时间</span> </td> 
      <td><span>将项目链接到方案时相应方案的持续时间。 此字段不可编辑。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>上次发布日期</span> </td> 
      <td><span>上次根据相应方案发布项目的日期。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>计划开始日期</span> </td> 
      <td><span>在计划开始月份的第一天，即项目与计划链接。</span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>计划结束日期</span> </td> 
      <td><span>该项目与某个项目链接的计划结束月份的最后一天。 </span> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>FTE和小时中的主动作业角色</span> </td> 
      <td> <p>有关相关职务角色及其为计划分配的时间的信息。 这包括：</p> 
       <ul> 
        <li>作业角色名称</li> 
        <li>FTE数</li> 
        <li> <p>所有FTE的小时数</p> <p>您可以使用小时数或FTE估算计划或方案所需的工作角色数量。 </p> <p>有关更多信息，请参阅 <a href="../../../scenario-planner/create-and-edit-plans.md" class="MCXref xref">在方案计划员中创建和编辑计划</a>. </p> </li> 
       </ul> <p>提示： <span>如果方案中每个月的职务角色数量不同，则此字段显示方案所需的最大角色数量。 例如，如果您需要1名顾问（1月）和2月（2月），列将显示2FTE以及所有月份2个FTE的相应小时数。</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关将项目与计划关联的信息，请参阅 [通过在方案规划器中发布方案来更新或创建项目](../../../scenario-planner/publish-scenarios-update-projects.md).

1. 单击 **保存更改**.
