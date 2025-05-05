---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: 配置Scrum
description: 在创建团队期间或之后，您可以为Scrum敏捷团队配置以下选项。
author: Lisa
feature: Agile
exl-id: 7509608e-96af-4601-80d4-791ee29046da
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '1739'
ht-degree: 0%

---

# 配置[!UICONTROL Scrum]

您可以在[!DNL Adobe Workfront]中创建Agile团队，如[创建Agile团队](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)中所述。 在创建Agile团队时，您可以选择团队用于完成其工作的方法。 您可以从以下选项中进行选择：

* Scrum
* Kanban

本文介绍了如何配置Scrum团队的设置。 在创建Agile团队并选择Scrum方法之后，您可以参考本文以更新以下设置：

* 故事的估计单位是点还是小时
* 敏捷故事板上的迭代和项目状态列
* 要在敏捷故事板上的故事卡上显示的其他字段
* 颜色指示器如何用于敏捷故事板上的故事
* 将工作项添加到开发周期时如何应用日期

有关配置Kanban团队的信息，请参阅[配置Kanban](/help/quicksilver/agile/get-started-with-agile-in-workfront/configure-kanban.md)。

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
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td> <p>任何</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td> <p>新文档： [!UICONTROL Standard]</p> 
   或
   <p>当前： [!UICONTROL Work]或更高版本</p> </td> 
  </tr>

<tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑团队的访问权限</p>  </td> 
  </tr>

</tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置故事的估计单位为点还是小时

>[!NOTE]
>
>如果团队有任何当前正在进行中的迭代，则无法更改此设置。

您可以将故事配置为使用点数或小时进行估计。

要配置如何为您的Agile团队估计故事：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。
1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有具有[!UICONTROL Standard]、[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。
   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;部分的&#x200B;**[!UICONTROL 估算]**&#x200B;中的故事区域，选择您是要使用点还是小时来估算故事的大小（工作负载）。 如果选择“点”，请指定多少小时等于1点。 （默认值为1点= 8小时。） 这是添加到故事的计划小时数。

   **示例：**&#x200B;如果您已选择估计故事的点数，1点等于8小时，并且估计故事的点数为3，则系统会将24个已计划小时数添加到故事中。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 在敏捷故事板上配置状态列

对于分配给团队的所有小版本或给定项目，您可以配置在敏捷故事板上显示的列。

* [配置迭代的状态列](#configure-status-columns-for-iterations)
* [配置项目的状态列](#configure-status-columns-for-projects)

### 配置迭代的状态列 {#configure-status-columns-for-iterations}

您可以为Agile团队定义故事板上的状态。 这些是在故事板上显示的唯一状态。

要定义可用于与Agile团队关联的故事板的状态，请执行以下操作：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有拥有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在&#x200B;**[!UICONTROL Agile]**&#x200B;部分中，找到&#x200B;**[!UICONTROL 故事板]**&#x200B;区域。

1. （可选）单击&#x200B;**[!UICONTROL 添加列]**&#x200B;以向故事板添加其他状态列。
1. （可选）使用拖放指示器拖动任意状态列，以重新排列故事板上的状态列。 无法移动第一列，也不能将另一列拖到第一列的前面。

   ![拖放](assets/agile-story-card-drag-and-drop.png)

1. 选择任务和问题状态。 任务状态显示为故事板上每个列的列标题。 问题状态您可以选择映射到任务状态。 这意味着当您将问题移动到故事板的另一列时，问题状态将更改为此处显示的问题状态，而不是更改为故事板上的列的名称（反映任务状态）。

   >[!IMPORTANT]
   >
   >只能选择锁定的系统范围状态；不能选择组特定的状态。 此外，第一列的状态始终对应于&#x200B;**[!UICONTROL New]**。

   如果[!DNL Workfront]管理员已配置自定义状态，则可以添加这些状态；自定义状态可按照[创建或编辑状态](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)中的说明进行配置。

   >[!NOTE]
   >
   >选择问题状态时，第三列始终默认为[!UICONTROL 已关闭]。 如果拥有三个以上的列，请确保手动更新这些列以反映正确的状态。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。

### 配置项目的状态列 {#configure-status-columns-for-projects}

有关如何配置项目状态列的信息，请参阅[在 [!DNL Adobe Workfront]](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)中创建或编辑视图一文中的[创建或自定义[!UICONTROL Agile]视图](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md#customizing-an-agile-view)部分。

## 配置要在敏捷故事板上的故事卡上显示的其他字段

将字段添加到故事卡时，填充字段时，字段为仅查看字段和仅显示字段。

默认情况下，任务和问题的故事卡上会显示以下类型的数据：

* 带有直接指向任务或问题的链接的新闻稿名称
* 带有直接项目链接的项目名称
* 此链接仅针对故事显示，不针对子任务显示
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

   ![附加字段](assets/agile-additional-fields-scrum.png)

1. 选择要添加的字段的名称。
1. 为要显示在文章或问题卡上的字段键入&#x200B;**[!UICONTROL 显示名称]**。
1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 配置颜色指示器如何用于敏捷故事板上的故事

默认情况下，敏捷迭代中的故事板图块会根据故事关联的项目进行颜色编码。 每个项目都会在故事板上任意指定一种颜色。 您可以更改每个Agile团队的默认行为。 敏捷故事的颜色可以与故事优先级、所有者等关联。

要更改将颜色分配给敏捷团队故事的行为：

{{step1-to-team}}

1. 单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新团队或在搜索栏中搜索团队。

1. 选择要管理的Agile团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。

   只有拥有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。

   ![编辑团队](assets/edit-team-settings-350x205.png)

1. 在[!UICONTROL Agile]部分的[!UICONTROL 将卡片颜色关联到]区域，从以下选项中选择：

   * **[!UICONTROL 项目]**：颜色与文章所关联的项目相关联。 (创建故事时，必须将其与项目关联，如[创建Agile故事](/help/quicksilver/agile/work-in-an-agile-environment/create-an-agile-story.md)中所述。 同一项目的所有任务以相同颜色显示。
   * **[!UICONTROL 自由表单]**：所有信息卡默认显示为蓝色，直到用户手动更改颜色为止，如Scrum展示板上的[[!UICONTROL 按颜色对故事进行分类]中所述。](/help/quicksilver/agile/use-scrum-in-an-agile-team//scrum-board/categorize-stories-by-color.md)
   * **[!UICONTROL 优先级]**：颜色与文章优先级关联，如下所示：

      * 高=红色
      * Medium =黄色
      * 低=绿色

        如果系统管理员为[!DNL Workfront]系统配置了自定义优先级，则最高优先级为红色，第二高为黄色，第三高为绿色。
   * **[!UICONTROL 任务所有者]**：具有相同主要被分配人的所有故事都是相同的颜色。 主要被分配者是首次分配至任务的用户。


1. 单击&#x200B;**[!UICONTROL 保存更改]**。

## 配置将工作项添加到开发周期时应用日期的方式

默认情况下，将工作项添加到Scrum迭代时，会修改该工作项的“计划开始日期”和“计划完成日期”，以匹配迭代的开始和结束日期。 您可以选择将原始日期保留在团队的所有工作项上。

{{step1-to-team}}

1. （可选）单击&#x200B;**[!UICONTROL 切换团队]**&#x200B;图标![切换团队图标](assets/switch-team-icon.png)，然后从下拉菜单中选择新的Scrum团队或在搜索栏中搜索团队。
1. 单击&#x200B;**[!UICONTROL 更多]**&#x200B;菜单，然后选择&#x200B;**[!UICONTROL 编辑]**。
只有拥有[!UICONTROL 计划]或[!UICONTROL 工作]许可证的团队成员才能看到此选项。
1. 在[!UICONTROL Agile]部分的[!UICONTROL 将工作项添加到开发周期]区域时，从以下选项中选择：

   * **[!UICONTROL 修改规划开始日期和规划完成日期以匹配迭代开始日期和结束日期]**：将工作项添加到迭代时，工作项日期将更改为迭代日期。

     有关如何修改日期的更多信息，请参阅[将故事添加到现有迭代](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)一文中的[了解添加故事如何影响任务日期](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md#understand-how-adding-stories-affects-task-dates)部分。
   * **[!UICONTROL 不修改规划开始日期和规划完成日期以匹配迭代开始日期和结束日期]**：将工作项添加到迭代时，工作项保留其原始日期。

   如果更改日期选项，则不会调整迭代中已存在的工作项的日期。

   这些选项会影响团队将工作项分配给彼此的迭代的日期。 例如，团队A将工作项日期修改为迭代日期，而团队B不修改工作项日期。 如果团队B将工作项分配给团队A的小版本，则将更改工作项日期。 但是，如果团队A将工作项分配给团队B的小版本，日期将不会更改。

1. 单击&#x200B;**[!UICONTROL 保存更改]**。
