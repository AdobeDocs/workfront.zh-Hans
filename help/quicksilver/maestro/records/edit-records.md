---
title: 编辑记录
description: 您可以在Adobe大师中编辑记录信息。 必须先创建记录类型，然后才能开始创建和编辑记录。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 66a4a1e11ff04008d1d0c77fbd6887e8f5f1c46b
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# 编辑记录

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

您可以在Adobe大师中编辑记录信息。 必须先创建记录类型，然后才能开始创建和编辑记录。
有关信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

&lt;! — 在此提及，详细信息视图中的字段与表格视图中的字段相同 — 本文从“管理记录”视图链接，其中一个引用此信息 — >

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe产品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵公司必须注册AdobeMaestro封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront计划</p></td>
   <td>
<p>任何</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证</p></td>
   <td>
   <p>任何</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">访问级别</td>
   <td> <p>任何</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">布局模板</td>
   <td> <p>系统管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/grant-access.md">授予对Adobe大师的访问权限</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 有关编辑记录的注意事项

* 您可以编辑您或其他用户创建的记录。 <!--will change with access levels-->
* 您无法编辑从其他记录链接的字段或包含计算的字段。
* 如果显示的记录链接到其他记录，则您正在编辑的记录的新信息将反映在链接的记录上。
* 不能批量编辑记录。 <!--this will probably change-->
* 只有当URL以以下内容开头时，才会被识别为单行文本字段类型中的链接： http://、https://、ftp://或www。.
* 编辑段落类型字段时，可以使用以下富文本格式选项：

   * 粗体
   * 斜体
   * 下划线
   * 添加链接
   * 添加项目符号列表
   * 添加编号列表

## 编辑记录

您可以从以下区域编辑记录：

* [从记录的详细信息页面](#edit-a-record-from-the-records-details-page)
* [从记录类型的表格视图中](#edit-a-record-from-the-record-type-table-view)

### 从记录的“详细信息”页面编辑记录

1. 单击 **主菜单** ![](assets/main-menu-workfront.png) 位于右上角，或 **主菜单** ![](assets/main-menu-shell.png) （如果可用），然后单击 **大师**.

   您上次访问的工作区将打开。

1. （可选）单击工作区名称右侧的向下箭头，选择要更新其记录的工作区。
1. 执行下列操作之一：

   * 在“表”视图中，单击记录的名称。
   * 在“表”视图中，将鼠标悬停在记录名称上，然后单击 **更多** 菜单 ![](assets/more-menu.png)，然后单击 **视图**

     ![](assets/contextual-menu-for-record-row.png)
   * 在“时间轴”视图中，单击记录栏。

   记录 **详细信息** 页面将打开。

1. 单击 **更多** 菜单 ![](assets/more-menu.png) 记录名称的右侧，然后单击 **编辑**

   或

   在“详细信息”页面上的任何可编辑字段中单击以编辑信息。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. 单击 **保存更改**. <!--logged a bug for this - this needs to be "Save"-->

### 从记录类型表格视图中编辑记录

1. 单击 **主菜单** ![](assets/main-menu-workfront.png) 位于右上角，或 **主菜单** ![](assets/main-menu-shell.png) （如果可用），然后单击 **大师** ![](assets/maestro-icon.png).

   您上次访问的工作区随即打开。

1. （可选）单击工作区名称右侧的向下箭头，选择要更新其记录的工作区。
1. 单击记录类型卡片。

   此时将打开记录类型页面。
1. （视情况而定）从 **视图** 下拉菜单（位于表的右上角），选择 **表** 视图。 这应为默认视图，除非您在上次访问时查看了时间轴视图中的记录类型。

   与所选记录类型关联的记录将显示在表格视图中。
1. 单击记录行内部以开始编辑有关内联记录的信息。

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. 按 **输入** 或单击行外以保存更改。 更改将自动保存。 “已保存”的指示器会短暂显示在表格视图的右上角，表示已保存更改。

   >[!NOTE]
   >
   >  您无法编辑以下字段的信息，因为它们是只读的，Workfront会自动更新它们：
   >  
   >  * 通过链接记录类型创建的链接字段
   >  * 以下类型的字段：“创建者”、“创建日期”、“上次修改者”、“上次修改日期”


1. （可选）复制某个字段的现有值，然后将其粘贴到另一条记录上的相同类型字段中，然后单击 **输入** 以保存更改。

   >[!NOTE]
   >
   >请考虑以下事项：
   >
   >* 不能从其他源复制信息，不能从与粘贴信息的字段类型相同的Maestro字段复制。
   >
   >* 您无法复制和粘贴在记录的“详细信息”区域中显示的字段的字段值。
   >* 不能复制和粘贴以下字段类型的字段值：
   ><ul>
   >
   > * 人员
   >
   > * 系统字段
   >
   > * 因连接记录而创建的链接字段

   <!--take People out of the list above when they release this - this might be coming later-->
