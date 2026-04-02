---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: 管理费率卡
description: 费率卡表示与客户签订的合同协议，合同中为完成工作的工作角色定义了每小时的费率。 在费率卡中，您可以根据属性为每个工作角色定义多个记帐费率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: e5ac8fde409b960aacd3cf7daa0532e9bc3e8121
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 1%

---

# 管理费率卡

{{highlighted-preview-article-level}}

费率卡表示与客户签订的合同协议，合同中为完成工作的工作角色定义了每小时的费率。 在费率卡中，您可以根据代理、位置或成本中心等属性为每个工作角色定义多个计费费率。 您的唯一费率属性在“设置”区域中配置。 有关详细信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

例如，代理机构A的工作角色是驻巴黎的Designer，代理机构B的工作角色是驻巴黎的其他Designer，而驻纽约的第三个Designer的工作角色不是分派给代理机构，每个代理机构的计费率各不相同。 但是，费率卡上的工作角色不需要属性。 属性用作建立更精细速率的工具。 费率卡上的记帐费率也可以是生效日期，以便费率在指定日期开始和结束。

您还可以锁定费率卡上的费率，以防止在项目或任务级别覆盖它们。 锁定费率是记帐费率层次结构中最高的，但项目保留的费率除外。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td>[！UICONTROL标准版]</td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对[！UICONTROL费率卡]的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>要编辑与您共享的费率卡，您必须拥有费率卡的管理权限。</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 添加费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 单击&#x200B;[!UICONTROL **新建费率卡**]，然后单击&#x200B;[!UICONTROL **新建费率卡**]。
1. 在&#x200B;[!UICONTROL **新费率卡**]&#x200B;框中键入费率卡的名称和描述。

   名称必须是唯一的。

   ![新费率卡对话框](assets/new-rate-card-dialog.png)

1. （可选）为费率卡选择&#x200B;[!UICONTROL **组**]。 这是定义费率卡的机构。
1. （可选）为费率卡选择&#x200B;[!UICONTROL **公司**]。 这是签订了费率合同的客户。

   >[!NOTE]
   >
   >本集团及本公司不仅用于费率卡详情，于为项目附加费率卡时亦会作为筛选条件。

1. 单击&#x200B;**创建**。

   此时将显示“费率卡片”>“工作角色和费率”屏幕。

1. 单击&#x200B;[!UICONTROL **添加工作角色**]。
1. 在&#x200B;[!UICONTROL **新记帐费率**]&#x200B;框中，选择&#x200B;[!UICONTROL **工作角色**]&#x200B;以定义其记帐费率。

   ![新建记帐费率对话框](assets/new-job-role-rate-on-rate-card.png)

1. （可选）选择开单费率的属性，如“代理”、“地点”或“成本中心”。

   >[!NOTE]
   >
   >这些属性是单独定义的，可能会影响收入和成本的计算。 有关详细信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

1. 为记帐费率选择&#x200B;[!UICONTROL **货币**]。
1. （可选）输入工作角色的&#x200B;[!UICONTROL **工作角色别名**]。

   如果您键入的别名不存在，则可以添加它。

   将费率卡附加到项目时，别名会出现在占位符分配、费用和报表等信息中，而不是内部工作角色名称中。

   >[!NOTE]
   >
   >* 在单个速率卡中，每个工作角色和属性组合只能有一个别名。
   >* 必须在费率卡上更新别名，并且无法在项目上编辑别名。

1. 在&#x200B;[!UICONTROL **记帐费率**]&#x200B;字段中，输入此工作角色及其属性的记帐费率。
1. （可选）选择&#x200B;[!UICONTROL **锁定速率**]&#x200B;以锁定此速率，不允许在项目或任务级别更改此速率。 如果需要，您可以稍后将其解锁。
1. （可选）单击&#x200B;[!UICONTROL **添加有效日期**]&#x200B;以将有效日期应用于记帐费率。
1. （可选）再次单击&#x200B;[!UICONTROL **添加日期有效费率**]&#x200B;以添加此工作角色及其属性的更多记帐费率（包含有效日期）。
1. （视情况而定）如果要为此工作角色添加多个开单费率，请输入以下信息：

   * [!UICONTROL **记帐费率**]：时间期间的记帐费率值。
   * [!UICONTROL **开始日期**]：费率开始的日期。
   * [!UICONTROL **结束日期**]：费率结束的日期。

     第一个记帐费率不需要有开始日期，最后一个记帐费率不需要有结束日期。 费率日期之间允许存在差异，但不允许日期重叠。 在间隔期间，开单费率层次结构的其他区域用于根据任务的收入类型确定开单费率。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

1. 单击&#x200B;[!UICONTROL **保存**]。
1. （可选）要为具有不同属性的相同工作角色或单独的工作角色添加其他记帐费率，请单击&#x200B;[!UICONTROL **添加工作角色**]。

   每个角色的费率将在您创建费率卡时添加到费率卡中。 基于日期的当前有效费率以图标![当前费率图标](assets/current-rate-icon.png)表示。

   ![显示费率的费率卡](assets/rates-on-rate-card.png)

## 编辑费率卡详细信息和费率

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 要编辑现有的费率卡，请在“费率卡”列表中单击费率卡的名称。
1. 要更新费率卡详细信息，请单击左侧面板中的&#x200B;[!UICONTROL **详细信息**]。
1. （可选）要将自定义表单附加到费率卡，请单击“详细信息”页面右上角的&#x200B;[!UICONTROL **添加自定义表单**]&#x200B;字段，然后从显示的列表中选择自定义表单。

   有关附加自定义表单的详细信息，请参阅[将自定义表单添加到对象](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

1. 编辑费率卡详细信息后，单击&#x200B;[!UICONTROL **保存更改**]。
1. 单击左侧面板中的&#x200B;[!UICONTROL **工作角色和费率**]&#x200B;以编辑计费费率。
1. 要编辑速率，请选中该速率旁边的复选框，然后单击屏幕底部操作栏中的&#x200B;[!UICONTROL **编辑**]。

   有关操作栏的详细信息，请参阅[使用增强列表](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)。

   >[!NOTE]
   >
   >由于每个费率都与角色和属性的组合相关联以创建唯一费率，因此在编辑费率时无法更改角色和属性。

1. 要从费率卡中删除记帐费率，请选中费率旁边的复选框，然后单击操作栏上的&#x200B;[!UICONTROL **删除**]。
1. 要锁定速率，请选中该速率旁边的复选框，然后单击操作栏上的&#x200B;[!UICONTROL **锁定**]。

   无法在项目或任务级别更改锁定费率。 锁定图标显示在列表中的锁定速率旁边。

   您还可以从操作栏解锁锁定率。

1. 要按百分比调整费率，请执行以下步骤：

   1. 在“费率卡”>“工作角色和费率”屏幕中选择要调整的所有费率。

      您可以选择一种费率或多个费率。 所有规则都将按相同的百分比调整。

   1. 在操作栏上单击&#x200B;[!UICONTROL **调整费率**]。
   1. 在&#x200B;[!UICONTROL **调整工作角色费率**]&#x200B;框中，选择是在所选时段（现有有效日期）期间进行费率调整，还是在您定义的自定义日期范围内进行费率调整。

      ![调整工作角色费率框](assets/adjust-job-role-rates-dialog.png)

   1. 输入费率的调整值。

      此值按百分比应用。 例如，如果输入10，则所选费率将增加10%。

   1. 单击&#x200B;[!UICONTROL **更新率**]。
   1. 单击确认消息上的&#x200B;[!UICONTROL **更新**]。

      所选比率会按百分比增加。

## 导入费率卡

请参阅文章[从模板](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md)导入费率卡。

## 复制费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 选中列表中费率卡旁边的复选框，然后单击&#x200B;**复制**&#x200B;图标![复制图标](assets/copy-icon.png)。
1. 在&#x200B;[!UICONTROL **复制费率卡**]&#x200B;框中键入新费率卡的名称。 然后，单击&#x200B;[!UICONTROL **创建**]。

   已保存新的费率卡。 根据需要编辑费率卡详细信息、工作角色和费率。

## 删除整个费率卡

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **费率卡**]。
1. 选中列表中费率卡旁边的复选框，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。

   >[!NOTE]
   >
   >附加到项目的费率卡将从项目中删除。

