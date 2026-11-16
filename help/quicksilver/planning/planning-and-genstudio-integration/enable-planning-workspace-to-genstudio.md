---
title: 在GenStudio for Performance Marketing中启用Workfront规划Workspace
description: 当您同时拥有这两个应用程序的访问权限时，可以使Adobe Workfront Planning工作区在GenStudio for Performance Marketing中可用。
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 3%
---
# 在GenStudio for Performance Marketing中启用Workfront规划工作区

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

如果贵公司同时购买了Adobe GenStudio for Performance Marketing并且您是Adobe Workfront Planning客户，则Workfront Planning中还提供了GenStudio工作区。

如果您在Workfront Planning中已有Planning工作区，则可以为GenStudio for Performance Marketing启用它，而不是在GenStudio中从中重新创建相同的数据。

启用工作区可将其链接到Adobe Could Storage项目，并将其记录类型和字段映射到GenStudio工作区。 完成配置后，您可以在GenStudio中打开工作区的记录。

您必须具备以下条件：

* 访问Workfront Planning和GenStudio for Performance Marketing。
* 链接到工作区的Adobe云存储项目。 组织管理员可以在Adobe Admin Console中创建一个。

  有关信息，请参阅[管理Adobe存储](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)。<!--ensure this site still works-->

## 访问权限要求

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
   <td role="rowheader"><p>Adobe Workfront 包</p></td> 
   <td> 
<p>任何Workfront或工作流以及任何计划包</p> 
或
<p>作为独立产品购买时的任何Planning包</p>

</td> 
   <tr> 
<td> 
   <p> 其他产品</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Adobe Admin Console设置</p> </td> 
   <td> 
   <p> 您必须在Adobe Admin Console中创建Adobe Storage Cloud项目 </p>

<p>有关信息，请参阅<a href="https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">管理项目</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td><p>工作流标准</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe计划许可证</p></td> 
   <td><p>规划标准</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Adobe Workfront访问级别配置</p></td> 
   <td> <p>当您同时具有Workflow和Planning包时，必须将Workflow和Planning许可证类型添加到Workfront访问级别</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing用户角色</p></td> 
   <td><p><ul><li>任何GenStudio用户角色（如果您需要访问营销活动、产品和角色）</li>
   <li>GenSudio System Manager（如果您需要访问激活） <!--and Events--></li></ul>
   有关信息，请参阅<a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">用户角色和权限</a>。 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>  
   <p>在Workfront规划中： </p>
   <ul>
   <li><p>管理对工作区的权限 <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>在Adobe GenStudio for Performance Marketing中： <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> 在Adobe GenStudio for Performance Marketing中创建权限以创建项目</p></li></ul>
   </td>  
</tbody> 
</table>

有关Adobe Workfront Planning访问权限的信息，请参阅[Adobe Workfront Planning访问概述](/help/quicksilver/planning/access/access-overview.md)。

有关Adobe GenStudio for Performance Marketing的详细信息，请参阅[Adobe GenStudio for Performance Marketing用户指南](https://experienceleague.adobe.com/zh-hans/docs/genstudio-for-performance-marketing/user-guide/home)。

+++ 

## 在GenStudio中启用Workfront规划工作区

1. 在Workfront Planning中，打开要启用的工作区。
1. 单击工作区名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**启用GenStudio**。

   **使工作区GenStudio**&#x200B;已启用框打开，包括以下步骤：

   1. **ACPC项目**：选择要与此工作区同步的&#x200B;**ACPC项目** （Adobe Cloud Storage项目），然后单击&#x200B;**下一步**。 用户通过此项目访问GenStudio中的工作区。

      ![启用工作区GenStudio - ACPC项目步骤](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **记录类型**：将工作区的记录类型映射到GenStudio所需的六种记录类型：

      * 营销活动
      * 产品
      * 用户画像
      * 渠道
      * 区域
      * 激活

      对于每个记录，请打开列表并选择匹配的Planning记录类型，或选择&#x200B;**添加新**&#x200B;以创建该记录，然后单击&#x200B;**下一步**。

      ![启用工作区GenStudio — 记录类型步骤](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **字段**：映射每个记录类型的字段。 使用对话框顶部的选项卡在记录类型之间移动。 对于每个字段，请选择匹配的Planning字段，或选择&#x200B;**添加新**&#x200B;以创建字段。

      对所有记录类型重复字段设置。

      ![启用工作区GenStudio — 字段步骤](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. 查看并解决任何警告。

      例如，新字段可以成为记录类型的主字段，或者已使用的字段别名被重命名（如果您已经有一个名为“Regions”的字段，则导入的字段可能会变为“Regions 2”）。

      映射&#x200B;**状态**&#x200B;字段会添加所需选项。

   1. 单击&#x200B;**发布**。

      启用工作区后，将显示一条确认消息。 在工作区中标记映射的记录类型。

      映射到可从GenStudio访问的记录类型卡片上有一个新的&#x200B;**Adobe**&#x200B;图标。

      ![带有Adobe图标的促销活动记录类型](assets/campaigns-record-type-card-with-adobe-icon.png)

1. 打开GenStudio，选择&#x200B;**促销活动**，然后单击屏幕左下角最初为此设置配置的&#x200B;**ACPC项目**。 查看导入的记录类型和字段。

   >[!TIP]
   >
   >您只会看到您的Adobe Cloud Storage项目成员资格允许的记录。
