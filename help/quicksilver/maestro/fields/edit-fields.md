---
title: 编辑字段
description: 在Adobe管理器中，您可以编辑已创建字段的字段设置。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: c264c0c96b818934a7c25ed54c7666d2d6c95e54
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->


# 编辑字段

>[!IMPORTANT]
>
>本文中的信息是指AdobeMaestro，它是Adobe Workfront提供的新产品。
>
>目前，AdobeMaestro是测试版计划的一部分，该计划对有限数量的客户开放。 您必须是Workfront客户才能使用Maestro功能。
>
>有关加入Maestro测试版计划的更多信息，请与您的客户代表联系。
>
>有关信息，请参阅 [Adobe大师概述](../maestro-overview.md).

您可以编辑已创建字段的字段设置。

有关创建Adobe生成器字段的信息，请参阅 [创建字段](../fields/create-fields.md).

本文介绍了如何编辑Maestro字段的设置。 有关编辑Maestro记录的字段值的信息，请参见 [编辑记录](/help/quicksilver/maestro/records/edit-records.md).

## 有关编辑字段信息的注意事项

* 如果您对字段所属的工作区具有管理权限，则可以编辑您创建的字段或其他用户创建的字段。
* 您可以在记录类型表中编辑字段。
* 您无法在记录的详细信息页面或时间线视图中编辑字段。
* 保存字段后，您无法编辑字段类型。
* 如果附加到“数字”、“百分比”或“货币”字段的记录中已经存储了负值，则不能取消选择以前选择的“允许负数”设置。
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 产品</p> </td>
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
   <td role="rowheader"><p>访问级别配置</p></td>
   <td> <p>Maestro没有访问控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Maestro区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 编辑字段

1. 单击 **主菜单** 图标 ![](assets/main-menu-workfront.png) 位于Workfront的右上角，或者 **主菜单** 图标 ![](assets/main-menu-shell.png)  （如果可用），然后单击 **大师** ![](assets/maestro-icon.png).

   默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要为其删除记录类型的工作区。

   工作区将打开，并显示与其关联的记录类型和分类。
1. 单击要编辑其字段的记录类型或分类卡。

   这将打开记录类型的页面。
1. （视情况而定）选择 **表格视图** 从 **视图** 记录类型页面右上角的下拉菜单
1. 将鼠标悬停在要编辑的字段的列标题上，单击字段名称后的向下箭头，然后单击 **编辑字段**

   或

   双击该字段的列标题。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 更新有关该字段的信息并单击 **保存**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >保存字段后无法更新字段类型。


1. （视情况而定）对于链接的记录字段，单击 **编辑查找字段** 并从链接的记录类型中添加或删除任何字段。

   有关更多信息，请参阅 [连接记录类型](../architecture/connect-record-types.md).
