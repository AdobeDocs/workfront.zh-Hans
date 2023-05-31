---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: 委派任务和问题
description: 您可以在外出办公时临时委派指派给您的工作。 本文介绍了如何委派任务和问题分配。
author: Alina
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 1%

---

# 管理任务和问题委派

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

您可以在外出办公时临时委派指派给您的工作。

您可以委派任务和问题分配，也可以委派审批。 本文介绍了如何委派任务和问题分配。

有关委派工作的一般信息，请参阅 [委派工作概述](../../manage-work/delegate-work/delegate-work-overview.md).

## 访问要求

>[!IMPORTANT]
>
>* 您选择作为委派的用户将获得与您委派给他们的任务和问题的权限相同的权限。
>* 这些权限必须在其访问级别内工作，有时，其访问级别可能低于您的访问级别。

   >
   >   
   >   例如，如果用户对其访问级别的任务只有“查看”访问权限，而您对您委派给他们的任务具有“管理”权限，则他们将对您委派给他们的任务获得“管理”权限。 但是，他们将无法对委派的任务执行与您相同的操作。 他们必须向系统管理员请求对任务的编辑访问权限，才能在您缺席时更新任务。
   >
   >   
   >   有关如何修改访问级别的信息，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* 对于在委派开始后分配的项目，在为其分配项目后可能最多需要一小时 [!DNL Workfront] 以与委派共享新分配的项目。



您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>审核或更高</p>

>[!NOTE]
>
>尽管您可以在拥有Request许可证时被分派到工作，但您不能将您的工作委派给其他人。 [!DNL Workfront] 不建议将工作分派给审阅或请求用户。

</tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和问题的访问权限如果您仍然没有访问权限，请咨询 [!DNL Workfront] 管理员（如果他们在您的访问级别设置了其他限制）。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参见 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> 创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看分配给您的任务或问题的权限或更高的权限</p> 
    <p>有关请求其他访问权限的信息，请参阅 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## 先决条件

在执行本文中所述的活动之前，必须确保以下各项：

* 您的 [!DNL Workfront] 或组管理员已启用 [!UICONTROL 允许用户删除具有记录小时数的任务和问题] 在中设置 [!UICONTROL 设置] 区域 [!DNL Workfront] 实例。

   有关更多信息，请参阅 [配置系统范围的任务和问题首选项](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## 将任务和问题委派给其他用户

在将工作委派给他人之前，我们建议您联系他们，并通知他们将指定为您工作项目的代表。 委派工作前请他们口头批准，以确保他们有必要的时间在您外出期间完成工作。

有关委派任务和问题的一般信息，请参阅 [委派任务和问题概述](delegate-work.md).

要将您的任务和问题委派给其他人，请执行以下操作：

1. 转到 [!UICONTROL **主页**] 区域，然后单击 [!UICONTROL **委派**] 在顶部 [!UICONTROL **工作列表**].

   ![](assets/delegate-button-in-home.png)

1. 在 [!UICONTROL **委派任务和问题**] 选项卡，更新以下内容：

   * [!UICONTROL **将您的任务和问题委派给**]：开始键入要将您的任务和问题委派给某个用户的名称，然后在该名称显示在列表中时将其选定。 您只能选择一个用户。\

      您选择作为代理的用户将获得与您委派给他们的任务和问题权限相同的权限。 有关更多信息，请参阅 [委派任务和问题概述](delegate-work-overview.md).

   * [!UICONTROL **开始日期**]：从日历中选择开始委派工作项的日期。

      >[!TIP]
      >
      >开始日期不能是过去。

   * [!UICONTROL **无结束日期**]：如果您不想指定委派的结束日期，请选择此选项。

   * [!UICONTROL **结束日期**]：从日历中选择委派应停止的日期。

      >[!TIP]
      >
      >不选择结束日期将仅启用当天的委派。

      ![](assets/delegate-box-expanded-in-home.png)

1. 单击&#x200B;[!UICONTROL **保存**]。

   会发生以下情况：

   * 您的工作已委派给指定用户。 委派任何日期在您选择的时间范围内（包括在启用委派后新分配的任务或问题）的未完成任务或问题。
   >[!TIP]
   >
   >   日期在委派时间范围内的已完成工作项不会被委派。


   * 您会在屏幕右上角收到一条消息，确认您已启用将工作委派给其他用户。 委托用户的名称显示在确认消息中。

   * 大多数区域都显示您的任务和问题已委派给其他用户，您可以在其中查看工作分配 [!DNL Workfront]. 有关哪些区域不包含代表名的详细信息，请参见 [委派任务和问题概述](delegate-work-overview.md).

   * 此 [!UICONTROL **委派**] 中的按钮 [!UICONTROL 主页] 区域更改为 [!UICONTROL **编辑委派**] 表示已建立委托。

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * 如果启用了事件通知和个人通知，您还会收到一封关于您委派的电子邮件确认。

   * 您选择作为委派的用户会收到一封有关委派的电子邮件（如果已启用其事件通知）。

      有关启用个人电子邮件通知的信息，请参阅 [激活或停用您自己的事件通知](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).





## 编辑或停止委派

如果您选择了结束日期，则可以让委派过期，也可以手动停止委派。 如果委派日期发生更改，您还可以修改委派的时间范围。

1. 转到 [!UICONTROL 主页] 区域，然后单击 [!UICONTROL 编辑委派] 工作列表的右上角。
1. 在 [!UICONTROL 委派任务和问题] 选项卡，执行以下操作之一：
   * 修改 [!UICONTROL **开始日期**] 或 [!UICONTROL **结束日期**]
   * 单击 [!UICONTROL **停止委派**]

   >[!TIP]
   >
   >    如果委派已开始，则只能编辑委派的结束日期。

   ![](assets/stop-delegation-screen-in-home.png)

1. （视情况而定）单击 [!UICONTROL **保存**] 保存新的委派日期

   或

   单击 [!UICONTROL **停止委派**] ，以确认停止委托。

   委派要么更新了日期，要么已停止，并且已从您的任务和问题中删除委派的用户。 他们对任务和问题的权限保持不变。


## 找到委托的工作和委托信息

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

在委派任务和问题时，有以下几方面： [!DNL Workfront] 您可在其中查看委托的工作或委托人。

* [在“工作”框中查找委派](#locate-delegates-in-the-assignments-box)
* [在中查找委托的工作 [!UICONTROL 主页]](#locate-delegated-work-in-home)


### 在中查找代理人 [!UICONTROL 指定任务] 框

当您的系统或组管理员在系统中启用工作委派时， [!UICONTROL 指定任务] 框会在其可访问的位置显示以下选项卡：

* [!UICONTROL **指定任务**]：此处显示分配给任务或问题的用户。
* [!UICONTROL **委派**]：由任务或问题的被分派人指定为委派的用户将显示在此处。

您可以访问 [!UICONTROL 指定任务] 框中的字符进行标识：

* 任务或问题标题

   ![](assets/assignments-and-delegates-panel-in-task-header.png)

   此 [!UICONTROL 指定任务] 任务或问题标题中的字段更改为 [!UICONTROL 任务和委派].

* 此 [!UICONTROL 工作负载均衡器] 手动分配任务或问题时

   ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> 您无法在中查看委派 [!UICONTROL 指定任务] 任务或问题编辑框的部分。

如果委派了任务或问题，并且 [!UICONTROL 委派] 子选项卡为空，可能存在以下情况之一：

* 您未被分派至任务或问题。
* 任务或问题日期不在委派的时间范围内。

>[!TIP]
>
>委派的任务和问题的计划或实际小时数未纳入资源管理工具中，例如 [!UICONTROL 工作负载均衡器] 或 [!DNL Resource Planner] （对于已委派用户）。 小时数仅与分配的用户相关联。

### 在中查找委托的工作 [!UICONTROL 主页]

1. 转到 [!UICONTROL **主页**] 区域，然后单击过滤器下拉菜单并选择以下一个或多个选项：
   * [!UICONTROL **已委派**]：查看委派给您或由您委派的任务和问题。
   * [!UICONTROL **已委派给我**]：查看由其他用户委派给您的任务和问题。
   * [!UICONTROL **由我委派**]：查看您委派给其他用户的任务和问题。

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. 单击 [!UICONTROL 排序] 下拉菜单按以下条件对列表进行排序：
   * [!UICONTROL 计划完成]. 这是默认排序选项。
   * [!UICONTROL 计划开始]
   * [!UICONTROL 提交日期]
   * [!UICONTROL 项目]
   * [!UICONTROL 我的优先级]
1. 展开中的分组 [!UICONTROL **工作列表**] 查看委托的工作项。 存在以下情况：
   * 对于您委托给其他人的项目，委托人的名称显示在 [!UICONTROL **工作列表**] 以及 [!UICONTROL **任务和委派**] 右边的字段。

   * 对于委派给您的项目，被分派人的姓名将显示在 [!UICONTROL **工作列表**] 以及 **[!UICONTROL 任务和委派]** 右边的字段。
   >[!TIP]
   >
   >    如果委托的开始日期设置为今天日期之后的某个日期，则委托的开始日期也会显示在 [!UICONTROL 工作列表]. 委派项目会显示在您为选择的分组中 [!UICONTROL 工作列表]，根据分组的类型。 例如，如果您按以下条件分组： [!UICONTROL 计划完成日期]，则委派的项目会显示在与其规划完成日期匹配的分组中。
