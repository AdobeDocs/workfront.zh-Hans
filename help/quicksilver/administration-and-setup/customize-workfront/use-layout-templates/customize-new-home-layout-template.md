---
title: 使用布局模板自定义新主页
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 您可以使用布局模板配置用户在打开新主页时看到的内容。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 7bae31a9454c88bd0e5525f4b4d11cd9e76ccd39
workflow-type: tm+mt
source-wordcount: '827'
ht-degree: 1%

---

# 使用布局模板自定义新主页

您可以使用布局模板配置用户首次打开新主页时看到的内容。

您可以配置：

* 默认情况下，工作区中显示哪些构件
* 选择哪个背景
* 特定构件设置，包括哪些筛选器和组可用于“我的项目”、“我的任务”和“我的问题”构件及其默认值

>[!IMPORTANT]
>
>应用布局模板后，最终用户能够更改其背景并在页面上重新排序小组件。 他们无法删除Workfront管理员包含的小部件。
> <br>
>管理员能够为用户添加新构件。 但是，如果最终用户已经自定义了其小组件顺序或后台选择，则这些特定自定义不会更改。



有关新主页的信息，请参阅[开始使用新主页](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md)。

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

## 使用布局模板自定义新主页

要使用布局模板自定义“新建主页”，请执行以下操作：

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。

1. 单击&#x200B;**自定义用户看到的内容**&#x200B;下的向下箭头![](assets/dropdown-arrow.png)，然后单击&#x200B;**主页Workspace**。

1. 在右侧显示的选项卡中，单击&#x200B;**设计和布局**&#x200B;以选择和排列小部件和背景，或单击&#x200B;**小部件设置**&#x200B;以管理单个小部件的设置，如可用的筛选器和组。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">设计和布局</td> 
      <td>
      <p>选择用户工作区中将显示哪些小部件、这些小部件的位置，并选择背景。 请注意，虽然用户无法删除选定的构件，但可以随意移动和调整其大小以及添加其他构件。</p>
      <p>此选项卡基本上可用作小型的新主页工作区；因此，可以根据<a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">新主页中添加、编辑或删除小组件</a>中描述的步骤对其进行自定义。 选择小组件并根据用户需要安排工作区。</p>
      <p>要更改背景，请按照<a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">开始使用新主页</a>中的<b>背景自定义</b>下的步骤操作。</p>
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
      <p>选择想要编辑的小组件后，右侧将显示可用选项。 这些选项包括<b>筛选器</b>、<b>列</b>和<b>组</b>。 您可以：</p>
      <ul>
      <li><p><b>选择并排序可供用户使用的筛选器、列或组：</b></p>
      <p>选中您希望用户能够使用的列表中所有选项旁边的框。 这些选项不会扩展到“摘要”面板。 您必须在布局模板的“摘要”选项卡中配置该区域。 对于用户，不会显示未勾选的选项。 拖放列表中的选项以设置顺序。</li></p>
      <p>

>[!IMPORTANT]
>
>用户必须至少具有视图的“创建”访问权限，管理员列配置才能正确应用于其新主页。

</p>
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

   如果您已完成自定义，请单击左下角的&#x200B;**保存**。

>[!IMPORTANT]
>
>必须刷新新主页才能查看布局模板中的自定义项。
