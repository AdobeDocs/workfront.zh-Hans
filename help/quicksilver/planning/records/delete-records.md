---
title: 删除记录
description: 您可以删除您或其他用户创建的记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 1%

---


# 删除记录

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

您可以删除Adobe Workfront Planning中不再相关的记录。 删除的记录删除后，您可以在30天内恢复这些记录。 有关恢复已删除记录的信息，请参阅[恢复已删除的记录](/help/quicksilver/planning/records/restore-deleted-records.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront包</p></td> 
   <td> 
<ul> 
<li><p>任何Workfront和任何Planning包</p></li>
或
<li><p>任何工作流和任何计划包</p></li></ul>
<p>有关每个Workfront Planning包中所包含内容的更多信息，请联系您的Workfront客户代表。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>标准</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>向工作区和记录类型提供或更高权限  </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr>   
</tbody> 
</table>

有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++   


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## 有关删除记录的注意事项

* 您可以删除您或其他用户创建的记录。
* 您可以恢复您或其他人已删除的记录。
* 如果删除的记录链接到其他记录，则不会删除链接的记录，但也会删除来自已删除记录的信息。
* 您无法从时间轴或日历视图中删除记录。

## 删除记录

您可以从以下区域删除记录：

* [从记录的页面](#delete-a-record-from-the-records-page)
* [从记录类型的表视图中](#delete-a-record-from-the-record-type-table-view)

### 从记录的页面中删除记录

{{step1-to-planning}}

1. 单击要删除其记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. 执行下列操作之一：

   * 在“表”视图中，单击记录的名称。
   * 在“表”视图中，将鼠标悬停在记录名称上，然后单击&#x200B;**更多**&#x200B;菜单![更多](assets/more-menu.png)，然后单击&#x200B;**查看**

     ![记录行的上下文菜单](assets/contextual-menu-for-record-row.png)
   * 在“时间轴”视图中，单击记录栏。

   此时将打开记录页面。

1. 单击记录名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**删除**，再次&#x200B;**删除**&#x200B;以进行确认。

   ![记录详细信息页面中的更多菜单选项](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
删除记录。
1. （可选）转到记录页面的表格视图，单击视图右上角的&#x200B;**撤消**&#x200B;图标![撤消图标](assets/undo-icon.png)，然后单击&#x200B;**最近删除的记录**&#x200B;以恢复删除的记录。

有关恢复已删除记录的信息，请参阅[恢复已删除的记录](/help/quicksilver/planning/records/restore-deleted-records.md)。

### 从记录类型表格视图中删除记录

{{step1-to-planning}}

1. 单击要删除其记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. （视情况而定）从表左上角的&#x200B;**视图**&#x200B;下拉菜单中，选择表视图。 这应为默认视图，除非您在上次访问时查看了时间轴视图中的记录类型。

   与所选记录类型关联的记录将显示在表格视图中。
1. 执行下列操作之一：

   * 右键单击记录行，然后单击&#x200B;**删除**。
   * 单击记录名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**删除**。

     ![记录行的上下文菜单](assets/contextual-menu-for-record-row.png)

   * 单击&#x200B;**打开详细信息**&#x200B;图标![在表名称字段中打开详细信息图标](assets/open-details-icon-in-table-name-field.png)以打开包含记录详细信息的框，然后单击记录名称右侧的&#x200B;**更多** ![更多菜单](assets/more-menu.png)，然后&#x200B;**删除**。

   删除记录。

1. （可选）执行以下操作之一以撤消或重做删除记录：

   * 单击&#x200B;**撤消**&#x200B;图标![撤消图标](assets/undo-icon.png)，然后单击&#x200B;**最近删除的记录**&#x200B;以恢复删除的记录。 有关恢复已删除记录的信息，请参阅[恢复已删除的记录](/help/quicksilver/planning/records/restore-deleted-records.md)。
   * 使用以下键盘快捷键可撤消或重做删除记录：

      * 按CTRL + Z (⌘ + Z表示Mac)以撤消删除记录
      * 按CTRL + Shift + Z (⌘ + Shift + Z用于Mac)以重做删除记录




