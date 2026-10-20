---
content-type: api
navigation-topic: general-api
title: 以非管理员用户管理事件订阅
description: 如果您的Workfront访问权限允许，您可以在权限和系统配置允许的范围内创建、查看和删除事件订阅。
author: Courtney
feature: Workfront API
role: Developer
source-git-commit: f0cde465a56d0cc936e8c886f4a120dec5fe5f73
workflow-type: tm+mt
source-wordcount: '342'
ht-degree: 5%
---

# 以非管理员用户管理事件订阅

如果您的Workfront访问权限允许，则可以从“设置”区域创建、查看和删除事件订阅。 但是，您的访问权限仅限于您的角色和组织的系统配置授权的订阅和操作。

并非每个用户都可以像对Workfront管理员一样使用此功能。 具有所需访问权限的用户只能在授予他们的范围内管理事件订阅。

例如，您的权限可能允许您仅管理一组已定义工作的某些对象类型、事件类型或预订。 您不能在访问和配置所允许的范围之外管理事件订阅。

有关管理员管理的设置，请参阅[在Workfront中配置事件订阅](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)。

有关事件订阅API的信息，请参阅[事件订阅API](/help/quicksilver/wf-api/general/event-subs-api.md)。

>[!NOTE]
>
>用户只能在其权限和组织的系统配置允许的范围内管理事件订阅。 访问权限并不自动等同于管理员访问权限。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 包</td>
   <td>“任一”</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront许可证</td>
   <td>
    <p>标准</p>
    <p>规划</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">访问级别配置</td>
   <td>
    <p>您必须具有相应的访问权限才能管理事件订阅。</p>
    <p>您的访问权限仅限于您的权限所允许的订阅和操作以及贵组织的系统配置。</p>
   </td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用事件订阅

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**系统**，然后单击&#x200B;**事件订阅**。
1. 查看您可用的订阅。
1. 仅创建、查看或删除授权范围内的订阅。

如果您看不到预期的选项，或者如果您无法创建或管理订阅，请与Workfront管理员联系，确认您的访问权限是否受角色、权限或系统配置的限制。

## 相关文章

* [在Workfront中配置事件订阅](/help/quicksilver/administration-and-setup/manage-workfront/manage-event-subscriptions/configure-event-subscriptions-in-workfront.md)
* [事件订阅API](/help/quicksilver/wf-api/general/event-subs-api.md)
