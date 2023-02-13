---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移动或删除的群组中的自定义状态
description: 本文介绍了在移动或删除群组时群组自定义状态会发生什么情况。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# 移动或删除的群组中的自定义状态

本文介绍了在移动或删除群组时群组自定义状态会发生什么情况。

## 移动的组中的自定义状态

请考虑以下情景，描述将一个群组移动到另一个群组下的新位置时，群组自定义状态会发生什么情况。

有关移动组的信息，请参阅 [移动组](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">在另一个组下移动组时 </td> 
   <td> <p>被移动组的所有状态都将保留在该状态中。 它们不会添加到群组新父群组的状态中。</p> <p>但是，被移动的组会继承组或组中任何锁定状态，这些状态现在在其层次结构中的位置较高。 此外，从现在起，如果管理员锁定层次结构中较高的状态，则被移动的组会继承该状态。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">当两个组中的状态具有相同的键值但属性不同时</td> 
   <td> <p>假设两个不同的子组从父组继承相同的解锁状态。 然后，这2个群组的群组管理员会通过不同方式自定义其群组的状态。</p> <p>之后，两个组中的一个将移到另一个组下。 现在，它们都具有具有相同键的状态，但是这两个组中具有不同的属性。</p> <p>在这种情况下，以下情况之一为true:</p> 
    <ul> 
     <li>如果新父组中的状态已解锁，则移动组中的状态将保留其属性，不受移动的影响。</li> 
     <li>如果新父组中的状态已锁定，则父组中状态的属性将覆盖移动组中状态的属性。</li> 
    </ul> <p>有关状态键的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>当被移动的组继承了其上一个父组的状态时 </td> 
   <td> <p>从前一个父组继承的所有自定义状态都随被移动的组一起提供，并成为其自己的自定义状态。 它们不再与上一个父组连接。</p> 
    <ul> 
     <li>如果上一个父组在移动后编辑锁定的自定义状态，则所做的更改不会影响已移动子组的状态。</li> 
     <li>如果上一个父组锁定在组移动时已解锁的自定义状态，则移动的子组的状态不会被锁定。</li> 
     <li>现在，被移动的组可以解锁在从前一个父组继承时锁定的状态。</li> 
    </ul> 
     <p><b>示例：</b><p> 
     <p>营销组的组管理员Olivia为组创建了两种状态。 她用ABC的键命名“First Review”，并锁定它。 她用钥匙XYZ给另一个“最终评论”取名，但不锁定它。</p> 
     <p>她还在营销组下创建一个名为“产品营销”的子组。 创建后，它会自动从营销组继承“首次审阅”和“最终审阅”。</p> 
     <p>稍后，Olivia将移动产品组下的产品营销子组。 “首次审核”和“最终审核”会将产品营销组一起转到产品组下的新位置。</p> 
     <p>虽然“首次查看”在移动之前已锁定，但产品营销组管理员现在可以编辑它，因为它不再是由其来源的父组控制的继承状态。</p> 
     <p>“最终审阅”会解锁并可编辑，原来如此。</p> 
     <p>对于营销组，Olivia更改了“第一次审阅”和“最终审阅”的颜色，并将其重命名为“首次审阅 — 编辑”和“最终审阅 — 编辑”。 她还锁定了“最终审阅 — 编辑”。 同时，在产品营销组中，状态“首次审核”和“最终审核”的颜色和名称不会发生更改。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 删除的组中的自定义状态

删除组或子组时，将与其关联的信息（包括其自定义状态）重新分配给其他组或子组。 已删除群组的状态将添加到目标群组的状态。

如果目标组也在使用已删除组的其中一个状态（两个组中的状态具有相同的键），并且目标组以不同的方式自定义了该状态，则目标组版本的设置将覆盖被移动组版本的设置。

>[!INFO]
>
>**示例：**
>
>组A的组管理员为其组重命名已解锁的系统级别状态。 组B的组管理员也会为其组重命名该状态。 尽管状态在两个组中具有不同的名称，但具有相同的键。
>
>之后，A组被删除，其所有信息被重新分配给B组。
>
>* 状态的B组版本的名称将覆盖A组版本的名称。
>* 如果状态在删除组A之前由组A中的某个人应用于某个对象，则该对象上的状态名称将更新为组B所使用状态的名称。
>
>有关状态键的信息，请参阅本文中的表格，位于 [创建或编辑自定义状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [创建或编辑群组的状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>有关删除群组的信息，请参阅 [删除群组](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
