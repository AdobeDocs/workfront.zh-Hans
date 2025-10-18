---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 移动或删除的组中的自定义状态
description: 本文介绍了在移动或删除组时组自定义状态所发生的情况。
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# 移动或删除的组中的自定义状态

本文介绍了在移动或删除组时组自定义状态所发生的情况。

## 已移动组中的自定义状态

考虑以下情景，描述当您将一个组移动到另一个组下的新位置时，组自定义状态会发生什么情况。

有关移动组的信息，请参阅[移动组](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md)。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">将组移动到另一个组下时 </td> 
   <td> <p>所有已移动组的状态都保持不变。 它们不会添加到组的新父组的状态。</p> <p>但是，被移动的组会继承该组中任何锁定状态，或者继承其层次结构中现在更高的组。 从现在起，如果管理员锁定了层次结构中较高位置的状态，则被移动的组将继承该状态。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">当两个组中的状态具有相同的键但不同的属性时</td> 
   <td> <p>假设两个不同的子组从父组中继承相同的解锁状态。 然后，这两个组的组管理员会以不同的方式自定义其组的状态。</p> <p>之后，将两个组中的一个移到另一个组的下方。 现在，这两个用户都有一个具有相同键的状态，但这两个用户组中有不同的属性。</p> <p>在本例中，以下任一情况为真：</p> 
    <ul> 
     <li>如果新父组中的状态已解锁，则被移动组中的状态将保留其属性，不受移动的影响。</li> 
     <li>如果新父组中的状态被锁定，则父组中的状态属性将覆盖移动组中的状态属性。</li> 
    </ul> <p>有关状态键的信息，请参阅<a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">创建或编辑状态</a>。</p> </td> 
  </tr> 
  <tr> 
   <td>当移动组的状态继承自其上一个父组时 </td> 
   <td> <p>从上一个父组继承的所有自定义状态都随移动的组一起出现，并成为其自己的自定义状态。 它们不再与上一个父组连接。</p> 
    <ul> 
     <li>如果上一父组在移动后编辑已锁定的自定义状态，则更改不会影响已移动子组的状态。</li> 
     <li>如果上一个父组锁定在组移动时解锁的自定义状态，则被移动的子组的状态不会锁定。</li> 
     <li>被移动的组现在可以解锁从上一个父组继承时锁定的状态。</li> 
    </ul> 
     <p><b>示例：</b><p> 
     <p>营销组的组管理员Olivia为该组创建两个状态。 她用键ABC命名了第一篇评论，并锁定了它。 她用XYZ键为另一个最终评论命名，并且没有锁定。</p> 
     <p>她还在营销组下创建了一个名为产品营销的子组。 在创建时，它会自动从营销组继承“首次审核”和“最终审核”。</p> 
     <p>稍后，Olivia将产品营销子组移到产品组下。 首次审阅和最终审阅都随产品营销组一起移至其位于产品组下的新位置。</p> 
     <p>虽然首次查看在移动之前被锁定，但产品营销组管理员现在可以编辑它，因为它不再是由其来源的父组控制的继承状态。</p> 
     <p>“最终审阅”已解锁，可以像往常一样编辑。</p> 
     <p>对于营销组，Olivia更改了“首次审阅”和“最终审阅”的颜色，并将其重命名为“首次审阅已编辑”和“最终审阅已编辑”。 她还锁定“最终审核编辑”。 同时，在产品营销组中，“首次审阅”和“最终审阅”状态的颜色和名称不会更改。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 已删除的组中的自定义状态

删除组或子组时，将与其关联的信息（包括其自定义状态）重新分配给另一个组或子组。 已删除组的状态将添加到目标组的状态。

如果已删除组的状态之一也由目标组使用（两个组中的状态具有相同的键），并且目标组以不同的方式自定义了状态，则目标组版本的设置将覆盖移动组的版本的设置。

>[!INFO]
>
>**示例：**
>
>A组的组管理员会为其组重命名已解锁的系统级状态。 B组的组管理员也会为其组重命名该状态。 虽然状态在两个组中的名称不同，但它具有相同的键。
>
>之后，删除组A，将其所有信息重新分配给组B。
>
>* 组B版本状态的名称将覆盖组A版本的名称。
>* 如果在删除某个组A中的某个人将该状态应用于该组，则该对象的状态名称将更新为组B使用的状态名称。
>
>有关状态键的信息，请参阅本文中[创建或编辑自定义状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [创建或编辑组的状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create)下的表。
>
>有关删除组的信息，请参阅[删除组](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)。
