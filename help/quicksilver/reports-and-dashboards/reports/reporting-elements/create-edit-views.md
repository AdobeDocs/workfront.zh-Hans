---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中创建或编辑视图
description: 您可以使用视图自定义您在屏幕上显示的信息类型。 您可以在Adobe Workfront中使用多种类型的视图。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# 在Adobe Workfront中创建或编辑视图

您可以使用视图自定义您在屏幕上显示的信息类型。 您可以在Adobe Workfront中使用多种类型的视图。

本文介绍了如何为列表和报表创建和编辑标准视图，以及如何创建敏捷视图。 有关更多信息，请参阅 [视图Adobe Workfront概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront计划*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront许可证*</strong></td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>编辑对过滤器、视图、分组的访问权限</p> <p>编辑对报表、功能板、日历的访问权限，以在报表中创建视图</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>管理报表的权限以创建或编辑报表中的视图</p> <p>管理要编辑的视图的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 创建或自定义视图

创建或自定义视图的过程因创建或自定义标准视图还是敏捷视图而异。

* [创建或自定义标准视图](#create-or-customize-a-standard-view)
* [创建或自定义敏捷视图](#create-or-customize-an-agile-view)

### 创建或自定义标准视图 {#create-or-customize-a-standard-view}

您可以创建新的标准视图，也可以自定义您之前创建的现有标准视图。

1. 单击 **查看** 要在其中创建或自定义视图的任何列表上的下拉菜单。
1. （可选）要自定义现有视图，请选择要自定义的标准视图。\
   在Workfront中，任何类型的列表（如报表、项目列表或任务列表）上都提供标准视图。
1. 单击 **查看** 下拉菜单，然后单击 **自定义视图** 或 **新建视图**.\
   的 **自定义视图** 对话框。

1. 在 **列预览** ，请执行以下任一操作：

   * 单击列标题，然后选择新字段，可修改任意列的值。
   * 通过单击 **添加列**，开始键入要添加的列的名称，然后在下拉列表中显示时单击该列。
   * 通过将列标题拖动到新位置来调整列的显示顺序。

      * （可选）在 **列设置** 区域，单击 **按以下方式汇总此列** 下拉列表中，然后选择用于汇总信息的可用选项之一。 选择此选项时，列中的信息会按报表的分组进行汇总。\
         对于日期字段，您可以按以下选项汇总值：

         * 最大
         * 最小

         对于数字和货币字段，您可以按以下选项汇总值：

         * 计数
         * Sum
         * 平均
         * 最大
         * 最小

         >[!NOTE]
         >
         >在分组中聚合以下字段的值时，父对象（例如，父任务）会出现以下例外：
         >   
         >   * 除“实际工时”(例如“计划/实际人工成本”、“计划/实际费用成本”、“计划/实际成本”、“计划/实际工时”之外的所有“数字”和“币种”字段仅汇总子任务和独立任务的值。 它们不会聚合父任务或父代父代的值。
         >   * 实际小时数汇总主要父任务和独立任务的值；它们不会聚合父任务或子任务的父任务的数字。
         >   * 数字和货币值的自定义数据字段聚合所有任务：父母、子女、父母的父母和独立任务。


         有关在报表中使用分组的更多信息，请参阅文章 [Adobe Workfront中的分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * （可选）单击 **高级选项** 要为列指定以下信息，请执行以下操作：

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>自定义列标签</strong></td> 
           <td><p>为列指定自定义标签。 此标签将替换默认标签。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>字段格式</strong></td> 
           <td>选择您希望在列中显示字段值的格式。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>在仪表板上显示此列</strong></td> 
           <td><p>当报表与其他报表并排显示时，选择此选项可在功能板上显示此列。 取消选择此选项时，在报表并排显示的功能板上查看报表时，不会显示此列。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>列规则</strong></td> 
           <td><p>单击 <strong>为此列添加规则</strong> 为列定义规则。 添加规则后，您可以定义字段和文本样式，以了解匹配该规则的字段的显示方式。 单击 <strong>添加规则</strong> 完成规则的定义后，您才会再次访问。</p></td> 
          </tr> 
         </tbody> 
        </table>

         有关有条件地设置报表中视图格式的详细信息，请参阅文章 [在文本模式中使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. （视情况而定）如果您单击 **高级选项**，单击 **完成**.

1. 单击 **保存视图** 创建新视图或将当前视图替换为您所做的更改。\
   或\
   单击 **另存为新视图** 将更改另存为新视图。

   >[!TIP]
   >
   >的 **另存为新视图** 是自定义内置Workfront视图时唯一可用的选项。

   您的访问权限指示视图的保存方式。 如果最初创建了视图，则可以保存更改；否则，系统会提示您保存版本。 请记住，您对视图所做的更改会影响已与其共享视图的用户。

### 创建或自定义敏捷视图 {#create-or-customize-an-agile-view}

您可以创建新的敏捷视图，或自定义您之前创建的现有敏捷视图。

>[!IMPORTANT]
>
>敏捷视图仅在查看项目时可用。

有关Agile视图的更多信息，请参阅文章 [在敏捷视图中管理项目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

要创建或自定义敏捷视图，请执行以下操作：

1. 转到项目中的任务列表。
1. 单击 **敏捷情节提要** 图标 ![](assets/agile-storyboard-nwe.png).

1. （视情况而定）要自定义现有的敏捷视图：

   1. 单击 **查看** 下拉菜单，然后选择要自定义的敏捷视图。\
      您无法自定义默认的Agile视图。

   1. 单击 **查看** 下拉菜单，然后单击 **自定义视图**.\
      ![](assets/view-agile-customize.png)

1. （视情况而定）要创建新的Agile视图，请单击 **新建视图**.\
   的 **自定义敏捷视图** 对话框。

1. 在 **自定义敏捷视图** 对话框中，为Agile视图指定名称。\
   我们建议您在视图名称中包含“Agile”一词，以便用户知道这是一个Agile视图。\
   此名称显示在 **查看** 下拉菜单。

1. 定义要在敏捷视图的文章展示板上显示的状态列。 这些是Workfront管理员定义的任务状态，如 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   只有系统状态才可在Agile文章展示板上使用。 如果状态仅适用于您所属的单个组，则该状态在敏捷文章展示板上不可用。 此外，在Agile视图中查看项目时，状态为仅对自定义组可用的任务不可见。

   用户可以在敏捷文章展示板上的这些状态列之间移动文章。\
   在定义状态列时，您可以执行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>重新排序状态列：</strong> </td> 
      <td> 将状态列拖动到您希望它显示的顺序。<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>删除状态列：</strong> </td> 
      <td>单击要删除的列上的(x)图标。<br>除非已将自定义状态添加到视图，且自定义状态等于“新建”，否则您无法删除“新建”状态。<br>有关创建自定义状态的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>添加状态列：</strong> </td> 
      <td> <p>单击 <strong>加号</strong> 图标，然后选择要添加的状态。<br>将显示所有默认系统状态，以及与您共享的任何自定义状态。<br>您最多可以配置10个状态来显示。</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. 在 **将卡片颜色与** ，请从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>叙述:</strong> </td> 
      <td>任何子任务都与父任务的颜色相匹配，因此任何给定泳道中所有文章的颜色都相同。<br>如果任务没有子任务或没有父任务，则在创建任务时，会随机为任务分配颜色。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自由表单:</strong> </td> 
      <td> 默认情况下，所有卡片都显示为蓝色，直到用户手动更改颜色为止，如文章中所述 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">按颜色在Scrum展示板上对文章进行分类</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>优先级:</strong> </td> 
      <td> <p> 颜色与文章优先级相关联，如下所示：</p> 
       <ul> 
        <li>高=红色</li> 
        <li>中=黄色</li> 
        <li>低=绿色<br>如果您的Workfront管理员为Workfront系统配置了自定义优先级，则最高优先级为红色，第二高优先级为黄色，其余为绿色。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>任务所有者:</strong> </td> 
      <td> 具有相同主要代理人的所有文章颜色相同。<br>主被分派人是最先分配给任务的用户。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **敏捷** 部分，在 **其他字段** 区域，单击 **添加字段**，然后选择要添加到文章卡片的字段。 （创建自定义视图或为报表创建列时，您可以添加这些字段。）\
   重复此过程，在文章卡片中添加最多三个其他字段。\
   在向文章卡片中添加字段时，字段是仅供查看的，并且仅在填充字段时才显示。

   默认情况下，文章卡片上会显示以下类型的数据：

   * 文章名称，带有直接指向任务的链接
   * 带有直接指向项目的链接的项目名称\
      仅当对迭代使用敏捷视图时，才会显示此链接；在项目上使用敏捷视图时，不会显示该视图。
   * 任务描述
   * 当前承诺
   * 通过调整完成百分比本身或通过调整完成的点数或小时数，查看和编辑完成百分比
   * 已分配的用户

   您可以在文章卡片上显示其他数据（包括自定义数据）。 出于任何原因，您可能希望在文章卡片上显示其他字段。 例如，如果您正在为项目中的多个客户处理文章，或者您可能希望显示任务开始日期，则可能希望显示客户ID。

1. 单击&#x200B;**保存**。\
   您的访问权限指示视图的保存方式。 如果最初创建了视图，则可以保存更改；否则，系统会提示您保存版本。 请记住，您对视图所做的更改会影响已与其共享视图的用户。

1. （可选）单击 **列表视图** 图标 ![](assets/list-view-in-agile-view-for-tasks.png) 返回任务列表。
