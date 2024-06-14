---
product-area: projects
navigation-topic: use-the-home-area
title: 在中显示项目 [!UICONTROL 工作列表] 在“主页”区域
description: 此 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 区域显示分配给您的所有工作项。 您可以控制哪些项目显示在 [!UICONTROL 工作列表]、使用筛选器以及对工作项进行分组和排序。
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1837'
ht-degree: 0%

---

# 在中显示项目 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 区域

<!-- Audited: 1/2024 -->


此 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 区域显示分配给您的所有工作项。 您可以控制哪些项目显示在 [!UICONTROL 工作列表]、使用筛选器以及对工作项进行分组和排序。

>[!NOTE]
>
>* 将问题转化为任务或项目时，问题会从分配给问题的用户的主页区域移除。
>
>* 将任务转化为项目时，该任务会被删除并从分配给该任务的用户的“主页”区域移除。


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
   <td> <p>新增：</p><ul><li>[！UICONTROL Contributor]仅供审批</li> <li>[！UICONTROL Standard]或更高版本（适用于所有其他对象）</li> <p>或</p> 
  </ul><p>当前：</p><ul><li>[！UICONTROL Review]仅供审批</li> <li>适用于所有其他对象的[！UICONTROL工作]或更高版本</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[！UICONTROL视图]或更高的项目、任务、问题和文档访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>Contribute权限或更高权限可为您需要处理的任务和问题提供内容</p>  </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 筛选 [!UICONTROL 工作列表]

您可以按以下项筛选项目： [!UICONTROL 工作列表] 以仅查看特定类型的项目。 例如，您可以过滤 [!UICONTROL 工作列表] 以仅显示问题或请求。

>[!NOTE]
>
>过滤器选项存储在浏览器中。 如果您始终在同一台计算机上使用同一浏览器（并且不清除网站数据），则所选筛选器不会更改。 如果切换浏览器或计算机，则筛选器将还原为默认选项，即取消选择所有筛选器。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 筛选]** ![](assets/filter-nwepng.png) 下拉菜单。 如果您选择了任何过滤器，则会显示选定过滤器的数量来代替图标。
1. 从以下筛选器选项中进行选择，以指定要显示的项目类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL All]</strong></td> 
      <td>显示并选择所有项目。 这包括任务、问题、批准、个人任务以及已完成的任务和问题。 </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL任务：处理]</strong></td> 
      <td> <p>仅显示您正在处理的任务。 这些是分配给您的任务，您已为其单击[！UICONTROL处理此项工作]按钮。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL任务：准备开始]</strong></td> 
      <td> 
       <div> 
        <p>仅显示已准备好开始的任务。 以下两个语句都必须为true：</p> 
        <ul> 
         <li> <p>这些任务及其父任务没有阻止它们进行处理的前置任务或任务限制。</p> </li> 
         <li> <p>任务的[！UICONTROL计划开始日期]是过去的日期，或者最多为两周后的日期。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL任务：未就绪]</strong></td> 
      <td> 
       <div> 
        <p>仅显示尚未准备就绪的任务。 以下任一语句必须为true：</p> 
        <ul> 
         <li> <p>这些任务及其父任务可能具有阻止它们进行处理的前置任务或任务限制。</p> </li> 
         <li> <p>这些任务的[！UICONTROL计划开始日期]在未来的两周以上。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL问题：正在处理]</strong></td> 
      <td> <p>仅显示您正在处理的问题。 这些是分配给您的问题，您已针对这些问题单击[！UICONTROL处理此项工作]按钮。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL问题：已请求]</strong></td> 
      <td>仅显示已分配但您未单击[！UICONTROL处理此项工作]按钮的问题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>个人的</strong></td> 
      <td>仅显示个人任务。 这些是您创建为[！UICONTROL待办事项]任务的任务，如一节中所述 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">创建个人任务</a> 在文章中 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">从[！UICONTROL主页]区域创建工作项</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL审批]</strong></td> 
      <td> 
       <div> 
        <p>仅显示分配给您或委托的审批以及您已提交的审批。 审批包括审批工作项（项目、任务和问题），以及审批文档、验证、访问请求和工时表。 有关审批的更多信息，请参阅以下文章：</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">查看审批</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">工作审批</a> </p> </li> 
        </ul> 
        <p>注意：您提交的批准以及您也是批准者之一的批准将被计算两次。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL委托：由我委托]</strong></td> 
      <td> 
       <div> 
        <p>仅显示已委派给其他用户的工作项。</p> 
        <p>有关委派任务的更多信息，请参阅 <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">将任务和问题委派给其他用户</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL已委派：已委派给我]</strong></td> 
      <td> 
       <div> 
        <p>仅显示其他用户临时委派给您的工作项。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL已完成]</strong></td> 
      <td> <p>仅显示已完成的任务、问题和个人任务。 系统会显示前两周的已完成工作，并根据完成工作的周分组到“工作列表”中。 不包括审批。</p> <p>除非选择此筛选器，否则已完成的工作将在[！UICONTROL工作列表]中隐藏。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* 过滤器选项基于对象（任务、问题、批准、个人任务）。
   >* 任务和问题按其与我们已准备好处理它们的关系的状态进一步过滤([!UICONTROL 正在处理]， [!UICONTROL 准备开始]， [!UICONTROL 未就绪] 任务，以及 [!UICONTROL 正在处理] 和 [!UICONTROL 已请求] 问题)。 您可以选择显示处于特定状态的任务或问题，或者单击任务或问题以选择并显示所有状态。
   >* 已完成项目有一个单独的过滤器，其中包括任务和问题。 这不包括审批。 此 [!UICONTROL 已完成] 过滤器包括个人任务。
   >* 您可以选择一次只显示一个状态。 例如，您只能显示 [!UICONTROL 正在处理] 仅任务 [!UICONTROL 已请求] 问题。 您还可以一次选择多个状态。
   >* 您不能对分配给您的某个团队的项目应用筛选器，并且团队分配未包含在直接分配给您的项目中。


1. （可选）进一步组织 [!UICONTROL 工作列表]，如一节中所述 [按日期、项目和优先级进行分组和排序](#group-and-sort-by-date-project-and-priority) 本文章中。

## 分组和排序方式 [!UICONTROL 日期]， [!UICONTROL 项目]、和 [!UICONTROL 优先级]

您可以对 [!UICONTROL 工作列表] 按 [!UICONTROL 计划完成日期]， [!UICONTROL 提交日期]， [!UICONTROL 项目]，或 [!UICONTROL 我的优先级]. 您选择的选项决定了项目在 [!UICONTROL 工作列表].

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 分组依据]** ![分组依据](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png) 下拉菜单。

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. 从以下选项中选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL计划完成]</strong></td> 
      <td> <p> 项目在[！UICONTROL工作列表]的以下分组中显示，具体取决于其[！UICONTROL计划完成日期] （每个分组中包含的项目数显示在标题标题旁边的括号中）：</p> 
       <ul> 
        <li> <p>[！UICONTROL延迟]</p> </li> 
        <li> <p>[！UICONTROL无计划完成日期]</p> </li> 
        <li> <p>[！UICONTROL本周]</p> <p>默认情况下，此分组是展开的。</p> </li> 
        <li> <p>[！UICONTROL下周]</p> </li> 
        <li> <p>[！UICONTROL已计划]，随后是各种[！UICONTROL计划完成日期]（多个分组）</p> </li> 
        <li> <p>[！UICONTROL完成]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL计划开始]</strong></td> 
      <td> <p>项目在[！UICONTROL工作列表]的以下分组中显示，具体取决于其[！UICONTROL计划开始日期] （每个分组中包含的项目数显示在标题标题旁边的括号中）：</p> 
       <ul> 
        <li> <p>[！UICONTROL延迟]</p> </li> 
        <li> <p>[！UICONTROL本周] </p> <p>默认情况下，此分组是展开的。</p> </li> 
        <li> <p>[！UICONTROL下周]</p> </li> 
        <li> <p>[！UICONTROL已计划]，其后各个[！UICONTROL已计划开始日期]（多个分组）</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL提交日期]</strong></td> 
      <td> <p>项目显示在[！UICONTROL工作列表]的以下分组中（每个分组中包含的项目数显示在标题标题旁边的括号中）：</p> 
       <ul> 
        <li> <p>[！UICONTROL无提交日期]</p> </li> 
        <li> <p>[！UICONTROL下周提交]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL项目]</strong></td> 
      <td>项目根据项目进行分组，项目在[！UICONTROL工作列表]中按字母顺序显示。 （每个分组中包含的项目数显示在标题标题旁边的括号中。）</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！UICONTROL我的优先级]</strong></td> 
      <td>项目按您选择的顺序显示。 有关更多信息，请参阅 <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">优先处理[！UICONTROL主页]区域中的工作</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>默认排序为升序。 如果将排序更改为降序，则选定的排序选项将存储在浏览器中。 如果您始终在同一台计算机上使用同一浏览器（并且不清除站点数据），排序不会更改，但如果您切换浏览器或计算机，则排序会更改为默认排序。

## 查看延迟项目

[!DNL Adobe Workfront] 使用以下日期来确定工作请求是否延迟：

* **任务**： [!UICONTROL 计划完成日期]
* **问题**： [!UICONTROL 计划完成日期]
* **文档**： [!UICONTROL 提交日期]
* **时间表**： [!UICONTROL 提交日期]
* **审批**： [!UICONTROL 提交日期]
* **验证审批**： [!UICONTROL 验证截止日期]

## 搜索 [!UICONTROL 工作列表]

当您搜索 [!UICONTROL 工作列表]，则分配给您的任何项目都会在搜索中返回（甚至包括当前未加载到屏幕上的项目）。 如果 [!UICONTROL 显示完成] 选项，则也会返回您在过去两周内标记为完成的任何项目。

此外，仅搜索工作项的名称（不搜索工作项中的信息，也不搜索工作项所在项目的名称）。

要搜索 [!UICONTROL 工作列表]：

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. （可选）筛选并分组 [!UICONTROL 工作列表]，如中所述 [筛选 [!UICONTROL 工作列表]](#filter-the-work-list) 和 [按日期、项目和优先级进行分组和排序](#group-and-sort-by-date-project-and-priority).

1. （可选）如果要搜索已完成的工作项，则必须配置 [!UICONTROL 工作列表] 以在搜索前显示已完成的项。

1. 单击搜索图标 ![Search](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. 开始键入要搜索的项目名称的名称。\
   此 [!UICONTROL 工作列表] 自动过滤以包含具有匹配名称的项目。

## 更改工作列表的大小

您可以更改 [!UICONTROL 工作列表] 因此它消耗的面积大约为家庭面积的四分之一到家庭面积的一半 [!UICONTROL 主页] 区域。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. 将鼠标悬停在 [!UICONTROL 工作列表]，然后向左或向右拖动，直到工作列表达到所需大小。

## 折叠和展开分组

中的项目 [!UICONTROL 工作列表] 在分组中显示。 您可以折叠和展开分组，以控制在给定时间页面上显示的信息量。

您可以折叠和展开以下项中的分组： [!UICONTROL 工作列表] 更好地控制哪些信息是可见的。\
默认情况下， [!UICONTROL 本周] 展开分组，并折叠所有其他分组。 下次访问“主页”区域时，将会记住您所做的任何更改。

1. 单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon.png) 单击Adobe Workfront右上角的或者（如果可用）单击 **[!UICONTROL 主菜单]** 图标 ![主菜单](/help/_includes/assets/main-menu-icon-left-nav.png) 图标，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 展开]** 或 **[!UICONTROL 折叠]** 要展开或折叠的任何分组旁边的箭头。

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   或\
   要同时展开或折叠所有分组，请单击 **[!UICONTROL 展开]** 或 **[!UICONTROL 折叠]** 按住任意分组旁边的箭头 [!UICONTROL Shift] 键。
