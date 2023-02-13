---
title: 使用布局模板自定义用户界面术语
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员，您可以使用布局模板来更改Workfront中显示的某些对象的标签，以匹配您组织中使用的术语。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# 使用布局模板自定义用户界面术语

作为Adobe Workfront管理员，您可以使用布局模板来更改Workfront中显示的某些对象的标签，以匹配您组织中使用的术语。

在保存您更改了术语的布局模板后，再次从Workfront中注销并重新登录后，您更改的标签即会显示在默认标签显示在整个Workfront的大多数区域中的位置：

* 主菜单
* 从主菜单访问的所有区域
* 所有选项卡
* 所有菜单
* Report Builder和报表元素（视图、过滤器和分组）
* 保存按钮
* 导出的文件
* 电子邮件
* 移动设备应用程序

>[!NOTE]
>
>* Outlook加载项区域不显示自定义标签。
>* 在自定义标签时，您可能会遇到语法和其他问题。 例如，如果将“Issue”更改为“Request”，则UI中可能会有一些位置显示短语“An request”。 有关更多信息，请参阅 [自定义对象名称的含义](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) 在文章中 [了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问权限级别。
要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>:如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义用户界面术语

1. 开始使用布局模板，如 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击 **设置术语** 在页面的右上角附近。
1. 执行以下任一操作：

   * 要使用Workfront提供的替代术语，请单击向下箭头  ![](assets/dropdown-arrow.png) 在标签旁边，单击下拉列表中所需的替代标签。

      >[!NOTE]
      >
      >对于非英语语言的本地化版本的Workfront，支持下拉列表中提供的替代标签。

   * 要为对象显示的标签提供您自己的自定义替代方法，请单击 **设置自定义名称** 在标签的右侧，然后键入 **奇异** 和 **复数** 自定义术语的形式。 您可以单击 **重置** 如果你改变主意了。

      您可以自定义以下对象名称：

      <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront对象</p></td>
        <td>
          <p>项目组合</p>
          <p>项目群</p>
          <p>项目</p>
          <p>任务</p>
          <p>问题</p>
          <p>目标</p>
          <p>结果</p>
          <p>活动</p>
         </ul></td>
        <td><p>有关这些对象的更多信息，请参阅 <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront目标对象</p></td>
        <td>
         <ul>
          <p>目标</p>
          <p>结果</p>
          <p>活动</p>
         </ul></td>
        <td><p>这些对象需要附加许可证。 有关更多信息，请参阅 <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目标概述</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront方案规划器对象</p></td>
        <td>
         <ul>
          <p>计划</p>
          <p>方案</p>
          <p>计划 </p>
         </ul></td>
        <td><p>这些对象需要附加许可证。 有关信息，请参阅 <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">方案规划器入门</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. 完成后，单击 **完成**.

   >[!TIP]
   >
   >单击完成（甚至在保存布局模板之后）后，您始终可以返回到“设置术语”设置，然后单击任何自定义术语旁边的重置，以将它们恢复为默认状态。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **保存**.

1. 要查看术语更改，请执行以下操作：

   1. 注销，然后重新登录Workfront。
   1. 关闭您为Workfront环境打开的所有浏览器选项卡。

   >[!IMPORTANT]
   >
   >在对术语进行更改之前，使用布局模板的任何人也需要使用此功能。

有关布局模板的更多信息，请参阅 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
