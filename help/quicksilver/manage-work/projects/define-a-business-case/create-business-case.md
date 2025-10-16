---
navigation-topic: business-case-and-scorecards
title: 为项目创建业务案例
description: 您可以使用业务案例来请求项目，并定义项目的目的、预算和潜在利益。 Portfolio经理或项目发起人在批准项目之前，会使用业务案例中的信息来分析和优先处理项目。
author: Becky
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: fa0b4322b9f7c1d506cf194645c7ae50ad8c0f0b
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# 为项目创建业务案例

<!--Audited: 6/2025-->

您可以使用业务案例来请求项目，并定义项目的目的、预算和潜在利益。 Portfolio经理或项目发起人在批准项目之前，会使用业务案例中的信息来分析和优先处理项目。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront计划</p></td> 
   <td> 
   <p>Prime或更高版本</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证</p></td> 
   <td> 
   <p>标准 </p> 
   <p>规划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>编辑对项目、财务数据和资源管理的访问权限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td> <p>管理项目或更高权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

通过业务案例请求项目时，请考虑以下事项：

* 您的Adobe Workfront管理员或组管理员必须启用业务案例的各个部分，然后才能将其显示在您的项目中。\
  有关在系统级别启用业务案例中的部分的信息，请参阅文章[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

  有关业务案例领域的信息，请参阅文章[业务案例领域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)。

* 如果希望项目在Portfolio优化器中获得分数，则必须完成业务案例的所有区域，但“目标”区域除外。 完成目标区域是可选的。 即使此区域未完成，项目也会在Portfolio Optimizer中获得一个分数。

  有关使用记分卡和Portfolio Optimizer的信息，请参阅文章[将记分卡应用于项目并生成一致性分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

## 创建业务案例

{{step1-to-projects}}

1. 单击&#x200B;**新建项目**，然后从出现的下拉列表中选择&#x200B;**请求项目**。 项目已创建，默认情况下会分配&#x200B;**Idea**&#x200B;状态。

   >[!CAUTION]
   >
   >如果在您的Workfront实例中删除了“想法”状态，则项目会置于新项目的默认状态，如项目偏好设置区域中所定义。 有关设置项目首选项的信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。

1. 在项目标题字段中输入名称。
1. （可选）单击&#x200B;**更多**&#x200B;图标![更多图标](assets/qs-more-icon-on-an-object.png)，然后单击&#x200B;**附加模板**&#x200B;以创建项目的工作划分结构。

   或

   开始手动将任务添加到项目。

1. （视情况而定）如果您已选择附加模板，请继续将模板附加到项目。
1. 在左侧面板中，单击&#x200B;**业务案例**。
1. （可选）要编辑&#x200B;**项目信息**&#x200B;部分，请单击&#x200B;**编辑项目信息**。 

   有关编辑&#x200B;**项目信息**&#x200B;分区字段的更多信息，请参阅[业务案例区域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info)一文中的[项目信息](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)分区。

1. （可选）要编辑&#x200B;**目标**&#x200B;部分，请单击&#x200B;**编辑目标**。

   有关编辑业务案例的&#x200B;**目标**&#x200B;部分的更多信息，请参阅[业务案例领域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals)一文中的[目标](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)部分。

1. （可选）要编辑&#x200B;**费用**&#x200B;部分，请单击&#x200B;**编辑费用**。

   有关编辑业务案例的&#x200B;**费用**&#x200B;部分的详细信息，请参阅[业务案例领域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses)一文中的[费用](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)部分。

1. （可选）单击&#x200B;**编辑资源预算**&#x200B;以预算您的资源并获得与项目上的工作角色关联的预算劳力成本。 有关详细信息，请参阅业务案例中的[预算资源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)。

   >[!TIP]
   >
   >此处显示的信息与系统级资源预算工具中显示的信息相同。

1. （可选）单击&#x200B;**编辑风险**&#x200B;以向此项目添加潜在风险。 有关向业务案例添加风险的信息，请参阅[业务案例领域概述](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)一文中的[风险](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md)部分。
1. （可选）在&#x200B;**将记分卡添加到此项目**&#x200B;下拉菜单中选择&#x200B;**记分卡**。

   必须先创建记分卡，然后才能将记分卡附加到项目。

   有关记分卡的更多信息，请参阅文章[将记分卡应用到项目并生成一致性分数](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)。

1. （可选）在&#x200B;**自定义Forms**&#x200B;下拉菜单中选择&#x200B;**自定义表单**。

   必须先创建自定义Forms，然后才能将其附加到项目。

   有关自定义Forms的详细信息，请参阅文章[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

1. 单击&#x200B;**提交**。 项目状态已更改为&#x200B;**已请求**，已提交它以批准业务案例。

   有关批准业务案例的详细信息，请参阅文章[批准业务案例](../../../manage-work/projects/define-a-business-case/approve-business-case.md)。


>[!TIP]
>
> 完成业务案例后，您可以将其副本导出到.pdf文件。 有关将业务案例导出到.pdf文件的详细信息，请参阅[导出项目的业务案例](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md)。


