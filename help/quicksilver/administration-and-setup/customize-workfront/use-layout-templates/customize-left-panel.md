---
title: 使用布局模板自定义左侧面板
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: 在布局模板中，您可以自定义用户在整个Adobe Workfront的左侧面板区域中看到的内容。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c0b0102eb1e1f45e794f962f7e905349f9e241eb
workflow-type: tm+mt
source-wordcount: '977'
ht-degree: 0%

---

# 使用布局模板自定义左侧面板

在布局模板中，您可以自定义用户在整个左侧面板区域中看到的内容 [!DNL Adobe Workfront].

例如，您可以确定用户在查看任务时在左侧面板中看到的下列项目：

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>对顺序和可见性所做的更改会反映在移动设备应用程序中。

有关组布局模板的信息，请参阅 [创建和修改组的布局模板](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> 要在系统级别执行这些步骤，您需要[!UICONTROL System Administrator]访问级别。<p>要为组执行这些操作，您必须是该组的经理。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自定义中某个区域的左侧面板 [!DNL Workfront]:

1. 开始使用布局模板，如 [创建和管理布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. 单击向下箭头 ![](assets/dropdown-arrow.png) 在 **[!UICONTROL 自定义用户看到的内容]**，然后单击要自定义的左侧面板。

   >[!NOTE]
   >
   >有关 [!UICONTROL 主页] 选项，请参阅 [自定义 [!UICONTROL 主页] 和 [!UICONTROL 概要] 使用布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md). 有关“列表”选项的信息，请参阅 [使用布局模板自定义过滤器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. 在 **[!UICONTROL 左面板]** 列表中，执行以下任一操作以确定用户将在选项的左侧面板中看到的内容([!DNL Workfront] 区域或对象类型)。

   * 显示 ![](assets/add-secondary-nav-item.png) 或隐藏 ![](assets/delete-secondary-nav-item.png) 项目。 任何没有 ![](assets/add-secondary-nav-item.png) 或 ![](assets/delete-secondary-nav-item.png) 无法隐藏。

   * 拖动项目 ![](assets/move-icon---dots.png) 来更改其在左侧面板中的顺序。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>选项</th> 
      <th>当用户单击以下内容时……</th> 
      <th>他们会看到您从以下位置选择的左侧面板项目：</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL项目]</td> 
      <td>项目的名称</td> 
      <td>[!UICONTROL任务]、[!UICONTROL项目详细信息]、[!UICONTROL业务案例]、[!UICONTROL更新]、[!UICONTROL文档]、[!UICONTROL问题]、[!UICONTROL风险]、[!UICONTROL审批]、[!UICONTROL基线]、[!UICONTROL计费率]、[!UICONTROL记录]、[!UICONTROL计费小时数、[!UICONTROL开销小时数]、 [!UICONTROL Workload Balancer]、[!UICONTROL People]、[!UICONTROL Utilization]、[!UICONTROL Queue Details]、[!UICONTROL Routing Rules]、[!UICONTROL Queue Topic]、[!UICONTROL Topic Group]、[!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL任务]</td> 
      <td>任务的名称</td> 
      <td> [!UICONTROL更新]、[!UICONTROL文档]、[!UICONTROL任务详细信息]、[!UICONTROL子任务]、[!UICONTROL问题]、[!UICONTROL时间]、[!UICONTROL批准]、[!UICONTROL费用]、[!UICONTROL前置任务]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL问题]</td> 
      <td>问题的名称</td> 
      <td> [!UICONTROL更新]、[!UICONTROL文档]、[!UICONTROL问题详细信息]、[!UICONTROL小时数]、[!UICONTROL批准]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROLPortfolio]</td> 
      <td>组合的名称</td> 
      <td>[!UICONTROL Projects]、[!UICONTROL Programs]、[!UICONTROLPortfolio详细信息]、[!UICONTROLPortfolio] [!UICONTROL优化]、[!UICONTROL文档]、[!UICONTROL更新]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>项目的名称</td> 
      <td>[!UICONTROL Projects]、[!UICONTROL Program Details]、[!UICONTROL Updates]、[!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL模板]</td> 
      <td>项目模板的名称</td> 
      <td>[!UICONTROL模板任务]、[!UICONTROL模板详细信息]、[!UICONTROL更新]、[!UICONTROL文档]、[!UICONTROL风险]、[!UICONTROL费用]、[!UICONTROL人员]、[!UICONTROL审批]、[!UICONTROL帐单费率]、[!UICONTROL队列详细信息]、[!UICONTROL规则]、[!UICONTROL路由控制，队列主题组]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL模板任务]</td> 
      <td>模板任务的名称</td> 
      <td>[!UICONTROL更新]、[!UICONTROL文档]、[!UICONTROL模板任务详细信息]、[!UICONTROL子任务]、[!UICONTROL费用]、[!UICONTROL批准]、[!UICONTROL前置任务]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL账单记录]</td> 
      <td>项目的计费记录的名称</td> 
      <td>[!UICONTROL账单记录详细信息]、[!UICONTROL可计费小时数]、[!UICONTROL可计费开支]、[!UICONTROL固定收入]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL项目]</td> 
      <td>项目 <img src="assets/projects-in-main-menu.png"> [!UICONTROL主菜单]中 <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL项目]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL请求]</td> 
      <td>请求的名称</td> 
      <td>[!UICONTROL New Request]、[!UICONTROL Submitted requests]、[!UICONTROL All Requests]、[!UICONTROL Drafts]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL功能板]</td> 
      <td>功能板的名称</td> 
      <td>[!UICONTROL My Dashboards]、[!UICONTROL Shared Dashboards]、[!UICONTROL All Dashboards]<p><b>注意</b>:如果您使用 [!DNL Adobe Workfront Classic]，则它们将显示在此列表底部。 对于用户，它们显示在[!UICONTROL功能板]区域左侧面板的底部。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>Scrum团队的名称</td> 
      <td><p>[!UICONTROL Iterations]、[!UICONTROL Current iteration]、[!UICONTROL Backlog]、[!UICONTROL Workload Balancer]、[!UICONTROL Updates]、[!UICONTROL Team Settings]</p> <p><strong>注意：</strong> 的 <strong>[!UICONTROL当前迭代]</strong> 仅当迭代中至少有一个任务或问题时，项目才会在左侧面板中显示。</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL看板团队]</td> 
      <td>看板团队的名称</td> 
      <td>[!UICONTROL工作负载平衡器]、[!UICONTROL看板板]、[!UICONTROL积压工作]、[!UICONTROL更新]、[!UICONTROL团队设置]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfall Team]</td> 
      <td>瀑布团队的名称</td> 
      <td>[!UICONTROL工作负载平衡器]、[!UICONTROL更新]、[!UICONTROL团队请求]、[!UICONTROL团队设置]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL迭代]</td> 
      <td>小版本的名称</td> 
      <td>[!UICONTROL Stories]、[!UICONTROL Issues]、[!UICONTROL Story Board]、[!UICONTROL Overview]、[!UICONTROL Custom Forms]、[!UICONTROL Updates] </td> 
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

   >[!NOTE]
   >
   >最后3个项目 **[!UICONTROL 自定义用户看到的内容]** 下拉列表([!UICONTROL 列表], [!UICONTROL 主页和摘要]和 [!UICONTROL 品牌策略])用于配置左侧面板以外的区域。 有关这些规则的信息，请参阅以下文章：
>   * [使用布局模板自定义过滤器、视图和分组](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [自定义 [!UICONTROL 主页] 和 [!UICONTROL 概要] 使用布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [品牌Adobe [!DNL Workfront] 使用布局模板](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)



1. （可选）如果要添加链接到组织功能板之一的左侧面板项目，请单击 **[!UICONTROL 添加自定义部分]**，键入 **[!UICONTROL 自定义章节标题]** 对于项目，添加功能板。

   功能板项目显示在左侧面板的底部。 当用户将鼠标悬停在左侧面板上时，会看到您在功能板项目旁边键入的自定义章节标题。

   >[!NOTE]
   用户可以向其左侧面板中添加自定义功能板项目。 在布局模板中添加自定义功能板项目时，您的项目会与它们合并，而不会覆盖或重置它们。 如果您将用户分配到具有自定义功能板项目的新布局模板，则也是如此。 有关用户如何自定义左侧面板的信息，请参阅 [创建自定义选项卡或区域](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).

   有关功能板的信息，请参阅 [功能板](../../../reports-and-dashboards/dashboards/dashboards-overview.md).

1. 继续自定义布局模板。

   或

   如果您已完成自定义，请单击 **[!UICONTROL 保存]**.

   >[!TIP]
   您可以单击 [!UICONTROL 保存] 随时要保存进度，稍后继续修改模板。
