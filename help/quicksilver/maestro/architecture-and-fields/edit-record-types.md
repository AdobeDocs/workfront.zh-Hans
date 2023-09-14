---
title: 编辑记录类型
description: 保存记录类型后，您可以对其进行编辑。 记录类型是AdobeMaestro的对象类型。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the objec types of Adobe Maestro.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 编辑记录类型

>[!IMPORTANT]
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

记录类型是AdobeMaestro的对象类型。 您可以编辑您或其他人创建的记录类型的外观。 有关创建Maestro记录类型的信息，请参阅 [创建记录类型](../architecture-and-fields/create-record-types.md).

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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## 编辑记录类型

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 在Workfront的右上角， <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其创建记录类型的工作区。
1. 将鼠标悬停在记录类型的卡片上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 记录类型卡的右上角，然后单击 **更新外观**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. 在“更新记录类型”框中，更新以下信息：

   * **记录名称**：根据需要编辑记录类型名称。 <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **外观**：编辑与记录类型关联的图标的颜色和形状。 执行以下操作：
      * 选择用于标识记录类型的颜色。 这是记录类型图标的颜色。 默认情况下选中“灰色”。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

     ![](assets/update-record-type-box.png)

1. 单击“更新记录类型”框外部以保存更改。
1. （可选）单击工作区区域中的记录类型卡以打开记录类型的页面。
1. 单击 **更多** “记录类型名称”右侧的菜单，然后单击 **重命名** 重命名记录类型

   或

   重命名标题中的记录类型。  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   您还可以在记录类型页面的标题中重命名记录类型。

