---
content-type: overview
product-area: projects
navigation-topic: financials
title: 设置工作角色以进行计费
description: 通过Workfront，您可以按不同于主要工作角色的工作角色对用户计费。 当某人临时执行应按不同费率计费的工作时，这将很有用。
author: Lisa
feature: Work Management
source-git-commit: d92908d358ca53ae9d443fd76556e3e8b273e3cb
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 3%

---

# 设置工作角色以进行计费

{{highlighted-preview-article-level}}

通过Workfront，您可以按不同于主要工作角色的工作角色对用户计费。 当某人临时执行应按不同费率计费的工作时，这将很有用。

您可以通过两种方式分配开单的工作角色：

* 在项目级别：当整个项目中的人员应按相同工作角色进行计费时，使用此选项。
* 在分配层：如果要在特定任务上按不同方式开单，请使用此字段。

>[!NOTE]
>
>* 计费工作角色仅适用于人员（用户）。 它不适用于常规工作角色或占位符。
>* 添加工作角色以进行计费只影响计费率，不影响成本。
>* 分配层开单始终优先于项目层开单。

有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)和[创建高级分配](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>标准</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> 编辑对费率卡的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理项目的权限 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在项目层分配工作角色以进行开单

在创建工作角色以对项目计费时：

* 计费角色适用于该项目内该用户的所有任务和分配。
* 计费使用所选工作角色的计费率，但成本仍遵循用户的主要角色。

要在项目层分配工作角色以进行开单，请执行以下操作：

1. 打开一个项目。
1. 在左侧面板中单击&#x200B;**计费资源**。
1. 选择&#x200B;**工作角色以计费**&#x200B;选项卡（如果尚未显示）。
1. 单击&#x200B;**添加>添加工作角色以进行计费**。
1. 在&#x200B;**添加工作角色以进行计费**&#x200B;框中，选择&#x200B;**用户**。
1. 选择&#x200B;**工作角色**&#x200B;用作此项目上此用户计费的工作角色。
1. （可选）单击&#x200B;**添加工作角色**&#x200B;以定义工作角色的有效日期以进行计费。 输入工作角色的&#x200B;**开始**&#x200B;和&#x200B;**结束**&#x200B;日期。

[添加在项目级别计费的工作角色](assets/jrfb-project-level.png)

1. 再次单击&#x200B;**添加工作角色**&#x200B;以指定不同时间段的额外计费角色。
1. 单击&#x200B;**保存**。

### 项目级别的示例

>[!BEGINSHADEBOX]

John的主要工作角色是Designer 1。 这个项目需要一位资深Designer，约翰正在填补。

您应在项目级别将计费工作角色设置为&#x200B;**高级Designer**。

结果：

* 记帐收入是高级Designer费率
* 成本是Designer 1的成本率（John的实际成本率）

>[!ENDSHADEBOX]

## 在分配层分配工作角色以进行开单

在添加工作角色以对分配进行开单时，该设置仅会覆盖该特定分配的项目层开单角色。

要在分配层分配工作角色以进行开单，请执行以下操作：

1. 打开项目并找到任务。
1. 转到任务的&#x200B;**高级工作**。

   有关信息，请参阅[创建高级工作](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md)。

1. 在任务分配网格上，找到列&#x200B;**工作角色以进行计费**。
1. 为每个分配选择一个需要不同开单的工作角色。

   >[!NOTE]
   >
   >如果在项目层分配了开单的工作角色，它将显示在分配中。 您可以单击&#x200B;**工作角色以计费**&#x200B;字段并选择另一个工作角色用于分配。
   >信息图标将通知您在项目层还是分配层定义了开单的工作角色。

   ![工作角色以针对分配计费](assets/jrfb-assignment-level.png)

### 分配层的示例

>[!BEGINSHADEBOX]

John的主要工作角色是Designer 1。 他被列为项目级别的高级Designer，但有一个特殊任务需要主要的Designer收费率。

您只需在该分配上将用于计费的工作角色设置为主要用户Designer。

结果：

* 约翰的其他所有任务都要求作为Designer高级官员
* 此任务记为主要Designer
* 成本仍为Designer 1

>[!ENDSHADEBOX]
