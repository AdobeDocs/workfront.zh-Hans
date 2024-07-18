---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 组如何继承状态
description: 列出组可用的状态时，您会看到以下内容
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# 组如何继承状态

列出组可用的状态时，您会看到以下内容

* 为组创建的自定义状态，如[创建或编辑组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md)中所述。
* 从系统和组层次结构中较高层继承的状态，如本文所述。

## 继承状态

当发生以下任何情况时，您的组将继承状态：

* 创建组。
* 管理员锁定更高级别组中的状态。
* 管理员删除另一个组并选择您的组代替该组。

下表逐一说明了这些情况。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">创建组时</td> 
   <td> <p>创建新组时，它会自动继承：</p> 
    <ul> 
     <li>如果新组是子组，则为组上的一级中的解锁状态。</li> 
    </ul> 
    <ul> 
     <li>系统级别的锁定状态。</li> 
    </ul> 
     <b>示例：</b></span></span> 
     <p>假设一个名为“营销”的组具有2个名为“营销通信”和“品牌推广”的子组。</p> 
     <p>营销组的组管理员会创建新的自定义状态，称为发现。</p> 
     <p>稍后，在营销组下创建一个新的子组，并将其称为Advertising。</p> 
     <p>您的子组会继承“发现”状态，因为您是在其他管理员创建“已解锁的发现”状态之后创建的。</p> 
     <p>由于发生此情况时，营销组下方的营销通信和品牌推广子组已存在，因此它们不会继承解锁的发现状态。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">当管理员在更高级别锁定状态时</td> 
   <td> <p>当Workfront管理员在系统级别锁定状态时，您的组会与系统中的所有其他组一起继承该状态。</p> <p>同样，当管理员锁定组之上的某个组的状态时，该组会与更高层组之下的任何其他子组一起继承该状态。</p> <p><b>注意</b>：稍后，如果管理员在系统级别或组之上的组中解锁这些状态之一，则您的组将保留它以前继承的状态。 现在，它是状态的单独版本，您可以仅为群组自定义它。</p> 
    <p><b>示例：</b></p>
    <p>营销组管理员将锁定上面提到的发现状态，以确保所有3个子组都具有该状态。</p> 
    <p>现在，营销沟通和品牌推广小组以及您的Advertising小组均处于“发现”状态。 当它在上面的Marketing组中锁定时，他们继承了该资产。</p> 
    <p>然后，营销组管理员会解锁发现状态，以便所有3个子组都具有其自己的发现状态版本。 现在，您和其他2个组的管理员可以自定义Discovery状态，以满足您的组的需要。</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">当管理员删除组时</td> 
   <td> <p>当管理员删除组并选择您的组在系统中代替它时，如果您的组中不存在已删除组的自定义状态，则您的组会继承已删除组的自定义状态。</p> 
   <p><b>示例： </b></p>
     <p>一个名为消息传递的组需要与您的Advertising组合并，因此Workfront管理员会删除消息传递组并选择您的组来代替该组。</p> 
     <p>消息传送组的唯一状态为“处理中”。 您的Advertising组现在拥有该状态以供使用。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 继承状态配置

创建顶级组时，它会从系统级别继承以下配置。 创建子组时，它会继承下一个较高组的以下配置。

* 默认状态配置

  有关这些对象的信息，请参阅[使用自定义状态作为默认状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md)。

* 状态显示订单配置

  有关这些对象的信息，请参阅[重新排序系统级和组状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md)。

如果有人在创建组后更改这些配置，则其状态不会受到影响。
