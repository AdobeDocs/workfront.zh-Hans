---
title: 使用布局模板自定义左侧面板
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 在布局模板中，您可以自定义用户在整个Adobe Workfront的左侧面板区域中看到的内容。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1102'
ht-degree: 0%

---

# 使用布局模板自定义左侧面板

<!--Audited: 10/2024-->

在布局模板中，您可以自定义用户在整个[!DNL Adobe Workfront]的左侧面板区域中看到的内容。

例如，您可以确定用户在查看任务时会在左侧面板中看到以下哪些项目：

![品牌左面板](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>对顺序和可见性所做的更改将反映在移动设备应用程序中。

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

## 自定义[!DNL Workfront]中某个区域的左侧面板：

1. 开始处理布局模板，如[创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)中所述。
1. 单击&#x200B;**[!UICONTROL 自定义用户看到的内容]**&#x200B;下的向下箭头![向下箭头](assets/dropdown-arrow.png)，然后单击要自定义其左侧面板的对象类型或[!DNL Workfront]区域的名称。

   下表列出了可自定义其左侧面板的对象类型和[!DNL Workfront]区域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>对象类型或[!DNL Workfront]区域</th> 
      <th>当用户单击以下内容时……</th> 
      <th>在布局模板中显示左侧面板中用户可查看的部分：</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[！UICONTROL项目]</td> 
      <td>项目的名称</td> 
      <td>[！UICONTROL任务]、[！UICONTROL项目详细信息]、[！UICONTROL业务案例]、[！UICONTROL更新]、[！UICONTROL文档]、[！UICONTROL问题]、[！UICONTROL风险]、[！UICONTROL批准]、[！UICONTROL基线]、[！UICONTROL记帐费率]、[！UICONTROL记帐记录]、[！UICONTROL uicontrol支出]、[！UICONTROL小时数]、[！UICONTROL工作负载均衡器]、[！UICONTROL人员]、[！UICONTROL利用率]、[！UICONTROL队列详细信息]、[！UICONTROL路由规则]、[！UICONTROL队列主题]、[！UICONTROL主题组]、[！UICONTROL量度]、[！UICONTROL规划]*</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL任务]</td> 
      <td>任务的名称</td> 
      <td> [！UICONTROL更新]、[！UICONTROL文档]、[！UICONTROL任务详细信息]、[！UICONTROL子任务]、[！UICONTROL问题]、[！UICONTROL小时数]、[！UICONTROL审批]、[！UICONTROL费用]、[！UICONTROL前置任务]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL问题]</td> 
      <td>问题的名称</td> 
      <td> [！UICONTROL更新]、[！UICONTROL文档]、[！UICONTROL问题详细信息]、[！UICONTROL小时数]、[！UICONTROL审批]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROLPortfolio]</td> 
      <td>项目组合的名称</td> 
      <td>[！UICONTROL项目]、[！UICONTROL项目]、[！UICONTROLPortfolio详细信息]、[！UICONTROLPortfolio]、[！UICONTROL优化]、[！UICONTROL文档]、[！UICONTROL更新]、[！UICONTROL规划]*</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL项目]</td> 
      <td>项目的名称</td> 
      <td>[！UICONTROL项目]、[！UICONTROL项目详细信息]、[！UICONTROL更新]、[！UICONTROL文档]、[！UICONTROL计划]*</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL模板]</td> 
      <td>项目模板的名称</td> 
      <td>[！UICONTROL模板任务]、[！UICONTROL模板详细信息]、[！UICONTROL更新]、[！UICONTROL文档]、[！UICONTROL风险]、[！UICONTROL费用]、[！UICONTROL人员]、[！UICONTROL批准]、[！UICONTROL计费率]、[！UICONTROL队列详细信息]、[！UICONTROL路由规则]、[！UICONTROL uicontrol队列主题]，[！UICONTROL主题组]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL模板任务]</td> 
      <td>模板任务的名称</td> 
      <td>[！UICONTROL更新]、[！UICONTROL文档]、[！UICONTROL模板任务详细信息]、[！UICONTROL子任务]、[！UICONTROL费用]、[！UICONTROL审批]、[！UICONTROL前置任务]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [！UICONTROL开票记录]</td> 
      <td>项目的开票记录名称</td> 
      <td>[！UICONTROL计费记录详细信息]、[！UICONTROL可计费小时数]、[！UICONTROL可计费费用]、[！UICONTROL固定收入]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL项目]</td> 
      <td>[！UICONTROL主菜单]中的项目<img src="assets/projects-in-main-menu.png"> <img src="assets/main-menu-icon.png"></td> 
      <td>[！UICONTROL项目]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL请求]</td> 
      <td>请求的名称</td> 
      <td>[！UICONTROL新请求]、[！UICONTROL提交的请求]、[！UICONTROL所有请求]、[！UICONTROL草稿]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL功能板]</td> 
      <td>仪表板的名称</td> 
      <td>[！UICONTROL我的仪表板]、[！UICONTROL共享仪表板]、[！UICONTROL所有仪表板]<p><b>注意</b>：如果您在[!DNL Adobe Workfront Classic]中使用布局模板为[！UICONTROL报告]区域创建了自定义选项卡，则这些选项卡将显示在此列表的底部。 对于用户，它们显示在左侧面板底部的[！UICONTROL功能板]区域。</p> </td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Scrum团队]</td> 
      <td>Scrum团队的名称</td> 
      <td><p>[！UICONTROL迭代]、[！UICONTROL当前迭代]、[！UICONTROL积压]、[！UICONTROL工作负载均衡器]、[！UICONTROL更新]、[！UICONTROL团队设置]</p> <p><strong>注意：</strong> <strong>[！UICONTROL当前迭代]</strong>项仅在迭代中至少有一个任务或问题时才会显示在左侧面板中。</p></td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Kanban团队]</td> 
      <td>Kanban团队的名称</td> 
      <td>[！UICONTROL工作负载均衡器]、[！UICONTROL Kanban board]、[！UICONTROL积压]、[！UICONTROL更新]、[！UICONTROL团队设置]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL Waterfall Team]</td> 
      <td>瀑布团队的名称</td> 
      <td>[！UICONTROL工作负载均衡器]、[！UICONTROL更新]、[！UICONTROL团队请求]、[！UICONTROL团队设置]</td> 
     </tr> 
     <tr> 
      <td>[！UICONTROL迭代]</td> 
      <td>迭代的名称</td> 
      <td>[！UICONTROL Stories]、[！UICONTROL Issues]、[！UICONTROL Story Board]、[！UICONTROL Overview]、[！UICONTROL Custom Forms]、[！UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   *贵公司必须额外购买Workfront Planning的许可证，以便能够将此区域添加到项目、项目组合和程序的左侧面板。 有关详细信息，请参阅[Adobe Workfront规划概述](/help/quicksilver/planning/general/planning-overview.md)


1. 在&#x200B;**[!UICONTROL 左侧面板]**&#x200B;列表中，执行以下任一操作来确定在左侧面板中您选择的[!DNL Workfront]区域或对象类型将看到的用户：

   * 单击&#x200B;**显示** ![显示图标](assets/add-secondary-nav-item.png)或&#x200B;**隐藏** ![隐藏图标](assets/delete-secondary-nav-item.png)以在左侧面板中显示或隐藏部分。 无法隐藏没有&#x200B;**显示**&#x200B;或&#x200B;**隐藏**&#x200B;图标的项目。

   * 拖动项目![移动图标](assets/move-icon---dots.png)以更改它们在左侧面板上的顺序。

   >[!NOTE]
   >
   >**[!UICONTROL 自定义用户看到的内容]**&#x200B;下拉列表中的以下项目引用了左侧面板以外的区域：
   >* [!UICONTROL 列表]
   >* [!UICONTROL 摘要面板]
   >* [!UICONTROL 主页]
   >* [!UICONTROL 品牌]
   > 
   >有关如何自定义其他区域的信息，请参阅以下文章：
   >
   >* [使用布局模板自定义筛选器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [使用布局模板自定义[!UICONTROL 摘要面板]](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [使用布局模板自定义主页](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* 使用布局模板[品牌Adobe [!DNL Workfront] ](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. （可选）如果要添加链接到贵组织某个功能板的左侧面板项，请单击&#x200B;**[!UICONTROL 添加自定义分区]**，为该项键入一个&#x200B;**[!UICONTROL 自定义分区标题]**，然后添加该功能板。

   仪表板项目显示在左侧面板的底部。 当用户将鼠标悬停在左侧面板中的仪表板项目旁边时，会看到您键入的自定义分区标题。

   >[!NOTE]
   >
   >用户可以将自定义功能板项目添加到他们自己的左侧面板。 在布局模板中添加自定义仪表板项目时，除了它们所添加的项目外，还会显示您的项目，而不会覆盖或重置这些项目。 如果将用户分配给具有自定义仪表板项目的新布局模板，也是如此。 有关用户如何自定义左侧面板的信息，请参阅[创建自定义选项卡或分区](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)。
   >
   >有关功能板的信息，请参阅[功能板](../../../reports-and-dashboards/dashboards/dashboards-overview.md)。

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击&#x200B;**[!UICONTROL 保存]**。

   >[!TIP]
   >
   >您可以随时单击&#x200B;[!UICONTROL **保存**]&#x200B;以保存进度（这将关闭布局模板编辑器），然后继续修改模板。
