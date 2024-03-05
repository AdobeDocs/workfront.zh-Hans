---
title: 使用布局模板自定义新主页
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 您可以使用布局模板配置用户在打开新主页时看到的内容。
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: 2551089a20d3301ff1cf7dd633114dbb5235e959
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 1%

---

# 使用布局模板自定义新主页

您可以使用布局模板配置用户在打开新主页时看到的内容。

您可以配置：

* 默认情况下，工作区中显示哪些构件，以及它们在页面上的布局
* 选择哪个背景
* 特定构件设置，包括哪些筛选器和组可用于“我的项目”、“我的任务”和“我的问题”构件及其默认值

>[!IMPORTANT]
>
>本页中介绍的管理员布局模板选项将覆盖单个用户的自定义选项。
>
>在保存对布局模板所做的更改后，该布局模板上的用户将会更改其新主页以匹配布局模板，并且其现有的构件选择将推送到页面底部。 虽然管理员选择的构件可以由用户重新定位并调整大小，但无法删除它们。

有关新主页的信息，请参见 [新主页入门](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

有关创建布局模板的信息，请参阅 [创建和管理布局模板](../use-layout-templates/create-and-manage-layout-templates.md).

有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关为用户分配布局模板的信息，请参阅 [将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。
要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 使用布局模板自定义新主页

1. 开始使用布局模板，如中所述 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. 单击向下箭头 ![](assets/dropdown-arrow.png) 下 **自定义用户查看内容**，然后单击 **主页工作区**.

1. 在右侧显示的选项卡中，单击 **设计和布局** 选择并排列小部件和背景，或者 **构件设置** 用于管理单个小组件的设置，如可用过滤器和组。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">设计和布局</td> 
      <td>
      <p>选择用户工作区中将显示哪些小部件、这些小部件的位置，并选择背景。 请注意，虽然用户无法删除选定的构件，但可以随意移动和调整其大小以及添加其他构件。</p>
      <p>此选项卡基本上可用作小型的新Home工作区；因此，可以根据中所述的步骤对其进行自定义 <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">在新主页中添加、编辑或删除构件</a>. 选择小组件并根据用户需要安排工作区。</p>
      <p>要更改背景，请执行以下步骤 <b>后台自定义</b> 在 <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">新主页入门</a>.</p>
      <p>

>[!NOTE]
>
>只有在布局模板中移动小组件或调整其大小才会触发用户的新主页更新其布局。 但是，添加或删除构件将触发对用户页面的更新。

</p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">构件设置</td> 
      <td>
      <p>更改单个小部件的设置。 目前，仅支持三个小组件：</p>
      <ul>
        <li>我的项目</li>
        <li>我的任务</li>
        <li>我的问题</li>
      </ul>
      <p>选择想要编辑的小组件后，右侧将显示可用选项。 这些选项包括 <b>过滤器</b>， <b>列</b>、和 <b>组</b>. 您可以：</p>
      <ul>
      <li><p><b>选择用户可用的筛选器、列或组：</b></p>
      <p>选中您希望用户能够使用的列表中所有选项旁边的框。 对于用户，不会显示未勾选的选项。</li></p>
      <li><p><b>为构件设置默认筛选器或组：</b></p>
      <p>将鼠标悬停在某个选项上，将显示一个按钮，允许您将该选项设置为用户的默认选项。 当前的默认页面右侧将显示一个蓝色的“默认”标记。</li></p>
      <li><p><b>将现有的筛选器、列或组添加到可用选项列表中：</b></p>
      <p>单击每个列表底部的加号按钮，在该列表中添加一个选项。 请注意，只能通过这种方式添加现有筛选器、字段（用于列）或组。</p></li>
      </ul>
      <p>

>[!NOTE]
>
>如果使用布局模板为特定构件设置默认过滤器或分组，则由于现有用户偏好设置，该过滤器或分组可能不会立即生效。 要立即应用新过滤器或分组，您或用户可能需要通过在其URL的末尾附加“/resetUser”来重置其用户偏好设置。

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存** 左下角。

