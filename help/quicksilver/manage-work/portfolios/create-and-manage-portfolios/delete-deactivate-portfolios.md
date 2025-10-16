---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: 删除和停用项目组合
description: 项目组合是Adobe Workfront中的项目或项目群的集合。 如果您发现某个项目组合与您的系统无关，则可以将其删除或停用。
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# 删除和停用项目组合

<!--Audited: 08/2025-->

项目组合是[!DNL Adobe Workfront]中的项目或项目群的集合。 如果您发现某个项目组合与您的系统无关，则可以将其删除或停用。

我们建议停用不再需要与未来项目关联的项目组合，而不是删除它，以保留有关当前与项目组合及其项目群关联的项目的历史信息。

## 访问要求

+++ 展开以查看访问要求。展开以查看本文中各项功能的访问要求。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[！UICONTROL标准版]</p>
   <p>[！UICONTROL计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[！UICONTROL Edit]对项目和项目组合的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合的[！UICONTROL Manage]权限 </p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions on the portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## 删除和停用项目组合概述

在决定删除还是停用项目组合时，请考虑以下事项：

* 删除项目组合将删除与其关联的项目群。

  >[!IMPORTANT]
  >
  >您无需拥有程序的任何权限即可删除项目组合。

* 删除项目组合并不会删除与其关联的项目。
* 您无法恢复已删除的项目组合。
* 停用项目组合可确保在创建项目时，项目组合及其项目的名称不再分配给项目。
* 停用已附加到项目的项目组合不会将其从项目中删除。 如果您从项目中删除已停用的项目组合，则必须先将其重新激活，然后才能将其重新附加到项目。

## 删除项目组合

{{step1-to-portfolios}}

1. 执行下列操作之一：

   * 在列表中选择项目组合，然后单击&#x200B;**[!UICONTROL 删除]**&#x200B;图标![删除图标](assets/delete.png)。
   * 单击项目组合以将其打开，然后单击项目组合名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-icon.png)，然后&#x200B;**删除Portfolio**。
1. 单击&#x200B;**[!UICONTROL 是，将其删除]**&#x200B;以进行确认。

   项目组合已删除，无法恢复。

## 取消激活项目组合

当您停用项目组合时，您仍然可以从[!UICONTROL 项目组合]区域访问该项目组合，但在用户尝试将其添加到项目组合时，它不再显示在项目组合列表中。

>[!NOTE]
>
>根据您的[!DNL Workfront]或组管理员配置布局模板的方式，[!UICONTROL 项目组合]区域可能不会显示在[!UICONTROL 主菜单]中。 有关详细信息，请参阅[使用布局模板自定义主菜单](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)。

{{step1-click-main-menu}}

1. 单击&#x200B;**[!UICONTROL 项目组合]** 。
1. 单击项目组合的名称。
1. 单击项目组合名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 停用Portfolio]**。
项目组合会立即停用。
1. （可选）单击项目组合名称右侧的&#x200B;**更多**&#x200B;菜单![更多菜单](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 激活Portfolio]**&#x200B;以重新激活它。


