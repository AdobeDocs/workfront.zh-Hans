---
product-area: projects
navigation-topic: manage-issues
title: 编辑问题
description: 您可以编辑有关您创建的问题或其他用户创建的问题（如果他们与您共享问题）的信息。 本文介绍了在有权搜索、查找和编辑问题时，可以如何进行此类操作。
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 0358e79bd606d0035959bba2a47256456b529b18
workflow-type: tm+mt
source-wordcount: '2532'
ht-degree: 3%

---

# 编辑问题

<!--Audited: 10/2025-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

您可以编辑有关您创建的问题或其他用户创建的问题（如果他们与您共享问题）的信息。

您可以编辑单个问题，也可以在列表中编辑问题。 有关编辑列表中的问题的信息，请参阅[编辑列表中的问题](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <ul><li>参与者或更高版本</li>
   <li>浅色或更高版本以编辑任务或项目的问题分区中的问题</li></ul>
   或：
   <ul><li>请求或更高版本</li> <li>查看或更高版本以编辑任务或项目的问题部分中的问题</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别</td> 
   <td> <p>编辑对问题的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>向问题贡献权限以编辑详细信息区域中的以下字段： </p>
   <ul>
   <li>描述</li>
   <li>状态</li>
   <li>严重性</li>
   </ul>
   <p>管理问题的权限以编辑详细信息区域或编辑问题框中的所有字段</p> <p> 有关向问题授予权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">共享问题</a></p> <p>有关请求其他权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license:</p>
   <ul><li>Contributor or higher</li>
   <li>Light or higher to edit issues in the Issues section of a task or project</li></ul>
   <p>Current license:</p>
  <ul><li>Request or higher</li> <li>Review or higher to edit issues in the Issues section of a task or a project</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>Edit access to Issues</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to an issue to edit the following fields in the Details area: </p>
   <ul>
   <li>Description</li>
   <li>Status</li>
   <li>Severity</li>
   </ul>
   <p>Manage permissions to an issue to edit all the fields in the Details area or in the Edit Issue box</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 编辑问题时的限制

有一些限制可能会阻止您编辑问题。

* 您无法编辑批准流程中的问题。 您只能记录时间或更新处于未决批准中的问题的状态。
* 仅当您的Workfront管理员或组管理员在项目偏好设置区域中启用此功能时，您才能编辑文档并将其添加到状态为“完成”、“废弃”或“未决批准”的项目中的问题。 有关设置项目首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

## 编辑单个问题

您可以使用“编辑问题”或“问题详细信息”区域编辑问题。 以下步骤描述了如何在编辑问题框中编辑问题。

1. 转到&#x200B;**主菜单**。
1. 单击&#x200B;**项目**，然后单击项目名称以打开该项目。
1. （可选）单击&#x200B;**任务**，然后单击任务的名称以打开该任务。
1. 单击左侧面板中的&#x200B;**问题**。

   ![问题图标](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. （可选）要编辑有关问题的有限信息，请单击左侧面板中的&#x200B;**问题详细信息**。

   >[!NOTE]
   >
   >根据您的Workfront管理员或组管理员如何修改布局模板，问题详细信息区域中的字段可能会重新排列或不显示。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

   要编辑“详细信息”部分中的信息，请执行以下操作：

   1. （可选）单击右上角的&#x200B;**全部折叠**&#x200B;图标以折叠所有区域。
   1. （可选且有条件）当某个区域折叠时，单击每个区域旁边的&#x200B;**向右箭头** ![向右箭头](assets/right-pointing-arrow.png)以展开要编辑的区域。
   1. （可选）要附加自定义表单，请在&#x200B;**添加自定义表单**&#x200B;字段中开始键入表单的名称，然后在表单显示在列表中时将其选中，然后单击&#x200B;**保存更改**。
   1. （可选）单击&#x200B;**导出**&#x200B;图标![导出图标](assets/export.png)以将概述和自定义表单信息导出到PDF文件，然后单击&#x200B;**导出**。 从以下项中选择：

      * 选择全部（仅在至少附加一个自定义表单时显示）
      * 概述
      * 一个或多个自定义表单的名称

      PDF文件将下载到您的计算机。

      ![导出问题详细信息](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      有关详细信息，请参阅[导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)。

   有关问题详细信息部分中可见字段的信息，请按照以下所述继续编辑问题框中的问题。

1. 要编辑有关问题的所有信息，请在列表中选择问题，然后单击列表顶部的&#x200B;**编辑**

   或

   单击列表中问题的名称，然后单击问题名称旁边的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**编辑。**

   显示&#x200B;**编辑问题**&#x200B;对话框。

   >[!IMPORTANT]
   >
   >您必须具有问题的管理权限才能看到编辑链接。

   所有问题字段在编辑问题框中可用，并按左侧面板中列出的区域分组。

1. 请考虑在以下任意部分中指定信息：

   * [问题名称](#issue-name)
   * [概述](#overview)
   * [任务](#assignments)
   * [自定义表单](#Custom%C2%A0F)
   * [设置](#settings)

   >[!NOTE]
   >
   >根据Workfront管理员如何设置布局模板，您的环境中编辑问题框中的字段可能不同。 有关信息，请参阅[使用布局模板自定义详细信息视图](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。
   >
   >在创建问题时，也可以从新建问题框访问以下部分中列出的大多数字段。 字段所在的部分与“新问题”框不匹配。 有关创建问题的信息，请参阅[创建问题](../../issues/manage-issues/create-issues.md)。

### 问题名称 {#issue-name}

1. 按如上所述开始编辑问题。
1. 单击&#x200B;**问题名称**。

   ![问题名称部分](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. 更新&#x200B;**问题名称**&#x200B;字段。
1. 单击&#x200B;**保存**&#x200B;或继续编辑以下部分。

### 概述 {#overview}

1. 按如上所述开始编辑问题。
1. 单击&#x200B;**概述**。

   ![问题概述部分](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. 更新或查看下表中的任何字段：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td> <p>添加有关问题的其他信息。</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">状态</td> 
      <td> <p>选择问题的状态。 有关问题状态的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">访问系统问题状态的列表</a>。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">优先级</td> 
      <td> <p>这是一个可视化标记，可用于排定问题的优先级。</p> <p>从以下选项中选择：</p> 
       <ul> 
        <li> <p><strong>无</strong> </p> </li> 
        <li> <p><strong>低</strong> </p> </li> 
        <li> <p><strong>正常</strong> </p> </li> 
        <li> <p><strong>高</strong> </p> </li> 
        <li> <p><strong>紧急</strong> </p> </li> 
       </ul> <p>根据您的Workfront管理员选择的项目偏好设置，优先级名称可能有所不同。 有关编辑优先级的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">创建和自定义优先级</a>。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">严重性</td> 
      <td> <p>这是一个可视标志，用于指示问题中描述的问题有多严重。 严重程度特定于问题。 从以下选项中选择：</p> 
       <ul> 
        <li> <p style="font-weight: bold;">轻微</p> </li> 
        <li> <p style="font-weight: bold;">导致混淆</p> </li> 
        <li> <p style="font-weight: bold;">有变通方案的错误</p> </li> 
        <li> <p style="font-weight: bold;">没有变通方案的错误</p> </li> 
        <li> <p style="font-weight: bold;">致命错误</p> </li> 
       </ul> <p>根据您的Workfront管理员选择的项目偏好设置，严重性名称可能有所不同。 有关编辑严重程度的更多信息，请参阅<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">创建或自定义问题严重程度</a>。</p> </td> 
     </tr>

   <tr> 
   <td role="rowheader">问题条件</td> 
   <td> <p>问题的条件是在其上放置一个标记以指示进展情况。</p> 
   <p>您可以自动或手动设置任务或问题的条件。</p>
   <p>您必须被分配到问题才能更改其条件。</p>
   <p>从以下选项中选择：</p> 
      <ul> 
   <li> <p style="font-weight: bold;">进展顺利</p> </li> 
   <li> <p style="font-weight: bold;">一些问题</p> </li> 
   <li> <p style="font-weight: bold;">主要障碍</p> </li> 
   </ul> </td> 
     </tr>

   <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>键入与问题相关信息相关的Web链接。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">类型</td> 
      <td> <p>根据项目经理在项目的队列详细信息区域中选择的队列属性，您也许能够指定问题的类型。 从<b>类型</b>下拉菜单的以下选项中进行选择： </p> 
       <ul> 
        <li> <p><strong>错误报告</strong> </p> </li> 
        <li> <p><strong>更改顺序</strong> </p> </li> 
        <li> <p><strong>问题</strong> </p> </li> 
        <li> <p><strong>请求</strong> </p> </li> 
       </ul> <p>根据Workfront管理员选择的项目偏好设置，问题类型的名称可能有所不同。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要联系人</td> 
      <td>默认情况下，主要联系人是问题的创建者。 要修改此设置，请在Workfront中开始键入任何活动用户的名称，然后从列表中选择该用户。 问题只能有一个主要联系人。<br>如果您更改了主要联系人，则原来的主要联系人仍具有此问题的管理访问权限。 共享问题时，必须从“问题访问权限”框中手动删除此访问权限。

   <b>提示</b>

   <p>添加主要联系人用户时，请注意头像、用户的主要角色及其电子邮件地址，以区分具有相同名称的用户。 用户必须与至少一个工作角色关联，才能在添加时查看工作角色。</p>
      <p> 您必须在访问级别中启用“查看联系信息”设置，用户才能查看用户的电子邮件。 有关信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">授予用户访问权限</a>。</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提交日期和时间</td> 
      <td> <p>这是问题的被分派人估计问题将完成的日期。 只有被分配者才能编辑此字段。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划开始日期</td> 
      <td>默认情况下，计划开始日期是创建问题的日期和时间。 您可以更新问题的<strong>计划开始日期</strong>。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计划完成日期和时间</td> 
      <td> 默认情况下，计划完成日期距默认计划开始日期有24小时。 默认情况下，问题的持续时间为1天。 您可以更新问题的<strong>规划完成日期</strong>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际开始日期和时间</td> 
      <td>当您将问题的状态更改为<strong>进行中</strong>时，会自动填充实际开始日期。 您可以更新问题的<strong>实际开始日期</strong>。 如果需要，您可以手动更新日期。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">实际完成日期和时间</td> 
      <td>当您将问题的状态更改为<strong>已关闭</strong>或<strong>已解决</strong>时，会自动填充实际完成日期。 您可以更新问题的<strong>实际完成日期</strong>。 如果需要，您可以手动更新日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">问题解决者</td> 
      <td> <p>这显示问题是否由其他对象解决。 您可以从下拉菜单中选择此问题是由任务、项目还是其他问题解决，然后开始键入将解决此问题的任务、项目或问题的名称。 当它出现在列表中时将其选中。</p>

   <b>备注</b>

   <ul><li>当您选择对象以解决问题时，问题状态将链接到解决对象的状态，并且无法在该问题上更改。 有关解析对象的详细信息，请参阅<a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述</a>。</li>

   <li>当您连接要由另一个任务、问题或项目解决的问题时，问题中的任何信息都不会传输到解决对象（在“解决者”字段中列出的任务、问题或项目）。 </li>

   <li>当您的系统或组管理员将“解决者”字段添加到问题自定义标题时，当存在与问题关联的解决对象时，该字段将更改为“解决问题”、“解决任务”或“解决项目”。

   当此字段显示在问题标题中时，您无法对其进行编辑。 有关自定义问题标题的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">使用布局模板自定义对象标题</a></li></ul>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">解决问题、解决任务或解决项目</td> 
      <td>解决问题、任务或问题的问题的链接名称。  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">这个问题已经解决</td> 
      <td>在您访问的问题得到解决后完成的问题链接名称。  </td> 
     </tr> 
    </tbody> 
   </table>


1. 单击&#x200B;**保存**&#x200B;或继续编辑以下部分。

#### 任务 {#assignments}

1. 按如上所述开始编辑问题。
1. 单击左侧面板中的&#x200B;**工作**。

   ![问题分派分区](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. 单击&#x200B;**搜索人员、角色和团队**，然后开始键入要分配给问题的用户、角色或团队的名称，然后单击该名称或当它显示在列表上时按Enter。

   <!--
   (NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)
   -->

   >[!NOTE]
   >
   >如果用户名包含特殊字符，则必须在搜索字段中包含特殊字符。

   您可以分配多个用户、工作角色或团队。 您只能分配活动用户、工作角色和团队。

   >[!TIP]
   >
   >
   >如果在停用用户、工作角色或团队之前已分配用户、工作角色或团队，则仍将其分配给工作项目。 在这种情况下，我们建议执行以下操作：
   >
   >* 将工作项重新分配给活动资源。
   >* 将已停用团队中的用户与活动团队关联，并将工作项重新分配给活动团队。

   <!--1. In the Production environment:
         1. Indicate whether an assignee is the primary assignee on the issue, by hovering over the name of the assignee and clicking **Make Primary**. A team cannot be the primary assignee of an issue.
         1. Update the following fields: 
         <table style="table-layout:auto"> 
         <col> 
         </col> 
         <col> 
         </col> 
         <tbody> 
         <tr> 
            <td role="rowheader">Planned Hours</td> 
            <td> <p>This is the amount of actual time it would take the assignees of the issue to complete it. Type the number of Planned Hours for the issue.<br></p> <p><b>NOTE</b></p>  <p>Changing the Planned Hours of the issue will not change the issue Planned Completion Date. </p> </td> 
         </tr> 
         <tr data-mc-conditions=""> 
            <td role="rowheader">Assignee's Role</td> 
            <td> <p>Select a role from the <strong>Assignee's Role</strong> drop-down menu when you selected a person as an assignee. This is the role that the assignee can fulfill on this issue. </p> <p><b>TIP</b>
            
            Only the job roles associated with each assignee in their profile appear in the drop-down menu.</p> </td> 
         </tr> 
         </tbody> 
         </table>-->


1. （可选）单击&#x200B;**分配给我**&#x200B;以将问题分配给您自己。
1. （可选）更新&#x200B;**计划小时数**&#x200B;字段。

   **计划小时数**&#x200B;是问题的被分派人完成该问题所需的小时数。

   >[!NOTE]
   >
   >更改问题的已计划小时数不会更改问题的已计划完成日期。

1. 要从所有问题中删除分配，请参阅[分配问题](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md)。

1. 单击&#x200B;**保存**&#x200B;或继续编辑以下部分。

### 自定义表单

1. 按如上所述开始编辑问题。
1. 单击&#x200B;**自定义Forms**。

   ![问题自定义表单分区](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. 在&#x200B;**添加自定义表单**&#x200B;字段中，选择要与问题关联的一个或多个自定义表单。 您必须先构建自定义表单，然后才可在此字段中选择它们。 列表中仅显示活动的自定义表单。 有关生成自定义表单的详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。 您最多可以为一个问题添加十个自定义表单。

1. （视情况而定）如果您在问题中附加了自定义表单，请编辑表单上的任何字段。 在保存问题之前，必须指定所有必填字段。

   >[!NOTE]
   >
   >根据您的Workfront管理员如何为自定义表单中的部分设置权限，并非每个人都可以查看或编辑给定自定义表单上的相同字段。 编辑自定义表单分区中字段的权限取决于您对问题本身的权限。 有关设置自定义表单各部分的权限的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。 有关设置问题权限的信息，请参阅[共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)。

1. 单击&#x200B;**保存**&#x200B;或继续编辑以下部分。

### 设置 {#settings}

1. 按如上所述开始编辑问题。
1. 单击&#x200B;**设置**。

   ![问题设置图标](assets/settings-section-edit-issue-box-nwe-350x240.png)

   更新以下信息：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">审批流程</td> 
      <td> 
       <div> 
       <p>选择要与问题关联的审批流程。 您的Workfront管理员必须定义系统级别的审批流程，然后才能将他们与问题关联。 对审批流程<span>具有管理权限的用户也可以创建特定于组的审批流程。</span>有关创建审批流程的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建审批流程</a>。 </p> 
       <p>添加审批流程时，请考虑以下事项： </p> 
       <ul> 
       <li>列表中仅显示有效的审批流程。 </li> 
       <li> <p>系统范围及组特定的批准流程会显示在列表中。 与项目组以外的组关联的审批流程不会显示在列表中。</p> <p>重要信息：如果项目组发生更改，则特定于组的审批流程将变成一次性审批流程。 有关对项目组的更改或审批流程中的更改如何影响审批设置的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>。 </p> </li> 
       <li> <p>您可以定义在创建请求队列或队列主题时自动附加到问题的默认批准流程。 有关更新队列详细信息的信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>。 有关创建队列主题的信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>。 </p> </li> 
       <li>批量编辑问题时，存在以下情况： 
       <ul> 
       <li><p>从同一组中选择多个问题时，此字段将显示系统级别和组特定的审批流程。</p></li> 
       <li><p>当您从不同的组中选择多个问题时，此字段仅显示系统级别的审批流程。</p></li> 
       <li><p>当任何问题附加一次性审批流程时，它将被您选择的系统级别或组级别审批流程替换。 </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">提醒通知</td> 
      <td> <p>选中要为其将提醒通知附加到此问题的复选框。 所有问题提醒通知都会显示。 您的Workfront管理员必须配置提醒通知，然后才能在问题中选择它们。 有关配置提醒通知的详细信息，请参阅<a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">设置提醒通知</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存。**

## 编辑问题标题中的问题（受限的）

您可以在问题标题中编辑有限数量的信息。

您的系统或组管理员可以自定义您在问题标题中看到的字段。 有关信息，请参阅[使用布局模板自定义对象标头](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)。

![问题标头](assets/issue-header-350x19.png)

默认情况下，问题标题中包含以下字段：

* 问题名称
* 完成百分比

  有关信息，请参阅[查看和更新任务的完成百分比](/help/quicksilver/manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md)。
* 任务
* 计划完成日期和时间
* 状态
* 如果在当前审批流程中将您设置为审批者，则做出审批决策
