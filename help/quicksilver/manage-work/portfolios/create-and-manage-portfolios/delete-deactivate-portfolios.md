---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 删除和停用项目组合
description: Portfolio是Adobe Workfront中的项目或项目群的集合。 如果您发现某个项目组合与您的系统无关，则可以将其删除或停用。
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# 删除和停用项目组合

<!--Audited: 01/2024-->

Portfolio是项目或项目群的集合 [!DNL Adobe Workfront]. 如果您发现某个项目组合与您的系统无关，则可以将其删除或停用。

我们建议停用不再需要与未来项目关联的项目组合，而不是删除它，以保留有关当前与项目组合及其项目群关联的项目的历史信息。

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>新文档： [！UICONTROL Standard] </p>
   <p>当前： [！UICONTROL计划] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>[！UICONTROL Edit]对项目和Portfolio的访问权限</p> <p><b>注释</b></p> <p> 如果您没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以更改您的访问级别，请参见 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合的[！UICONTROL Manage]权限 </p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

## 删除和停用项目组合概述

在决定删除还是停用项目组合时，请考虑以下事项：

* 删除项目组合将删除与其关联的项目群。

  >[!IMPORTANT]
  >
  >您无需拥有程序的任何权限即可删除项目组合。

* 删除项目组合并不会删除与其关联的项目。
* 您无法恢复已删除的项目组合。
* 停用项目组合可确保在创建项目时，项目组合及其项目的名称不再分配给项目。

## 取消激活项目组合

当您停用项目组合时，您仍然可以从以下位置访问它： [!UICONTROL Portfolio] 区域，但是当用户尝试将其添加到项目时，它不再显示在项目组合列表中。

>[!NOTE]
>
>根据贵机构的 [!DNL Workfront] 或组管理员配置布局模板， [!UICONTROL Portfolio] 区域可能不会显示在 [!UICONTROL 主菜单]. 有关更多信息，请参阅 [使用布局模板自定义主菜单](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 位于的右上角 [!DNL Adobe Workfront].

1. 单击 **[!UICONTROL Portfolio]** .
1. 单击项目组合的名称。
1. 单击 **更多** 菜单 ![](assets/more-icon.png) 项目组合名称的右侧，然后单击 **[!UICONTROL 取消激活Portfolio]**.

## 删除项目组合

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) Adobe Workfront的右上角。

1. 单击 **[!UICONTROL Portfolio]** .
1. 选择项目组合，然后单击 **[!UICONTROL 删除]**&#x200B;此&#x200B;项 [!UICONTROL 删除] 图标 ![](assets/delete.png).
1. 在出现的框中，单击 **[!UICONTROL 是的，删除它]** 以确认。
