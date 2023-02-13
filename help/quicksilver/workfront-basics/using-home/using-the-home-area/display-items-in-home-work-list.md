---
product-area: projects
navigation-topic: use-the-home-area
title: 显示 [!UICONTROL 工作列表] 在主区
description: 的 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 区域会显示分配给您的所有工作项。 您可以控制在 [!UICONTROL 工作] 列表，如下所述。
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# 显示 [!UICONTROL 工作列表] 在主区

的 [!UICONTROL 工作列表] 在 [!UICONTROL 主页] 区域会显示分配给您的所有工作项。 您可以控制在 [!UICONTROL 工作] 列表，如下所述。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 许可证*</strong></td> 
   <td> <p>[!UICONTROL Review]（仅供审批）</p> <p>[!UICONTROL Work]或更高版本（适用于所有其他对象）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置*</strong></td> 
   <td> <p>[!UICONTROL视图]或更高版本对项目、任务、问题和文档的访问权限</p> <p>注意：如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>对象权限</strong></td> 
   <td> <p>为您需要处理的任务和问题提供权限或更高权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## 筛选 [!UICONTROL 工作列表]

您可以在 [!UICONTROL 工作列表] 以仅查看特定类型的项目。 例如，您可以过滤 [!UICONTROL 工作列表] 以仅显示问题或请求。

>[!NOTE]
>
>过滤器选项存储在浏览器中。 如果您在同一台计算机上始终使用相同的浏览器（并且不清除网站数据），则选定的过滤器不会更改。 如果切换浏览器或计算机，则过滤器会还原为默认选项，即取消选择所有过滤器。

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 过滤器]** ![](assets/filter-nwepng.png) 下拉菜单。
1. 从以下筛选器选项中进行选择，以指定要显示的项目类型：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL All]</strong></td> 
      <td>显示并选择所有项目。 这包括任务、问题、批准、个人任务以及已完成的任务和问题。 </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL任务正在处理]</strong></td> 
      <td> <p>仅显示您正在积极处理的任务。 这些是分配给您的任务，您已为这些任务单击了[!UICONTROL Work On It]按钮。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL任务准备开始]</strong></td> 
      <td> 
       <div> 
        <p>仅显示已准备好开始的任务。 以下两个语句必须都为true:</p> 
        <ul> 
         <li> <p>这些任务及其父代没有前任或任务约束，无法处理这些任务。</p> </li> 
         <li> <p>任务的[!UICONTROL计划开始日期]是过去的或将来的两周。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL任务未就绪]</strong></td> 
      <td> 
       <div> 
        <p>仅显示尚未准备好启动的任务。 以下任一语句必须为true:</p> 
        <ul> 
         <li> <p>这些任务及其父代可能具有前任或任务约束，以阻止他们进行工作。</p> </li> 
         <li> <p>这些任务的[!UICONTROL计划开始日期]将来会超过两周。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL问题处理]</strong></td> 
      <td> <p>仅显示您正在积极处理的问题。 这些是分配给您的问题，您已为此单击[!UICONTROL Work On It]按钮。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[！请求的UICONTROL问题]</strong></td> 
      <td>仅显示分配给您但尚未单击[!UICONTROL Work On It]按钮的问题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>个人的</strong></td> 
      <td>仅显示个人任务。 这些任务是您创建为[!UICONTROL To Do]任务的任务，如一节中所述 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">创建个人任务</a> 在文章中 <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">从[!UICONTROL Home]区域创建工作项</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Approvals]</strong></td> 
      <td> 
       <div> 
        <p>仅显示分配给您或已委派给您的批准以及您提交的批准。 批准包括对工作项（项目、任务和问题）的批准，以及对文档、校样、访问请求和时间表的批准。 有关批准的更多信息，请参阅以下文章：</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">查看批准</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">工作批准</a> </p> </li> 
        </ul> 
        <p>注意：您提交的批准以及您也是批准者之一的批准将被计数两次。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL已完成]</strong></td> 
      <td> <p>仅显示已完成的任务、问题和个人任务。 已完成的工作将显示前两周的工作，并根据完成的周分组到工作列表中。 不包括批准。</p> <p>除非您选择此过滤器，否则已完成的工作将隐藏在[!UICONTROL工作列表]中。</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* 过滤器选项基于对象（任务、问题、批准、个人任务）。
   >* 任务和问题会根据其状态进一步过滤，以便与我们准备处理这些任务和问题([!UICONTROL 处理], [!UICONTROL 准备开始], [!UICONTROL 未就绪] ，以及 [!UICONTROL 处理] 和 [!UICONTROL 请求] )。 您可以选择显示特定状态中的任务或问题，或单击任务或问题以选择和显示所有状态。
   >* 已完成的项目有一个单独的过滤器，它包括任务和问题。 这不包括批准。 的 [!UICONTROL 已完成] 过滤器包括个人任务。
   >* 一次只能选择一个状态。 例如，您只能显示 [!UICONTROL 处理] 任务和仅 [!UICONTROL 请求] 问题。
   >* 您无法对分配给您的一个团队的项目应用过滤器，并且这些过滤器不会包含在直接分配给您的项目中。



1. （可选）进一步组织 [!UICONTROL 工作列表]，如一节中所述 [按日期、项目和优先级分组和排序](#group-and-sort-by-date-project-and-priority) 在本文中。

## 分组和排序依据 [!UICONTROL 日期], [!UICONTROL 项目]和 [!UICONTROL 优先级]

您可以对 [!UICONTROL 工作列表] by [!UICONTROL 计划完成日期], [!UICONTROL 提交日期], [!UICONTROL 项目]或 [!UICONTROL 我的优先级]. 您选择的选项可确定项目在 [!UICONTROL 工作列表].

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 分组依据]** 下拉菜单。

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. 从以下选项中进行选择：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL计划完成]</strong></td> 
      <td> <p> 项目在[!UICONTROL工作列表]中以下分组中显示，具体取决于其[!UICONTROL计划完成日期]（每个分组中包含的项目数显示在标题标题旁边的括号中）：</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL无计划完成日期]</p> </li> 
        <li> <p>[!UICONTROL本周]</p> <p>默认情况下，此分组会展开。</p> </li> 
        <li> <p>[!UICONTROL下周]</p> </li> 
        <li> <p>[!UICONTROL计划]，然后是各种[!UICONTROL计划完成日期]（多个分组）</p> </li> 
        <li> <p>[!UICONTROL Complete]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL计划开始]</strong></td> 
      <td> <p>项目在[!UICONTROL工作列表]中以下分组中显示，具体取决于其[!UICONTROL计划开始日期]（每个分组中包含的项目数显示在标题标题旁边的括号中）：</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL本周] </p> <p>默认情况下，此分组会展开。</p> </li> 
        <li> <p>[!UICONTROL下周]</p> </li> 
        <li> <p>[!UICONTROL已计划]，后跟各种[!UICONTROL计划开始日期]（多个分组）</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL提交日期]</strong></td> 
      <td> <p>项目在[!UICONTROL工作列表]的以下分组中显示（每个分组中包含的项目数显示在标题标题旁边的圆括号中）：</p> 
       <ul> 
        <li> <p>[!UICONTROL无提交日期]</p> </li> 
        <li> <p>[!UICONTROL下周提交]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL项目]</strong></td> 
      <td>项目会根据项目进行分组，并且项目会在[!UICONTROL工作列表]中按字母顺序显示。 （每个分组中包含的项目数显示在标题标题旁边的圆括号中。）</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL My Priority]</strong></td> 
      <td>项目按您选择的顺序显示。 有关更多信息，请参阅 <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">在[!UICONTROL Home]区域优先处理工作</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>默认排序为升序。 如果将排序更改为降序，则选定的排序选项会存储在浏览器中。 如果您在同一台计算机上始终使用相同的浏览器（并且不清除网站数据），则排序不会更改，但是，如果您切换浏览器或计算机，则排序会更改为默认排序。

## 查看延迟项目

[!DNL Adobe Workfront] 使用以下日期确定工作请求是否延迟：

* **任务**: [!UICONTROL 计划完成日期]
* **问题**: [!UICONTROL 计划完成日期]
* **文档**: [!UICONTROL 提交日期]
* **工时单**: [!UICONTROL 提交日期]
* **批准**: [!UICONTROL 提交日期]
* **校样批准**: [!UICONTROL 校样截止时间]

## 搜索 [!UICONTROL 工作列表]

当您搜索 [!UICONTROL 工作列表]，则搜索中会返回分配给您的任何项目（甚至是当前未在屏幕上加载的项目）。 如果 [!UICONTROL 显示结束] 选项时，也会返回您在过去两周内标记完成的任何项目。

此外，只搜索工作项的名称（不搜索工作项内的信息，也不搜索工作项所在项目的名称）。

搜索 [!UICONTROL 工作列表]:

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. （可选）筛选 [!UICONTROL 工作列表]，如 [筛选 [!UICONTROL 工作列表]](#filter-the-work-list) 和 [按日期、项目和优先级分组和排序](#group-and-sort-by-date-project-and-priority).

1. （可选）如果您正在搜索已完成的工作项，则必须配置 [!UICONTROL 工作列表] ，以在搜索之前显示已完成的项目。
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. 开始键入要搜索的项目名称的名称。\
   的 [!UICONTROL 工作列表] 会自动过滤为包含具有匹配名称的项目。

## 更改工作列表的大小

您可以更改 [!UICONTROL 工作列表] 因此，它会消耗大约四分之一到大约一半的“主区” [!UICONTROL 主页] 的上界。

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 将鼠标悬停在 [!UICONTROL 工作列表]，然后向左或向右拖动直到工作列表达到所需大小。

## 折叠和展开分组

中的项目 [!UICONTROL 工作列表] 按分组显示。 您可以折叠和展开分组以控制在给定时间页面上显示的信息量。

您可以在 [!UICONTROL 工作列表] 以更好地控制哪些信息可见。\
默认情况下， [!UICONTROL 本周] 组将展开，所有其他组都将折叠。 下次访问“主页”区域时，您所做的任何更改都会被记住。

1. 单击 **[!UICONTROL 主菜单]** ![](assets/main-menu-icon.png) ，然后单击 **[!UICONTROL 主页]**.
1. 单击 **[!UICONTROL 展开]** 或 **[!UICONTROL 折叠]** 要展开或折叠的任意分组旁边的箭头。

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   或\
   要同时展开或折叠所有分组，请单击 **[!UICONTROL 展开]** 或 **[!UICONTROL 折叠]** 按住任意分组旁边的箭头 [!UICONTROL Shift] 键。
