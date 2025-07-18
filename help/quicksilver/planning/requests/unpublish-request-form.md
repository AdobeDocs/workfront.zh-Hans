---
title: 在Adobe Workfront Planning中取消发布请求表单
description: 如果请求表单不再需要或不再相关，您可以取消发布该表单。 取消发布后，您将删除每个人访问该表单的权限。
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '863'
ht-degree: 3%

---

# 在Adobe Workfront Planning中取消发布请求表单


<!--take Preview and Production references at Production time-->

<span class="preview">此页面上高亮显示的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>

{{planning-important-intro}}

如果请求表单不再需要或不再相关，您可以取消发布该表单。 取消发布后，您将删除每个人访问该表单的权限。

如果您希望让一小部分人可以使用请求表单，则还可以更改与共享请求表单的实体。

## 访问要求

+++ 展开以查看访问要求。

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
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront平台</p></td>
   <td>
<p>贵组织的Workfront实例必须载入Adobe Unified Experience才能访问Workfront Planning。</p>
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">适用于Workfront的Adobe Unified Experience</a>。 </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td>
   <td>
   <p>标准</p>
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
   <td>
   <ul>
   <li><p>管理工作区<span class="preview">和记录类型</span>的权限 </p></li>
    <li><p>系统管理员可以管理他们未创建的工作区。 </p></li>
    </ul>
   <p>有关共享Workfront Planning对象权限的信息，请参阅  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">在Adobe Workfront Planning中共享权限概述</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>版面模板</p></td>
   <td> <p>在生产环境中，必须将所有用户（包括系统管理员）分配到包含Planning的布局模板。</p>
<p><span class="preview">在“预览”环境中，标准用户和系统管理员默认启用Planning。</span></p>  
</td>
  </tr>
 </tbody>
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 更改请求表单的共享

如果您与所有人（包括组织外部的用户）公开共享请求，则可以考虑将此访问限制于查看或管理表单关联的工作区的某些用户。

要更改请求表单的共享，请执行以下操作：

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。

1. 单击页眉中记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**管理请求表单**。

   与记录类型关联的所有请求表单都会显示在表格视图中。
1. 将鼠标悬停在请求表单的名称上，然后单击其名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**共享**。
1. 通过选择下列选项之一来更新共享选项：

   * 任何对工作区具有查看或更高访问权限的人员
   * 任何对工作区具有贡献或更高访问权限的人员
   * 任何知道链接的人

   有关详细信息，请参阅[在Adobe Workfront Planning中创建和管理申请表单](/help/quicksilver/planning/requests/create-request-form.md)。
1. （可选）如果您更改了请求表单的共享方式，并且要通过新链接将其共享给新的人员组，请单击&#x200B;**复制链接**。

## 取消发布记录类型的请求表单

当请求表单变得无关紧要，并且您不希望再有任何人访问它时，您可以取消发布它。

{{step1-to-planning}}

1. 单击要在其中添加记录的工作区。

   工作区将打开，记录类型显示为卡片。

1. 单击记录类型卡片。 有关创建记录类型的信息，请参阅[创建记录类型](/help/quicksilver/planning/architecture/create-record-types.md)。

   记录类型页面将在您上次访问的视图中打开。 默认情况下，将在表格视图中打开记录类型页面。

1. 单击页眉中记录类型名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**管理请求表单**。

   与记录类型关联的所有请求表单都会显示在表格视图中。
1. 将鼠标悬停在请求表单的名称上，然后单击其名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-menu.png)，然后单击&#x200B;**取消发布**

或

单击请求表单的名称以将其打开，然后单击请求表单右上角的&#x200B;**取消发布**。

![取消发布按钮突出显示](assets/unpublish-button-highlighted.png)

屏幕底部会显示一条确认消息，通知您表单已取消发布。

**取消发布**&#x200B;链接或按钮更改为&#x200B;**发布**。

1. （视情况而定）如果在打开表单后取消发布表单，请单击&#x200B;**保存**。

   用户无法再通过链接或Workfront请求区域中的请求队列访问请求表单。

   之前使用请求表单添加的任何记录都保留在记录类型页面上。

   之前添加的任何请求都会保留在Workfront的请求区域的规划选项卡上。
