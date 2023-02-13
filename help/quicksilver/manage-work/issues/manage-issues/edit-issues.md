---
product-area: projects
navigation-topic: manage-issues
title: 编辑问题
description: 您可以编辑有关您创建的问题的信息，或者其他用户在与您共享问题时创建的信息。
author: Alina
feature: Work Management
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 3f5e5e9832fc33d39ea5dfbbc513b80adbf113f5
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 3%

---

# 编辑问题

您可以编辑有关您创建的问题的信息，或者其他用户在与您共享问题时创建的信息。

您可以编辑单个问题，也可以在列表中编辑问题。 有关编辑列表中问题的信息，请参阅 [编辑列表中的问题](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求或更高版本</p> <p>在任务或项目的“问题”部分中查看或更高许可证以编辑问题</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别*</td> 
   <td> <p>编辑对问题的访问权限</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关访问访问级别中问题的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">授予对问题的访问权限</a>. 有关Workfront管理员如何更改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>在“问题详细信息”区域，为问题提供编辑权限 </p> <p>在“编辑问题”框中管理问题的权限以对其进行编辑</p> <p> 有关授予问题权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题 </a></p> <p>有关请求其他权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 编辑问题时的限制

有一些限制可能会阻止您编辑问题。

* 您无法编辑审批流程中的问题。 您只能记录时间或更新处于“待批准”状态的问题的状态。
* 仅当您的Workfront管理员或组管理员在“项目首选项”区域中启用此功能时，您才能编辑文档，并将文档添加到项目上状态为“完成”、“无效”或“待批准”的问题。 有关设置项目首选项的信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## 编辑单个问题

您可以使用“编辑问题”或“问题详细信息”区域编辑问题。 以下步骤介绍了如何在“编辑”问题框中编辑问题。

1. 转到 **主菜单**.
1. 单击 **项目**，然后单击项目名称以打开项目。
1. （可选）单击 **任务** ，然后单击任务的名称以打开该任务。
1. 单击 **问题** 中。

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. （可选）要编辑有关问题的有限信息，请单击 **问题详细信息** 中。

   ![](assets/qs-issue-details-icon-highlighted-and-expanded-on-issue-350x206.png)

   >[!NOTE]
   >
   >根据Workfront管理员或组管理员修改布局模板的方式，“问题详细信息”区域中的字段可能会重新排列或不显示。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   要编辑详细信息部分中的信息，请执行以下操作：

   1. （可选）单击 **全部折叠** 图标来折叠所有区域。
   1. （可选和视情况而定）折叠区域后，单击 **向右箭头** ![](assets/right-pointing-arrow.png) 展开要编辑的区域。
   1. （可选）要附加自定义表单，请在 **添加自定义表单** 字段，然后在列表中显示时将其选中，然后单击 **保存更改**.
   1. （可选）单击 **导出** 图标 ![](assets/export.png) 要将概述和自定义表单信息导出到PDF文件，请单击 **导出**. 从以下选项中进行选择：

      * 全选（仅当至少附加了一个自定义表单时才显示）
      * 概述
      * 一个或多个自定义表单的名称

      PDF文件将下载到您的计算机。

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      有关更多信息，请参阅 [导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).
   有关“问题详细信息”部分中显示的字段的信息，请继续编辑“编辑问题”框中的问题，如下所述。

1. 要编辑与问题有关的所有信息，请在列表中选择问题，然后单击 **编辑** 列表顶部

   或

   单击列表中问题的名称，然后单击 **更多** 菜单，然后 **编辑。**

   的 **编辑问题** 对话框。

   >[!IMPORTANT]
   >
   >您必须拥有问题的“管理”权限，才能查看“编辑”链接。

   所有问题字段在“编辑问题”框中均可用，并按左侧面板中列出的区域进行分组。

1. 请考虑在以下任一部分中指定信息：

   * [问题名称](#issue-name)
   * [概述](#overview)
   * [分配](#assignments)
   * [自定义表单](#Custom%C2%A0F)
   * [设置](#settings)

   >[!NOTE]
   >
   >根据Workfront管理员设置布局模板的方式，“编辑问题”框中的字段在您的环境中可能会有所不同。 有关信息，请参阅 [使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

### 问题名称 {#issue-name}

1. 按如上所述开始编辑问题。
1. 单击 **问题名称**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. 更新 **问题名称** 字段。
1. 单击 **保存** 或继续编辑以下部分。

### 概述 {#overview}

1. 按如上所述开始编辑问题。
1. 单击 **概述**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. 更新或查看下表中的任意字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td> <p>添加有关该问题的其他信息。</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">基本信息部分</td> 
     </tr> 
     <tr> 
      <td role="rowheader">状态</td> 
      <td> <p>选择问题的状态。 有关问题状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态列表</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">优先级</td> 
      <td> <p>这是一个可视标记，用于确定问题的优先级。</p> <p>从以下选项中进行选择：</p> 
       <ul> 
        <li> <p><strong>无</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p><strong>正常</strong> </p> </li> 
        <li> <p><strong>高</strong> </p> </li> 
        <li> <p><strong>紧急</strong> </p> </li> 
       </ul> <p>根据Workfront管理员选择的项目首选项，优先级名称可能会因您而异。 有关编辑优先级的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">创建和自定义优先级</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">严重程度</td> 
      <td> <p>这是一个可视标记，用于指示问题中描述的问题的严重程度。 严重性是特定于问题的。 从以下选项中进行选择：</p> 
       <ul> 
        <li> <p style="font-weight: bold;">轻微</p> </li> 
        <li> <p style="font-weight: bold;">导致混淆</p> </li> 
        <li> <p style="font-weight: bold;">有变通方案的问题</p> </li> 
        <li> <p style="font-weight: bold;">没有变通方案的问题</p> </li> 
        <li> <p style="font-weight: bold;">致命错误</p> </li> 
       </ul> <p>根据Workfront管理员选择的项目首选项，严重性的名称可能会因您而异。 有关编辑严重性的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">创建或自定义问题严重性</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>键入与问题相关的Web链接。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">类型</td> 
      <td> <p>根据项目经理在项目的“队列详细信息”区域中选择的“队列属性”，您可能可以指定问题的类型。 从 <b>类型</b> 下拉菜单： </p> 
       <ul> 
        <li> <p><strong>错误报告</strong> </p> </li> 
        <li> <p><strong>更改顺序</strong> </p> </li> 
        <li> <p><strong>问题</strong> </p> </li> 
        <li> <p><strong>请求</strong> </p> </li> 
       </ul> <p>根据Workfront管理员选择的项目首选项，问题类型的名称可能会因您而异。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要联系人</td> 
      <td>默认情况下，“主要联系人”是问题的创建者。 要修改此名称，请在Workfront中开始键入任何活动用户的名称，然后从列表中选择该名称。 问题只能有一个主要联系人。<br> 如果更改主联系人，则原始主联系人仍具有管理问题的访问权限。 在共享问题时，必须从“问题访问”框中手动删除此访问权限。

   <b>笔尖</b>

   添加主要联系人用户时，请注意头像、用户的主要角色及其电子邮件地址，以区分名称相同的用户。 用户必须至少与一个作业角色关联，才能在您添加时查看该角色。


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提交日期和时间</td> 
      <td> <p>这是问题的受让人估计问题将完成的日期。 只有被分配者才能编辑此字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划开始日期</td> 
      <td>默认情况下，计划开始日期是创建问题的日期和时间。 您可以更新 <strong>计划开始日期</strong> 问题。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划完成日期和时间</td> 
      <td> 默认情况下，计划完成日期是自默认计划开始日期起24小时。 默认情况下，问题的持续时间为1天。 您可以更新 <strong>计划完成日期</strong> 问题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际开始日期和时间</td> 
      <td>当您将问题的状态更改为 <strong>正在进行</strong>. 您可以更新 <strong>实际开始日期</strong> 问题。 您可以根据需要手动更新日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际完成日期和时间</td> 
      <td>当您将问题的状态更改为 <strong>已关闭</strong> 或<strong>已解决</strong>. 您可以更新 <strong>实际完成日期</strong> 中。 您可以根据需要手动更新日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">问题解决者</td> 
      <td> <p>这显示问题是否由其他对象解决。 您可以从下拉菜单中选择此问题是由任务、项目解决还是由其他问题解决，然后开始键入将解决此问题的任务、项目或问题的名称。 当列表中显示时选择它。</p>

   <b>注释</b>

   选择要解决问题的对象时，问题状态将链接到解决对象的状态，无法对问题进行更改。 有关解析对象的更多信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.

   <b>笔尖</b>

   当您的系统或组管理员将“解决者”字段添加到问题自定义标头时，当存在与问题关联的解决对象时，该字段将变为“解决问题”、“解决任务”或“解决项目”。

   当此字段显示在问题标题中时，您无法编辑该字段。 有关自定义问题标题的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">使用布局模板自定义对象标头 </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">解决问题、解决任务或解决项目</td> 
      <td>解决问题的问题、任务或问题的链接名称。  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">这个问题已经解决</td> 
      <td>在您访问的问题得到解决时完成的问题的链接名称。  </td> 
     </tr>


   </tbody> 
   </table>





1. 单击 **保存** 或继续编辑以下部分。

#### 分配 {#assignments}

1. 按如上所述开始编辑问题。
1. 单击 **分配** 中。

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. 单击 **搜索人员、角色和团队** 然后，开始键入要分配给该任务的用户、角色或团队的名称，然后单击该名称或在该名称显示在列表中时按Enter键。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含特殊字符。

   >[!TIP]
   >
   >您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。
   >
   >
   >如果在停用用户、作业角色或团队之前已分配它们，则它们仍会被分配到工作项。 在这种情况下，我们建议执行以下操作：
   >
   >* 将工作项重新分配给活动资源。
   >* 将已停用团队中的用户与活动团队相关联，并将工作项重新分配给活动团队。


1. （可选）将鼠标悬停在被分派人的名称上并单击，以指示被分派人是否是问题上的主要被分派人 **设为主要**. 团队不能是问题的主要代理人。
1. 更新以下字段：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">计划小时</td> 
      <td> <p>这是问题的受让者完成问题的实际时间。 键入问题的计划小时数。<br></p> <p>注意：更改问题的计划小时数不会更改问题的计划完成日期。 </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">受让人的角色</td> 
      <td> <p>从 <strong>被分派人的角色</strong> 下拉菜单。 这是受让人可以在此问题上履行的角色。 </p> <p><b>笔尖</b>

   只有与其配置文件中的每个代理人关联的作业角色才会显示在下拉菜单中。</p> </td>
   </tr> 
    </tbody> 
   </table>

1. 单击 **保存** 或继续编辑以下部分。

### 自定义Forms

1. 按如上所述开始编辑问题。
1. 单击 **自定义Forms**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. 在 **添加自定义表单** 字段中，选择要与问题关联的自定义表单。 您必须先构建自定义表单，然后才能在此字段中进行选择。 列表中仅显示活动的自定义表单。 有关构建自定义表单的更多信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 您最多可以在问题中添加10个自定义表单。

1. （视情况而定）如果您将自定义表单附加到问题，请编辑表单上的任何字段。 在保存问题之前，必须指定所有必填字段。

   >[!NOTE]
   >
   >根据Workfront管理员为自定义表单中各个部分设置权限的方式，并非每个人都可以查看或编辑给定自定义表单中的相同字段。 对自定义表单的某个部分中的字段进行编辑的权限取决于您对问题本身拥有的权限。 有关设置自定义表单各部分权限的信息，请参阅 [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md). 有关设置问题权限的信息，请参阅 [共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. 单击 **保存** 或继续编辑以下部分。

### 设置 {#settings}

1. 按如上所述开始编辑问题。
1. 单击 **设置**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   更新以下信息：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">批准流程</td> 
      <td> 
       <div> 
       <p>选择要与问题关联的审批流程。 您的Workfront管理员必须定义系统级别的审批流程，然后才能将它们与问题关联。 具有审批流程管理访问权限的用户 <span> 也可以创建特定于组的审批流程。</span>有关创建审批流程的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建审批流程</a>. </p> 
       <p>添加审批流程时，请考虑以下事项： </p> 
       <ul> 
       <li>列表中仅显示活动的批准流程。 </li> 
       <li> <p>系统范围和特定于组的审批流程将显示在列表中。 与项目组以外的组关联的批准流程不会显示在列表中。</p> <p>重要信息：如果项目组发生更改，则特定于组的审批流程将变为一次性审批流程。 有关项目组更改或审批流程更改如何影响审批设置的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>. </p> </li> 
       <li> <p>您可以定义默认的审批流程，以便在创建请求队列或队列主题时自动附加到问题。 有关更新队列详细信息的信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>. 有关创建队列主题的信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>. </p> </li> 
       <li>在批量编辑问题时，存在以下情况： 
       <ul> 
       <li><p>从同一组中选择多个问题时，此字段中将显示系统级别和特定于组的审批流程。</p></li> 
       <li><p>从不同组中选择多个问题时，此字段中仅显示系统级别的审批流程。</p></li> 
       <li><p>如果任何问题附加了一次性审批流程，则将由您选择的系统级别或组级别审批流程取代。 </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> <p>选中要附加到此问题的提醒通知复选框。 将显示所有问题提醒通知。 您的Workfront管理员必须先配置提醒通知，然后才能对问题进行选择。 有关配置提醒通知的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">设置提醒通知</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **保存。**

## 在问题标题中编辑问题（受限）

您可以在问题标题中编辑有限量的信息。

您的系统或群组管理员可以自定义您在问题标题中看到的字段。 有关信息，请参阅 [使用布局模板自定义对象标头](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

默认情况下，问题标题中包含以下字段：

* 问题名称
* 完成百分比
* 分配
* 计划完成日期和时间
* 状态
* 如果您在当前审批流程中设置为审批者，则应做出审批决策
