---
title: 创建或编辑状态
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: 作为Adobe Workfront管理员，您可以为项目、任务和问题创建自定义状态。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 2%

---

# 创建或编辑状态

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

作为Adobe Workfront管理员，您可以为项目、任务和问题创建自定义状态。 这些权限可以适用于整个Workfront系统中的用户，也可以适用于特定组或子组。 有关状态的更多信息，请参阅 [状态概述](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>群组管理员还可以创建自己的群组状态，以便仅供其群组使用。 有关更多信息，请参阅 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

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

## 创建或编辑自定义状态

您可以添加自定义状态，以供整个组织或单个群组使用。

在为整个组织创建自定义状态时，您可以对其进行配置，以便系统中的所有组都可以使用该状态，而无需对其进行编辑。 或者，您也可以对其进行配置，以便群组管理员可以为其群组修改它，如 [创建或编辑群组状态](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 在左侧面板中，单击 **项目首选项** > **状态**.

1. （视情况而定）如果您正在创建或编辑状态以供系统范围使用，请确保 **系统状态** 框中，将选定此变量。

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   或

   如果状态是组或子组的状态，请开始在右上角键入组的名称，然后在显示时选择该名称。

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. 选择对象类型的选项卡(**项目**, **任务**&#x200B;或 **问题**)。

1. 如果要创建新状态，请单击 **添加新状态**.

   或

   如果您正在编辑现有状态，请将鼠标悬停在该状态上，然后单击 **编辑** 图标。

   ![](assets/custom-status-edit.png)

1. 使用以下选项配置状态：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">状态名称</td> 
      <td> <p>键入状态名称。 这是必填字段。</p> <p>在创建状态名称时，请注意，系统中的其他人可以创建具有相同名称的状态。 我们建议使用唯一的名称，以避免在Workfront中选择状态时造成混淆。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">描述</td> 
      <td>（可选）键入状态描述。 这会向使用者传达其目的。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">颜色</td> 
      <td> <p>通过单击颜色字段并从色板面板中选择颜色来自定义状态的颜色。 您还可以在字段中输入十六进制数。</p> <p>当用户查看对象时，状态颜色显示在Workfront的右上角。</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">等于</td> 
      <td> <p>从列表中选择一个最能描述状态函数的选项。 例如，如果状态名称为“完成”，则与其等同的选项应为“完成”。</p> <p>每个状态都必须等同于其中一个选项，因为这决定了状态的工作方式。</p> <p>创建状态后，无法修改此选项。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">密钥</td> 
      <td> <p>如果要创建新状态，请键入状态的代码或缩写，或使用为您生成的代码或缩写。 此键值在Workfront中必须唯一，因为它可用于报告目的。 如果尝试指定系统中已在使用的键，则该字段将变为红色。</p> <p>使用缩写时可能会有所帮助，该缩写对于使用缩写的用户而言是可识别的。</p> <p>创建状态后，无法修改此选项。</p> <p>您不能更改“计划”、“当前”和“完成”状态的关键代码。 如果您以文本模式生成报表，则务必要这样做。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">隐藏状态</td> 
      <td> <p>（仅限项目和任务状态）</p> <p>如果希望对用户隐藏状态，请启用此选项。 禁用该设置（默认设置）后，系统中的所有用户都可以使用该状态。</p> <p>您可以通过禁用所有4种问题类型（错误报表、更改顺序、问题、请求）来隐藏问题状态。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">锁定所有群组</td> 
      <td>
       <p>锁定状态后，系统中的用户可以查看和使用该状态，组管理员无法为其组自定义该状态。</p> 
       <p>解锁状态后，群组管理员可以针对其各个群组自定义该状态。</p>

   <div>
       <p>您可以在系统批准过程中同时使用锁定状态和已解锁状态。 如果创建具有已解锁系统状态的系统批准流程，则整个系统的用户可以将批准流程附加到系统中的任何项目、任务或问题。</p>
       <p> 在以下情况下，会显示警告消息，以帮助您和您的用户了解解锁状态的结果：</p>
       <ul>
       <li>管理员解锁在批准流程中使用的系统级别状态。 出现一条消息，警告可能会删除其组的已解锁状态，这将阻止组成员正确使用分配给其组的对象的批准流程。</li>
       <li>用户开始编辑使用已解锁状态的批准流程。 系统会显示一条消息，提醒用户已解锁状态，以便用户评估重新锁定或替换该状态是否是个好主意。</li>
       <li>在对象上附加具有解锁状态的系统级批准进程，并删除分配给该对象的组的状态。 当组成员转到对象的“批准”部分时，将显示一条消息，说明无法为对象启动批准流程。</li>
       </ul>
       <p>有关锁定状态的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">锁定和解锁的系统级别状态</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**保存**。

   有关将此状态设为默认状态的说明，请参阅 [使用自定义状态作为默认状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

有关重新排序组状态的信息，请参阅 [重新排序系统级别和组状态](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
