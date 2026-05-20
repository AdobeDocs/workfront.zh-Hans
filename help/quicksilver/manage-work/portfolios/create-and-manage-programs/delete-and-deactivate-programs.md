---
product-area: programs
navigation-topic: Create and manage programs
title: 删除和停用程序
description: 项目群表示共享跨项目边界的共同策略、目标或目标的项目集合。 项目是项目组合的一个细分，它们不能存在于项目组合之外。 项目通常与同一项目组合中的其他项目共享相同的资源。 当程序变得无关时，您可以将其删除或停用。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 605d1ec5-ca2e-4ff0-87e1-fa53d8ac4a95
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 1%

---

# 删除和停用程序

项目群表示共享跨项目边界的共同策略、目标或目标的项目集合。 项目是项目组合的一个细分，它们不能存在于项目组合之外。 项目通常与同一项目组合中的其他项目共享相同的资源。

当项目群变得无关时，您可以执行以下操作之一，以防止用户将项目群与该项目群关联：

* 取消激活项目：现有项目仍与项目群及其相应的项目组合关联。 尝试将新项目与项目群关联时，用户不再将项目群视为选项。
* 删除项目：现有项目将失去与项目的关联，并直接在项目组合下移动。 当用户尝试将其未来的项目与项目群关联时，不再将该项目群视为选项。

我们建议停用而不是删除项目组合，以保留项目的历史信息。 但是，有时可能必须删除项目。

## 访问权限要求

+++ 展开以查看访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 包</td>

<td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>[!UICONTROL 标准版]</p><p>[!UICONTROL 计划]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>[!UICONTROL Edit]对项目组合和程序的访问权限 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>项目组合的[!UICONTROL Manage]权限</p> <p>创建项目后，默认情况下，您拥有[!UICONTROL Manage]权限。</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 删除项目

{{step1-to-programs}}

1. 单击项目名称以将其打开。
1. 单击项目名称右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**删除项目**。
1. 单击&#x200B;**是，将其删除**&#x200B;以进行确认。

   已删除该程序，并出现以下情况：

   * 现有项目将失去与项目的关联，并直接在项目组合下移动。
   * 当用户尝试将其未来的项目与项目群关联时，不再将该项目群视为选项。

## 取消激活项目

{{step1-to-programs}}

1. 单击项目名称以将其打开。
1. 执行下列操作之一：

   * 单击程序名称右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**停用程序**。
   * 单击程序右侧的&#x200B;**更多**&#x200B;菜单，然后单击&#x200B;**编辑**

     或

     单击左侧面板中的&#x200B;**程序详细信息**&#x200B;部分，然后取消选中&#x200B;**处于活动状态**&#x200B;框。

   将立即停用该程序，并出现以下情况：

   * 现有项目仍与项目群及其相应的项目组合关联。
   * 尝试将新项目与项目群关联时，用户不再将项目群视为选项。
