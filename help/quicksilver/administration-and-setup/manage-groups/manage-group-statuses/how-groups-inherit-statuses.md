---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: 组如何继承状态
description: 列出群组可用的状态时，您会看到以下信息
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# 组如何继承状态

列出群组可用的状态时，您会看到以下信息

* 为群组创建的自定义状态，如 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* 从系统继承和从组层次结构中的较高层继承的状态，如本文中所述。

## 继承状态

发生以下任何情况时，您的组会继承状态：

* 您创建群组。
* 管理员锁定较高级别组中的状态。
* 管理员会删除另一个组并选择您的组来替代它。

下表说明了每种情况。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">创建群组时</td> 
   <td> <p>创建新组时，该组会自动继承：</p> 
    <ul> 
     <li>如果新组是子组，则在组上一级中处于已解锁状态。</li> 
    </ul> 
    <ul> 
     <li>系统级别的锁定状态。</li> 
    </ul> 
     <b>示例：</b></span></span> 
     <p>假设一个名为“营销”的组有2个名为“营销通信和品牌”的子组。</p> 
     <p>营销组的组管理员创建一个名为“发现”的新自定义状态。</p> 
     <p>稍后，您在营销组下创建一个新子组，并将其命名为“广告”。</p> 
     <p>您的子组会继承发现状态，因为您在其他管理员创建解锁的发现状态后创建了该组。</p> 
     <p>由于营销组下方已存在营销通信和品牌子组，因此当发生此情况时，它们不会继承已解锁的发现状态。</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">当管理员锁定更高级别的状态时</td> 
   <td> <p>当Workfront管理员锁定系统级别的状态时，您的组会继承该状态以及系统中的所有其他组。</p> <p>同样，当管理员锁定组上方某组的状态时，您的组会继承该状态以及较高组下方的任何其他子组。</p> <p><b>注意</b>:之后，如果管理员在系统级别或组上方的组中解锁其中一种状态，则您的组将保留之前继承的状态。 现在，它是状态的单独版本，您可以仅为组自定义它。</p> 
    <p><b>示例：</b></p>
    <p>营销组管理员锁定上述发现状态，以确保所有3个子组都具有该状态。</p> 
    <p>与您的广告组一起，营销通信和品牌推广组现在具有发现状态。 当它被锁定在其上方的营销群组中时，他们会继承它。</p> 
    <p>然后，营销组管理员将解锁发现状态，以便所有3个子组都具有自己的发现状态版本。 现在，您和其他2个组的管理员可以自定义发现状态以满足您组的需求。</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">管理员删除群组时</td> 
   <td> <p>当管理员删除组并选择您的组在系统中的位置时，如果已删除的组中不存在自定义状态，则组会继承这些状态。</p> 
   <p><b>示例： </b></p>
     <p>名为“消息”的组需要与您的广告组合并，因此Workfront管理员会删除“消息”组并选择您的组来替代它。</p> 
     <p>消息传送组具有名为“正在处理”的唯一状态。 您的广告组现在具有可用的状态。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## 继承状态配置

创建顶级组时，它会从系统级别继承以下配置。 在创建子组时，它会从下一个较高的组中继承以下配置。

* 默认状态配置

   有关这些内容的信息，请参阅 [使用自定义状态作为默认状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* 状态显示订单配置

   有关这些内容的信息，请参阅 [重新排序系统级别和组状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

如果在创建组后有人更改了这些配置，则其状态不会受到影响。
