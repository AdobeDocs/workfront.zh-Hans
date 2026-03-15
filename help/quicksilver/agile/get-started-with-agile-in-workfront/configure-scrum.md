---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 配置Scrum
description: 您可以在创建团队的过程中或之后为Scrum Agile团队配置以下选项。
author: Courtney
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '1725'
ht-degree: 1%

---

# 配置[!UICONTROL Scrum]

您可以在[!DNL Adobe Workfront]中创建Agile团队，如[创建Agile团队](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)中所述。 创建Agile团队时，您可以选择团队用于完成工作的方法。 您可以从以下选项中进行选择：

* Scrum
* 看板

本文描述如何配置Scrum组的设置。 在创建Agile团队并选择Scrum方法之后，您可以参阅本文来更新以下设置：

* 文章是以点数还是小时为单位进行估计
* 迭代和项目的Agile故事板上的状态列
* 要在敏捷故事板上的故事卡上显示的其他字段
* 颜色指示器如何用于敏捷故事板上的故事
* 将工作项添加到开发周期时如何应用日期

有关配置Kanban团队的信息，请参阅[配置Kanban](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p> 
   <p>工作版或更高版本</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑团队的访问权限</p>  </td> 
  </tr>

</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置是按点还是按小时估算故事

>[!NOTE]
>
>如果团队有任何当前正在进行中的小版本，则无法更改此设置。

您可以将故事配置为使用点数或小时进行估计。

要配置如何为您的Agile团队估计故事，请执行以下操作：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。
1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有具有[!UICONTROL Standard]、[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。
   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;部分的&#x200B;**[!UICONTROL 估计]**&#x200B;中的故事中，选择是否要使用点数或小时来估计故事的大小（工作负荷）。 如果选择“点”，请指定小时数等于1点。 （默认值为1点= 8小时。） 这是添加到文章中的计划小时数。

   **示例：**&#x200B;如果您已选择以磅为单位估计文章，1磅等于8小时，而文章以3磅为单位估计，则系统会向文章添加24个计划时数。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 在Agile故事板上配置状态列

您可以为分配给团队的所有小版本或给定项目配置在Agile故事板上显示的列。

* [配置迭代的状态列](#configure-status-columns-for-iterations)
* [配置项目的状态列](#configure-status-columns-for-projects)

### 配置迭代的状态列 {#configure-status-columns-for-iterations}

您可以定义Agile团队在故事板中的现有状态。 这些是在文章讨论区中显示的唯一状态。

要定义可用于与Agile团队关联的故事板的状态，请执行以下操作：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有拥有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在&#x200B;**[!UICONTROL 敏捷]**&#x200B;部分中，找到&#x200B;**[!UICONTROL 故事板]**&#x200B;区域。

1. （可选）单击&#x200B;**[!UICONTROL 添加列]**&#x200B;向文章讨论区添加其他状态列。
1. （可选）使用拖放指示器拖动任何状态列，以在文章讨论区中对状态列重新排序。 无法移动第一列，也不能将另一列拖到第一列之前。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 同时选择任务和问题状态。 任务状态在文章板上显示为每栏的栏标题。 您选择的问题状态映射到任务状态。 这意味着，当您将问题移动到文章讨论区的另一列时，问题状态将更改为此处显示的问题状态，而不是文章讨论区上的列名称（反映任务状态）。

   >[!IMPORTANT]
   >
   >仅锁定的系统范围状态可供选择；不能选择组特定状态。 此外，第一列的状态始终与&#x200B;**[!UICONTROL New]**&#x200B;相对应。

   如果[!DNL Workfront]管理员已配置自定义状态，则可以添加这些状态；可以按照[创建或编辑状态](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中所述配置自定义状态。

   >[!NOTE]
   >
   >选择问题状态时，第三列的默认值始终为[!UICONTROL 已关闭]。 如果列数超过三列，请确保手动更新列以反映正确的状态。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。

### 配置项目的状态列 {#configure-status-columns-for-projects}

有关如何配置项目状态列的信息，请参阅[在[!UICONTROL 中创建或编辑视图]中](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view)创建或自定义[视图 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)一节。

## 配置要在敏捷故事板上的故事卡上显示的其他字段

将字段添加到文章卡后，当填充字段时，字段将仅供查看并仅显示。

默认情况下，在故事卡上显示以下类型的任务数据和问题数据：

* 文章名称，带有直接指向任务或问题的链接
* 项目名称，其中包含直接指向项目的链接
* 此链接仅对文章显示，对子任务不显示
* 任务或问题描述
* 当前承诺
* 通过调整完成百分比本身或通过调整完成点数或小时数，查看和编辑完成百分比
* 已分配的用户

您可以在故事卡上显示其他数据（包括自定义数据）。 出于各种原因，您可能希望在故事卡上显示其他字段。 例如，如果您正在开发周期内为多个客户处理故事，则可能需要显示客户ID，或者您可能需要显示项目开始日期或项目完成日期。

>[!NOTE]
>
>如果您在故事卡上使用自定义字段，则名称中不能包含句点/点。

配置分配给敏捷团队的故事卡以显示其他字段：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。
只有拥有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;部分中，键入字段名称以找到它。

   ![其他字段](assets/agile-additional-fields-scrum.png)

1. 选择要添加的字段的名称。
1. 键入&#x200B;**[!UICONTROL 显示名称]**&#x200B;以在文章或问题卡上显示的字段。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 配置颜色指示器如何用于敏捷故事板上的故事

默认情况下，敏捷开发周期中的故事板图块会根据与故事关联的项目进行颜色编码。 每个项目都会在故事板上任意指定一种颜色。 您可以更改每个Agile团队的默认行为。 Agile故事的颜色可以与故事优先级、所有者等关联。

要更改将颜色分配给Agile团队故事的行为：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有具有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在[!UICONTROL Agile]部分的[!UICONTROL 将卡颜色关联到]区域，从以下选项中选择：

   * **[!UICONTROL 项目]**：颜色与文章所绑定到的项目相关联。 (文章创建后，必须将其与项目关联，如[创建Agile文章](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md)中所述。 同一项目的所有任务以相同颜色显示。
   * **[!UICONTROL 自由格式]**：默认情况下，所有信息卡都显示为蓝色，直到用户手动更改颜色为止，如[[!UICONTROL 按颜色对文章进行分类] （在情绪板上）](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md)中所述。
   * **[!UICONTROL 优先级]**：颜色与文章优先级关联，如下所示：

      * 高=红色
      * 中=黄色
      * 低=绿色

        如果系统管理员为[!DNL Workfront]系统配置了自定义优先级，则最高优先级为红色，第二高为黄色，第三高为绿色。
   * **[!UICONTROL 任务所有者]**：具有相同主要被分配人的所有故事都是相同的颜色。 主要被分配者是首次分配至任务的用户。


1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 配置将工作项添加到开发周期时应用日期的方式

默认情况下，将工作项添加到Scrum迭代时，会修改工作项的“计划起始日期”和“计划完成日期”，以匹配迭代的起始日期和结束日期。 您可以选择保留团队所有工作项的原始日期。

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队，或在搜索栏中搜索团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。
只有具有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。
1. 在[!UICONTROL Agile]部分的[!UICONTROL 将工作项添加到迭代后]区域，从下列选项中选择：

   * **[!UICONTROL 修改计划开始日期和计划完成日期以匹配迭代开始日期和结束日期]**：将工作项添加到迭代后，工作项日期将更改为迭代日期。

     有关如何修改日期的详细信息，请参阅[将文章添加到现有迭代](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understand-how-adding-stories-affects-task-dates)一文中第[了解添加文章如何影响任务日期](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)节。
   * **[!UICONTROL 不要修改计划开始日期和计划完成日期以匹配迭代开始日期和结束日期]**：将工作项添加到迭代中时，工作项将保留其原始日期。

   如果更改日期选项，则不会调整已在小版本中的工作项的日期。

   这些选项会影响团队将工作项目分配给彼此的小版本的日期。 例如，团队A将工作项日期修改为迭代日期，团队B不修改工作项日期。 如果团队B将工作项分配给团队A的小版本，则工作项日期将更改。 但是，如果团队A将工作项目分配给团队B的小版本，则日期不会更改。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。
