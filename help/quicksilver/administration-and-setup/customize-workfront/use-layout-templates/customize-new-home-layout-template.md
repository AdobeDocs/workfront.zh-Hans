---
title: 使用布局模板自定义主页
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 您可以使用布局模板配置用户在Adobe Workfront中打开主页时看到的内容。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '853'
ht-degree: 1%

---

# 使用布局模板自定义主页

您可以使用布局模板配置用户首次打开主页时看到的内容。

您可以配置：

* 默认情况下，工作区中显示哪些构件
* 选择哪个背景
* 特定构件设置，包括哪些筛选器和组可用于“我的项目”、“我的任务”和“我的问题”构件及其默认值

>[!IMPORTANT]
>
>应用布局模板后，最终用户能够更改其背景并在页面上重新排序小组件。 他们无法删除Workfront管理员包含的小部件。
> 
>管理员能够为用户添加新构件。 但是，如果最终用户已经自定义了其小组件顺序或后台选择，则这些特定自定义不会更改。

有关主页的信息，请参阅[主页入门](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md)。

有关创建布局模板的信息，请参阅[创建和管理布局模板](../use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关将布局模板分配给用户的信息，请参阅[将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

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
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td><p>新增：标准</p>
  <p> 当前：计划</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。
要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

*有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用布局模板自定义主页

要使用布局模板自定义主页，请执行以下操作：

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。

1. 单击&#x200B;**自定义用户看到的内容**&#x200B;下的向下箭头![](assets/dropdown-arrow.png)，然后单击&#x200B;**主页Workspace**。

1. 在右侧的选项卡中，单击下列选项之一：

   * **设计和布局**：选择以选择和排列小部件和背景
   * **构件设置**：选择此项可管理单个构件的设置，如可用的筛选器和组。

   下表包含有关每个选项卡的详细信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">设计和布局</td> 
      <td>
      <p>选择将在用户的工作区中显示哪些小部件、其位置并选择背景。</p> 
      <p>请注意，虽然用户无法删除选定的构件，但他们可以随意移动这些构件并调整其大小。 他们还可以添加更多构件。</p>
      <p>此选项卡的主要功能是预览具有此布局模板的用户将体验的实际主页工作区。</p> 
      <p> 执行以下任一操作： </p>
      <ul><li>根据<a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">在主页</a>中添加、编辑或删除构件中描述的步骤自定义此选项卡。 </li>
      <li>选择小组件并根据用户需要安排工作区。</li>
      <li>要更改背景，请按照<a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">开始使用主页</a>中的<b>背景自定义</b>下的步骤操作。</li></p>
      <p>

   >[!NOTE]
   >
   >只有在布局模板中移动小组件或调整其大小才会触发用户的主页更新其布局。 但是，添加或删除构件将触发对用户页面的更新。

   </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">构件设置</td> 
      <td>
      <p>更改单个小部件的设置。</p> 
      <p>

   >[!NOTE]
   >
   >这些选项不会扩展到“摘要”面板。 您必须在布局模板的“摘要”选项卡中配置该区域。

   </p>
      <p> 从左侧列表中的以下构件中选择：</p>
      <ul>
        <li>我的项目</li>
        <li>我的任务</li>
        <li>我的问题</li>
      </ul>
      <p>选择想要编辑的小部件后，选择要在右侧用于主页的<b>筛选器</b>、<b>列</b>和<b>组</b>。</p>
      <p> 您可以：</p>
      <ul>
      <li><p>通过选中列表中选项旁边的复选框，选择用户可用的筛选器、列或组并对它们进行排序。 对于用户，不会显示未勾选的选项。</p></li>
      <li> <p>拖放列表中的选项以设置顺序。</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* 筛选器、列和组选项链接到布局模板中的列表自定义选项。 此处所做的更改也将应用于这些设置。
   >* 用户必须至少具有视图的“创建”访问权限，管理员列配置才能正确应用于其主页。

   </p>
      <li><p>将鼠标悬停在某个选项上，然后单击<b>设置为默认值</b>，为构件设置默认筛选器或组。 当前默认值在其右侧显示蓝色<b>默认</b>徽章。</p></li>
      <li><p>单击每个列表底部的加号按钮，将现有的筛选器、列或组添加到可用选项列表中，以向该列表中添加选项。 请注意，只能通过这种方式添加现有筛选器、字段（用于列）或组。</p></li>
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

   如果您已完成自定义，请单击左下角的&#x200B;**保存**。

   >[!IMPORTANT]
   >
   >用户必须刷新其主页才能查看布局模板中的自定义项。
