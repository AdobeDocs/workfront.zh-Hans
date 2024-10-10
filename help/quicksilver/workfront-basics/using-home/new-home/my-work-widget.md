---
product-area: home
navigation-topic: use-the-home-area
title: 使用“我的工作”小组件管理您的工作
description: “我的工作”小组件将所有已分配的任务、问题和请求显示在一个位置。 在这里，您可以筛选和组织您的工作，记录时间，进行更新，并将工作项标记为完成。
author: Courtney
feature: Get Started with Workfront
source-git-commit: 7b3658e2f13ea75cd7ae09cb7c3486dfc4a0bdb3
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 5%

---


# 使用“我的工作”小组件管理您的工作

“我的工作”小组件将所有已分配的任务、问题和请求显示在一个位置。 在这里，您可以筛选和组织您的工作，记录时间，进行更新，并将工作项标记为完成。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证</strong></td> 
   <td> <p>当前：Contribute</p>
   <p>或</p> 
   <p>新：[！UICONTROL Light]或更高版本<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL视图]或更高的项目、任务、问题和文档访问权限</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>您需要处理的任务和问题的Contribute权限或更高版本</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查找使用过滤器的工作

您可以微调“我的工作”筛选器以重点关注工作列表中的特定项目：

![](assets/filter-my-work-widget.png)

### 筛选器详细信息

<table>
  <tbody>
    <tr>
      <td>正在处理</td>
      <td>显示您当前处理的项目</td>
    </tr>
    <tr>
      <td>准备开始</td>
      <td>显示项目和 
      <ul>
      <li>没有未完成的前置任务或任务限制</li>
      <p>和</p>
      <li>计划开始日期是过去的日期，或者最多在未来的两周内</li>
      </ul>
      </td>
    </tr>
    <tr>
      <td>未就绪</td>
      <td>显示具有
       <ul>
      <li>未完成的前置任务或阻止处理项目的任务限制</li>
      <p>或</p>
      <li>超过两周后的计划开始日期</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>已请求</td>
      <td>显示您尚未开始处理的问题</td>
    </tr>
    <tr>
      <td>已由我委派</td>
      <td>显示已委派给其他用户的项目</td>
    </tr>
    <tr>
      <td>已委派给我</td>
      <td>显示用户委派给您的项目</td>
    </tr>
    <tr>
      <td>已完成</td>
      <td>显示过去两周内完成的工作。 此筛选器选项不包括审批。</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>如果您要查找更具体的过滤选项，可以使用“我的任务”或“我的问题”小组件。 有关“我的任务”和“我的问题”筛选器的详细信息，请参阅[新建主页小部件筛选器概述](/help/quicksilver/workfront-basics/using-home/new-home/widget-filter-overview-new-home.md)。

## 组织您的工作

您可以使用我的工作小组件的排序和分组功能以对您有意义的方式组织您的工作。

### 排序

您可以对工作列表进行排序

* 到期日期
过期项目在日期旁边显示一个警告图标。 Workfront使用规划完成日期来确定任务和问题是否已过期。
* 名称
* 完成百分比
* 状态

>[!TIP]
>
>要创建在“我的工作”小部件的顶部显示所有过期项目的列表，请按照“到期日期”排序，并且不应用分组。


![](assets/sort-my-work-widget.png)

### 组

您可以将工作列表分组为

* 项目
* 状态
* 到期日期
到期日期由计划完成日期确定。

>[!NOTE]
>
>应用分组时，您在“排序”菜单中的选择将决定分组内的顺序。


![](assets/group-my-work-widget.png)

## 更新摘要中的工作项信息

您可以打开“摘要”面板以快速更新任务或问题中的信息。 在摘要中，您可以

* 更新完成百分比
* 添加更新
* 导航到文档区域以上传文档
* 查看工作项详细信息和更新自定义字段
Workfront管理员可以自定义哪些字段显示在布局模板的摘要中。 有关详细信息，请参阅[使用布局模板自定义主页和摘要](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。
* 更改工作项状态
* 查看子任务
* 记录时间
* 查看附加的审批流程

要打开“摘要”，请将鼠标悬停在工作项上，然后单击&#x200B;**摘要**&#x200B;图标![](assets/open-summary-new-home.png)。

有关如何使用摘要面板的其他信息，请参阅[摘要概述](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)。

## 使用快速操作更新工作项

您可以使用快速操作菜单执行以下操作

* 记录时间
* 添加更新
* 更新自定义表单
* 上传文件

要找到快速操作菜单，请将鼠标悬停在工作项上。 快速操作列表显示在&#x200B;**处理它**&#x200B;或&#x200B;**完成**&#x200B;按钮附近。

![](assets/quick-actions-new-home.png)


## 查看审批和团队请求

审批和团队请求未显示在我的工作小部件中。 如果您定期处理审批和团队请求，我们建议您将以下构件添加到新主页：

* 我的审批
* 所有审批
* 团队请求

有关向新主页添加构件的信息，请参阅新主页中的[添加、编辑或删除构件](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md)。




