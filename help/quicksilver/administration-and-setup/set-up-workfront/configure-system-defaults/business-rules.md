---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: 创建和编辑业务规则
description: 您可以选择按月还是按季度接收新的Workfront功能。
author: Lisa
feature: System Setup and Administration
role: Admin
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d96ddcc2f514d9f79e94a3437a3b66e07a270abc
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# 创建和编辑业务规则

业务规则允许您对Workfront对象应用验证，并阻止用户在满足某些条件时创建、编辑或删除对象。 业务规则通过防止可能会损害数据完整性的操作，帮助提高数据质量和运营效率。

单个业务规则只能分配给一个对象。 例如，如果创建业务规则以在某些条件下不编辑项目，则无法将相同的规则应用于任务。 您必须为任务创建具有相同条件的单独业务规则。

当用户与对象交互时，访问级别和对象共享具有比业务规则更高的优先级。 例如，如果用户具有不允许编辑项目的访问级别或权限，则这些权限将优先于允许在特定条件下编辑项目的业务规则。

将多个业务规则应用于对象时，也会存在层次结构。 例如，您有两个业务规则。 其中一项限制在2月份创建费用。 第二个阻止在项目状态为完成时编辑项目。 如果用户尝试在6月将费用添加到已完成的项目，则无法添加该费用，因为它触发了第二个规则。

业务规则适用于通过API以及在Workfront界面中创建、编辑和删除对象。

>[!NOTE]
>
>由于业务规则会阻止某些操作，因此您应始终首先在沙盒或预览环境中配置业务规则，并在在生产环境中启用它们之前对其进行彻底测试。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具备以下条件才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront计划</td> 
   <td>Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>标准</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>系统管理员</td> 
  </tr>  
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## 业务规则方案

一些简单的业务规则方案包括：

* 用户无法在2月的最后一周添加新费用。 该公式可表述为： `IF(AND(MONTH($$TODAY) = 2, DAYOFMONTH($$TODAY) >= 22), "You cannot add new expenses during the last week of February.")`
* 用户无法编辑处于完成状态的项目。 该公式可表述为： `IF({status} = "CPL", "You cannot edit this project because it is in Complete status.")`

构建业务规则的语法与在自定义表单中构建计算字段的语法相同。 有关语法的更多信息，请参见 [使用表单设计器添加计算字段](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

有关IF语句的信息，请参见 [“IF”语句概述](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) 和 [计算自定义字段中的条件运算符](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

有关基于用户的通配符的信息，请参见 [使用基于用户的通配符对报告进行归纳](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

有关基于日期的通配符的信息，请参阅 [使用基于日期的通配符对报表进行泛化](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

## 添加新业务规则

{{step-1-to-setup}}

1. 单击 **业务规则** 在左侧面板中。
1. 单击 **新业务规则**.
1. 选择要为其分配业务规则的对象类型，然后单击 **继续**.

   ![选择对象](assets/object-for-business-rule2.png)

1. 键入 **名称** 用于业务规则。
1. 在 **处于活动状态** 字段中，选择保存规则时该规则是否应处于活动状态。

   如果您选择 **否**，则规则将另存为不活动，您可以稍后激活它。

1. 选择 **触发器** 用于业务规则。 选项包括：

   * **创建对象时：** 该规则在用户尝试创建对象时应用。
   * **在对象编辑时：** 该规则在用户尝试编辑对象时应用。
   * **对象删除时：** 该规则在用户尝试删除对象时应用。

1. （可选）输入 **描述** 以及应用时会发生什么情况。
1. 在业务规则对话框中心的公式编辑器中构建公式。

   业务规则的格式为“如果满足定义的条件，则禁止用户对该对象执行操作，并显示消息。”

   在公式区域中，您构建的业务规则的部分是条件，以及在满足条件时在Workfront中显示的消息。

   * “对象”是您在创建业务规则时选择的对象类型。 它显示在对话框的标题中。
   * “action”是您为规则选择的触发器：创建、编辑或删除对象。
   * 由于对象和操作已定义，因此不要将它们包含在公式中。
   * 当用户触发业务规则时，向用户显示自定义错误消息。 它应就出现什么问题以及如何纠正问题提供明确的说明。

   ![添加业务规则对话框](assets/add-business-rule-dialog-no-ai-button.png)

   此示例是费用的业务规则。 如果本月是六月，则不允许用户创建新费用，并且消息将对此进行说明。

   有关业务规则的更多示例，请参阅 [业务规则方案](#scenarios-for-business-rules) 本文章中。

1. （可选）使用公式 **表达式** 和 **字段** 帮助构建规则的右侧面板中。

   搜索表达式或字段以缩小可用项列表。

   可用字段列表仅限于与业务规则对象类型相关的字段。

1. 单击 **保存** 在您完成业务规则构建之后。

>[!NOTE]
>
>添加业务规则后，应通过添加、编辑或删除关联对象对其进行测试，以确保正确应用该规则。

## 激活业务规则

当业务规则处于非活动状态时，业务规则列表中的活动字段显示为False。 您不能更新列表视图中规则的状态。

要激活业务规则，请执行以下操作：

1. 在规则列表中选择业务规则并单击编辑图标。
1. 选择 **是** 对象 **处于活动状态** 在业务规则对话框中。
1. 单击&#x200B;**保存**。
