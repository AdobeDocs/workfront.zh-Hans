---
product-area: reporting
navigation-topic: reporting-elements
title: 在Adobe Workfront中创建或编辑视图
description: 您可以使用视图自定义在屏幕上显示的信息类型。 您可以在Adobe Workfront中使用多种类型的视图。
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 0c0ffbeefb0eed8d1ca2a6e68ed19b40080726df
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 4%

---

# 在Adobe Workfront中创建或编辑视图

<!-- Audited: 11/2024 -->

您可以使用视图自定义在屏幕上显示的信息类型。 您可以在Adobe Workfront中使用多种类型的视图。

本文介绍了如何创建和编辑列表和报告标准视图。

有关详细信息，请参阅Adobe Workfront中的[视图概述](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</strong></td> 
   <td> 
    <p>参与者或更高版本</p>
    <p>请求或更高版本</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对筛选器、视图、分组的访问权限</p> <p>编辑对报告、功能板、日历的访问权限以在报告中创建视图</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理对报告的权限以创建或编辑报告中的视图</p> <p>管理视图的权限以编辑它</p>
   </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。
+++

## 创建或自定义视图

创建或自定义视图的过程因您是创建或自定义标准视图、Agile视图还是展示板视图而异。

* [创建或自定义标准视图](#create-or-customize-a-standard-view)
* [创建或自定义敏捷视图](#create-or-customize-an-agile-view)

### 创建或自定义标准视图 {#create-or-customize-a-standard-view}

您可以创建新的标准视图，也可以自定义之前创建的现有标准视图。

1. 在要创建或自定义视图的任何列表中单击&#x200B;**视图**&#x200B;下拉菜单。

1. 单击&#x200B;**+新建视图**按钮以创建新视图。
或
单击鼠标上要编辑的现有视图右侧出现的**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)。
将显示**自定义视图**&#x200B;对话框。

1. 在&#x200B;**列预览**&#x200B;部分中，执行以下任一操作：

   * 通过单击列标题并选择新字段来修改任何列的值。
   * 通过单击&#x200B;**添加列**&#x200B;来添加列，开始键入要添加的列的名称，然后在它出现在下拉列表中时单击它。
   * 通过将列标题拖动到新位置来调整列的显示顺序。

   * 在&#x200B;**列设置**&#x200B;区域中，单击&#x200B;**按**&#x200B;汇总此列，然后选择您希望数据在列中显示的方式。 此选项适用于以下列类型：
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>日期字段</strong></td> 
           <td><ul>
           <li>最大</li>
         <li>最小</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>货币字段</strong></td> 
           <td><ul>
           <li>计数</li>
         <li>Sum</li>
           <li>平均</li>
         <li>最大</li>
           <li>最小</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>字符串和布尔字段</strong></td> 
           <td><ul><li>计数</li></ul>
           <p>注意：Workfront通常不建议按计数汇总布尔字段，因为该值将始终为true/false。</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >在分组中汇总以下字段的值时，以下例外适用于父对象（例如，父任务）：
     >   
     > * 除“实际小时数”（例如，“计划/实际劳力成本”、“计划/实际费用成本”、“计划/实际成本”、“计划小时数”）之外的所有数字和货币字段汇总仅子任务和独立任务的值。 它们不会汇总父任务的值或父任务的父值。
     > * 实际小时数汇总了主父任务和独立任务的值；它们不会汇总父任务或子任务的父任务的数字。
     > * 数字和货币值的自定义数据字段汇总了所有任务：父代、子代、父代的父代和独立任务。
     >
     >有关在报表中使用分组的更多信息，请参阅Adobe Workfront中的[分组概述](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)一文。

      * （可选）单击&#x200B;**高级选项**&#x200B;为列指定以下信息：

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>自定义列标签</strong></td> 
           <td><p>指定列的自定义标签。 此标签将替换默认标签。 我们建议仅使用UTF-8字符以避免兼容性问题。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>字段格式</strong></td> 
           <td>选择您希望为列中的字段显示值的格式。</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>在仪表板上显示此列</strong></td> 
           <td><p>当报告与其他报告并排显示时，选择此选项可在功能板上显示此列。 如果未选择此选项，则在报告并排显示的功能板上查看报告时，不会显示此列。</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>列规则</strong></td> 
           <td><p>单击<strong>+为此列</strong>添加规则以定义该列的规则。 添加规则后，您可以定义字段和文本样式，以显示与该规则匹配的字段。 完成规则定义后，单击<strong>添加规则</strong>。</p></td> 
          </tr> 
         </tbody> 
        </table>

        有关报表中条件格式视图的详细信息，请参阅文章[在文本模式下使用条件格式](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md)。

1. （视情况而定）如果您已单击&#x200B;**高级选项**，请单击&#x200B;**完成**。

1. 单击&#x200B;**保存视图**&#x200B;以创建新视图，或使用更改替换当前视图。\
   或\
   单击&#x200B;**另存为新视图**&#x200B;以将更改另存为新视图。

   >[!TIP]
   >
   >在自定义内置Workfront视图时，**另存为新视图**&#x200B;是唯一可用的选项。

   您的访问权限规定了视图的保存方式。 如果最初创建了该视图，则可以保存更改；否则，系统会提示您保存版本。 请记住，您对视图所做的更改会影响与其共享该视图的用户。

### 创建或自定义敏捷视图 {#create-or-customize-an-agile-view}

Agile视图（也称为展示板视图）仅显示项目中的任务和问题列表。

它们已预配置，但您可以为其修改某些设置。

有关Agile视图或展示板视图的详细信息，请参阅文章[在Agile视图中管理项目](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md)。

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
