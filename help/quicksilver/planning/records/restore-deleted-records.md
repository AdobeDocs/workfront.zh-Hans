---
title: 恢复已删除的记录
description: 您可以从Adobe Workfront Planning的“最近删除”区域中恢复已删除的记录。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 6327e5625481ce7ff8d744bc6eb50d417cbb4413
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 1%

---


# 恢复已删除的记录

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

您可以从Adobe Workfront Planning的“最近删除”区域中恢复已删除的记录。

有关删除记录的信息，请参阅[删除记录](/help/quicksilver/planning/records/delete-records.md)。

## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准</p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员对所有工作区具有权限，包括他们未创建的工作区</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 有关恢复已删除记录的注意事项

* 记录会储存在“最近删除”的纸盒中30天。 30天后，这些记录将从Workfront Planning中永久删除。
* 如果删除的记录链接到其他记录，则不会删除链接的记录，但也会删除来自已删除记录的信息。 恢复删除的记录将恢复连接记录中的信息。
* 您可以批量恢复记录。
* 删除记录后，以下信息将存储在“最近删除”框中：
   * **名称**：这是记录的“主要”字段中的信息。 有关记录主字段的详细信息，请参阅[主字段概述](/help/quicksilver/planning/fields/primary-field-overview.md)。
   * **删除日期**：记录删除的时间和日期。
   * **最近删除的时间**：自记录删除后的时间。 在当前日期之前30天以上被删除的记录不会显示在“最近删除”框中。
   * **删除者**：删除记录的用户的名称。

## 恢复已删除的记录

1. 转到已删除记录的记录类型页面。
1. 单击任何记录类型页面视图右上角的&#x200B;**撤消**&#x200B;图标![](assets/undo-icon.png)，然后单击&#x200B;**最近删除的**。

   此时会显示&#x200B;**最近删除的**&#x200B;框。

   ![](assets/recently-deleted-box.png)

1. 选择要删除的记录，然后单击&#x200B;**还原** > **还原**。 您可以选择多个记录。

   如果恢复成功，您将在屏幕底部收到成功通知。
1. 转到表视图并查看已还原的记录。