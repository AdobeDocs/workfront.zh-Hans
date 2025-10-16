---
title: 使用布局模板自定义用户界面术语
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 作为Adobe Workfront管理员，您可以使用布局模板更改显示在Workfront中的某些对象的标签，以匹配您在组织中使用的术语。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 3%

---

# 使用布局模板自定义用户界面术语

作为Adobe Workfront管理员，您可以使用布局模板更改显示在Workfront中的某些对象的标签，以匹配您在组织中使用的术语。

在保存更改了术语的布局模板，然后注销Workfront并重新登录后，您更改的标签将显示在Workfront大多数区域默认标签的位置：

* 主菜单
* 从主菜单访问的所有区域
* 所有选项卡
* 所有菜单
* Report Builder和报告元素（视图、过滤器和分组）
* 保存按钮
* 导出的文件
* 电子邮件
* 移动应用程序

>[!NOTE]
>
>* Outlook加载项区域不显示自定义标签。
>* 在自定义标签时，您可能会遇到语法和其他问题。 例如，如果将“问题”更改为“请求”，则在UI中可能会有这样一些地方，您会看到短语“请求”。 有关详细信息，请参阅[了解Adobe Workfront中的对象](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names)一文中的[自定义对象名称的含义](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

有关布局模板的更多信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。

有关组的布局模板的信息，请参阅[创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)。

配置布局模板后，必须将其分配给用户，以使您所做的更改对其他人可见。 有关将布局模板分配给用户的信息，请参阅[将用户分配给布局模板](../use-layout-templates/assign-users-to-layout-template.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront包</td> 
   <td><p>任何</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td><p>标准</p>
       <p>规划</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>要在系统级别执行这些步骤，您需要系统管理员访问级别。</p>
        <p>要为组执行这些操作，您必须是该组的经理。</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 自定义用户界面术语

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 单击页面右上角附近的&#x200B;**设置术语**。
1. 执行以下任一操作：

   * 要使用Workfront提供的替代术语，请单击标签旁边的向下箭头![向下箭头](assets/dropdown-arrow.png)，然后在下拉列表中单击所需的替代标签。

     >[!NOTE]
     >
     >非英语本地化的Workfront版本支持下拉列表中提供的替代标签。

   * 要为对象显示的标签提供您自己的自定义替代项，请单击标签右侧的&#x200B;**设置自定义名称**，然后键入自定义项的&#x200B;**单数**&#x200B;和&#x200B;**Plural**&#x200B;形式。 如果您改变主意，可以单击&#x200B;**重置**。

     您可以自定义以下对象名称：

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront对象</p></td>
        <td>
          <p>组合</p>
          <p>项目群</p>
          <p>项目</p>
          <p>任务</p>
          <p>问题</p>
          <p>目标</p>
          <p>结果</p>
          <p>活动</p>
         </ul></td>
        <td><p>有关这些对象的详细信息，请参阅<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">了解Adobe Workfront中的对象</a>。</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront目标对象</p></td>
        <td>
         <ul>
          <p>目标</p>
          <p>结果</p>
          <p>活动</p>
         </ul></td>
        <td><p>这些对象需要额外的许可证。 有关详细信息，请参阅<a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront目标概述</a>。</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scenario Planner对象</p></td>
        <td>
         <ul>
          <p>计划</p>
          <p>方案</p>
          <p>规划 </p>
         </ul></td>
        <td><p>这些对象需要额外的许可证。 有关信息，请参阅<a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Scenario Planner入门</a>。</p></td>
       </tr>
      </tbody>
     </table>

1. 完成后，单击&#x200B;**完成**。

   >[!TIP]
   >
   >单击“完成”（甚至在保存布局模板后）后，您始终可以返回“设置术语”设置，然后单击任何自定义术语旁边的“重置”(Reset)，以将它们返回到默认状态。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击&#x200B;**保存**。

1. 要查看术语更改，请执行以下操作：

   1. 注销并重新登录Workfront。
   1. 关闭您已为Workfront环境打开的所有浏览器选项卡。

   >[!IMPORTANT]
   >
   >在您更改术语之前，使用该布局模板的任何用户也需要此权限。

有关布局模板的更多信息，请参阅[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)。
