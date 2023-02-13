---
title: 访问系统问题状态列表
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: 您可以使用问题的状态向系统中的用户显示给定时间的问题在开发阶段的哪个阶段。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# 访问系统问题状态列表

您可以使用问题的状态向系统中的用户显示给定时间的问题在开发阶段的哪个阶段。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 访问问题状态

您可以访问和修改系统级别的问题状态。 您可以编辑有关默认系统状态的一些信息，也可以创建新的自定义状态。 有关创建自定义状态或编辑系统状态的更多信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

要访问系统级别的问题状态，请执行以下操作：

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **项目首选项** > **状态**.

1. 单击 **问题** 选项卡，以查看Workfront中可用的问题状态。

   ![](assets/issue-status.png)

## 系统问题状态

Workfront具有10个原始问题状态。 下表中的前4个是必需的，这意味着您可以解锁、重命名和重新排序它们，但无法隐藏或删除它们。

您可以添加自定义问题状态，以满足贵组织的需求。 有关更多信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

对于用户，更改问题状态通常是手动过程。 但是，当问题状态根据系统中发生的其他因素自动更改时，可能会出现下面列表中所述的情况。

随Workfront实例提供了以下问题状态：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>系统问题状态</th> 
   <th>如何使用状态</th> 
   <th>状态中会发生什么情况</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>新（必需状态）</td> 
   <td>这是每个新创建问题的默认状态。</td> 
   <td>如果某个项目的问题处于“当前”状态，则该问题会显示在分配给该问题的用户的“工作请求”选项卡中。 用户现在可以开始处理此问题。</td> 
  </tr> 
  <tr> 
   <td>正在进行（必需状态）</td> 
   <td> <p>您可以在此状态中放置一个问题，以指示该问题的工作已开始。</p> <p>如果问题的解决方式与另一个对象（任务、项目或其他问题）连接，则当将解决对象的状态更改为“进行中”时，问题状态将自动更改为“进行中”。 </p> <p>有关解析对象的更多信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
   <td> <p>如果某个项目的问题处于“当前”状态，则该问题会显示在分配给该问题的用户的“工作”选项卡中。</p> <p>当问题正在进行时，该问题会显示实际开始日期的值。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>已关闭（必需状态）</td> 
   <td> <p>您可以在问题完成后将其手动标记为已关闭。 </p> <p>如果问题的解决方式与另一个对象（任务、项目或其他问题）连接，则当将解决对象的状态更改为“已关闭”时，问题状态将自动更改为“已关闭”。</p> <p>有关解析对象的更多信息，请参阅 <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">解析和可解析对象概述 </a>.</p> </td> 
   <td> <p>当问题关闭时，该问题将从被分派人的工作列表中删除。 在这种情况下，问题会显示实际完成日期的值。 </p> <p>当项目的所有任务都完成并且问题都关闭时，项目就可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>暂挂（必需状态）</td> 
   <td> <p>您可以手动将问题标记为“暂挂”，以指示完成问题存在延迟。 </p> </td> 
   <td> <p>如果某个项目的问题处于“当前”状态，则该问题会显示在分配给该问题的用户的“工作”选项卡中。 </p> <p>当项目上的所有任务都已完成，但项目上至少存在一个“暂挂”问题时，无法完成项目。 </p> </td> 
  </tr> 
  <tr> 
   <td>重新打开（等于正在进行）</td> 
   <td> <p>在此状态下，您可能会放置一个问题，以指明在问题之前关闭时该问题的工作尚未完成，需要重新打开该问题才能完成工作。</p> </td> 
   <td> <p>如果某个项目的问题处于“当前”状态，则该问题会显示在分配给该问题的用户的“工作请求”选项卡中。 用户现在可以开始处理此问题。</p> <p>此状态在报表中很重要，可区分首次打开的问题（通常处于“新建”状态）和之前关闭后打开的问题（通常处于“重新打开”状态）。 </p> </td> 
  </tr> 
  <tr> 
   <td>等待反馈（等于暂挂）</td> 
   <td>在此状态中，您可能会提出问题，以表明您正在等待反馈（通常来自主联系人），然后才能继续处理问题。 </td> 
   <td> <p>如果某个项目的问题处于“当前”状态，则该问题会显示在分配给该问题的用户的“工作”选项卡中。</p> <p>如果问题“正在等待反馈”，则无法完成项目。</p> <p>此状态在报告中很重要，可区分当前打开但正在处理的问题（通常处于“进行中”状态）和当前打开但未处理的问题，因为完成这些问题需要更多反馈（通常处于“等待反馈”状态）。</p> </td> 
  </tr> 
  <tr> 
   <td>不能复制（等于关闭）</td> 
   <td>在此状态下，您可能会放置一个问题，以指示您正在关闭该问题，但是您看不到触发打开该问题的问题。 问题可能仍然存在，但在给定时间无法复制。 </td> 
   <td> <p>此状态在报告中很重要，它区分已完成的问题和已解决的问题（通常处于“已关闭”状态）以及在给定时间（通常处于“无法复制”状态）不可见的问题。</p> <p>将问题标记为无法复制时，该问题将从被分派人的工作列表中删除。 在这种情况下，问题会显示实际完成日期的值。</p> <p>如果项目上的所有任务都已完成，并且某些问题处于“无法复制”状态，则项目可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>已解决（等于关闭）</td> 
   <td>您可能会在此状态中放置一个问题，以指示您正在关闭该问题，并且创建该问题的问题已实际解决。</td> 
   <td> <p>此状态在报告中非常重要，可区分通过或不通过决议而关闭的问题（通常处于“已关闭”状态）和通过实际决议而关闭的问题（通常处于“已解决”状态）。</p> <p>将问题标记为“已解决”后，该问题将从被分派人的“工作”列表中删除。 在这种情况下，问题会显示实际完成日期的值。</p> <p>如果项目上的所有任务都已完成，并且至少有一个问题处于“已解决”状态，则项目可以完成。 </p> </td> 
  </tr> 
  <tr> 
   <td>已验证完成（等于关闭）</td> 
   <td>在此状态中，您可能会放置一个问题，以表示您正在关闭该问题，并且您已验证生成该问题的问题已得到解决。</td> 
   <td> <p>将问题标记为“已验证完成”(Verified Complete)后，该问题将从被分派人的“工作进程”(Working On)列表中移除。 在这种情况下，问题会显示实际完成日期的值。</p> <p>如果项目上的所有任务都已完成，并且某些问题处于“已验证的完成”状态，则项目可以完成。</p> </td> 
  </tr> 
  <tr> 
   <td>无法解决（等于关闭）</td> 
   <td>在此状态中，您可能会放置一个问题，以指示您正在关闭该问题，但生成该问题的问题无法解决。</td> 
   <td> <p>此状态在报告中非常重要，可区分通过或未通过决议而关闭的问题（通常处于“已关闭”状态）和未通过实际决议而关闭的问题（通常处于“不解决”状态）。</p> <p>当问题标记为“不解决”时，该问题将从被分派人的“工作”列表中删除。 在这种情况下，问题会显示实际完成日期的值。</p> <p>如果项目上的所有任务都已完成，并且至少有一个问题处于“无法解决”状态，则项目可以完成。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义问题状态

Workfront管理员可以向Workfront添加系统级别和组级别的问题状态，并更改用户看到这些状态的顺序。 有关更多信息，请参阅 [创建或编辑状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

群组管理员可以添加特定于一个群组的自定义状态。 有关更多信息，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
