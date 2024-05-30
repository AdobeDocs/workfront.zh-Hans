---
title: 编辑记录类型
description: 保存记录类型后，您可以对其进行编辑。 记录类型是Adobe Workfront Planning的对象类型。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 49335ec86057e4985477034558a271bf4efcab5e
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# 编辑记录类型

{{planning-important-intro}}

记录类型是Adobe Workfront Planning的对象类型。 您可以编辑您或其他人创建的记录类型的外观。 有关创建Workfront Planning记录类型的信息，请参阅 [创建记录类型](../architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>要将Adobe Workfront Planning记录类型与Experience Manager Assets连接，您必须具有Adobe Experience Manager Assets许可证，并且贵组织的Workfront实例必须载入Adobe业务平台或Adobe Admin Console。</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront协议</p></td>
   <td>
<p>贵组织必须注册Adobe Workfront计划封闭测试版计划。 请联系您的客户代表以查询此新产品/服务。 </p>
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
   <td> <p>Workfront Planning没有访问级别控制</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>权限</p></td>
   <td> <p>管理工作区的权限</a> </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区
</td>
  </tr>
<tr>
   <td role="rowheader"><p>布局模板</p></td>
   <td> <p>您的Workfront或组管理员必须在布局模板中添加Planning区域。 有关信息，请参阅 <a href="../access/access-overview.md">访问概述</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## 编辑记录类型

{{step1-to-maestro}}

默认情况下应打开上次访问的工作区。

1. （可选）展开现有工作区名称右侧的向下箭头，然后选择要编辑其记录类型的工作区。
1. 将鼠标悬停在记录类型的卡片上，然后单击 **更多** 菜单 ![](assets/more-menu.png) 记录类型卡的右上角，然后单击 **编辑**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. 在 **编辑记录类型** 框中，更新以下信息：

   * 根据需要编辑记录类型名称。 <!--did they add a field label for this? -->
   * **描述**：编辑或添加记录类型的描述，其中包含有关该记录类型的更多信息。
   * 编辑与记录类型关联的图标的颜色和形状。 执行以下操作：
      * 选择用于标识记录类型的颜色。 这是记录类型图标的颜色。 默认情况下选中“灰色”。
      * 从列表中选择一个图标，或开始键入图标的名称以描述其表示的内容，然后在显示时选择它。 这是记录类型的图标。 默认情况下，会选择一个文件图标。

     ![](assets/update-record-type-box.png)

1. 单击&#x200B;**保存**。
1. （可选）单击工作区区域中的记录类型卡以打开记录类型的页面。
1. 单击 **更多** “记录类型名称”右侧的菜单，然后单击 **编辑** 更新有关记录类型的信息。

   >[!TIP]
   >
   >   您可以重命名标题中的记录类型。

   ![](assets/more-menu-options-from-record-details-page.png)

   <!--check this screen shot - not sure this is valid ???-->

1. （可选）展开记录类型名称右侧的向下箭头，然后选择要编辑的其他记录类型。
