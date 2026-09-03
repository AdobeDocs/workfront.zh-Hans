---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 覆盖公司级别的工作角色记帐费率
description: 创建工作角色后，您可以选择为该角色选择每小时记帐费率。 您可以创建特定于公司的每小时记帐费率。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ee60987e-78b5-4853-9a4f-e44aa7a81c05
TQID: https://experienceleague.adobe.com/EbnybXqWehstH2ziLqNZfMHtarMvUiugvWioYv9wLds
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 8c08e110aeccdf6d6416fd1070fbcbd40fd46983
workflow-type: tm+mt
source-wordcount: 857
ht-degree: 2%

---

# 覆盖公司级别的工作角色记帐费率

{{preview-fast-release-general}}

创建工作角色后，您可以选择为该角色选择每小时记帐费率。 您可以创建特定于公司的多个小时记帐费率。 每个记帐费率在特定日期范围内有效。

在项目级别，您可以启用一个选项，以允许公司级别的记帐费率覆盖项目级别的费率。 有关详细信息，请参阅[用公司级别的记帐费率覆盖项目级别的记帐费率](../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>要将费率属性添加到公司层开单费率，请执行以下操作：工作流Ultimate</p>
       <p>要创建公司级别的记帐费率并编辑所有其他费率设置：任何Workfront或工作流包</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL标准版]</p>
       <p>[！UICONTROL计划]</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td> <p>如果您不是系统管理员，则可以管理对公司的访问权限</p>
   <p>编辑对财务数据的访问权限</p> </td>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 覆盖或更改用于特定工作角色的已建立记帐费率

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 公司]**。
1. 找到分配工作角色的公司。
1. 单击列表中的公司名称。
1. 单击左侧面板中的&#x200B;**[!UICONTROL 记帐费率]**。
1. 单击&#x200B;**[!UICONTROL 添加记帐费率] > [!UICONTROL 新记帐费率]**，或单击&#x200B;<span class="preview">**添加记帐费率**</span>。
1. 在[!UICONTROL 新建记帐费率]对话框中，选择&#x200B;[!UICONTROL **工作角色**]&#x200B;以定义其记帐费率。

### 在生产环境中：

[!UICONTROL **默认记帐费率**]&#x200B;显示此工作角色的系统级别费率。

![新建记帐费率对话框](assets/date-effective-billing-rates-for-company.png)

1. 在&#x200B;[!DNL **记帐费率1**]&#x200B;字段中输入记帐费率。 然后，单击&#x200B;[!UICONTROL **保存**]&#x200B;以一次性覆盖记帐费率。

   或

   单击&#x200B;[!UICONTROL **添加费率**]&#x200B;以添加更多具有有效日期的记帐费率。

1. （视情况而定）如果要添加多个开单费率，请输入以下信息：

   * **[!UICONTROL 记帐费率1]、2等。**：时间段的记帐费率值。
   * **[!UICONTROL 开始日期]**：费率生效的日期。
   * **[!UICONTROL 结束日期]**：费率结束的日期。

     记帐费率1没有开始日期，最后一个记帐费率没有结束日期。 某些日期会自动添加。 例如，如果记帐费率1没有结束日期，并且您添加开始日期为2023年5月1日的记帐费率2，则结束日期为2023年4月30日将添加到记帐费率1，这样不存在间隔。

1. 单击&#x200B;[!UICONTROL **保存**]。

   >[!NOTE]
   >
   >项目上工作角色费率的更改将仅影响该项目。 公司级别的费率更改将影响所有项目。 有关详细信息，请参阅[覆盖记帐费率和计算项目收入的概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

<div class="preview">

### 在“预览”环境中：

1. 选择费率属性，如机构、地点或成本中心。

   这些属性是单独定义的，可能会影响收入和成本的计算。 有关详细信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

   ![新建记帐费率对话框](assets/company-billing-rates-090326.png)

1. 为汇率选择&#x200B;**货币**。 Workfront管理员在“设置”区域添加基本货币。 您可以将所选内容更改为其他可用货币，也可以更改有效日期时间范围内的货币。

   >[!TIP]
   >
   >此字段仅提供系统中汇率区域中可用的货币。 如果只设置一种货币，则只有该货币可用。

   有关在Workfront中设置基础货币的信息，请参阅[设置汇率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

   有关更改项目货币的信息，请参阅[更改项目货币](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)。

1. 在&#x200B;[!DNL **记帐费率**]&#x200B;字段中输入工作角色的记帐费率。

   这是工作角色的每小时记帐费率。 此值计算与角色相关的任务和问题的计划收入和实际收入，最终计算项目的计划收入和实际收入。 使用选定币种输入汇率。

   如果使用属性，则属性和工作角色将组合起来定义唯一费率。 例如，A代理人在纽约的Designer角色可以与B代理人在巴黎的Designer角色具有不同的费率。

   对于日期有效记帐费率，单击&#x200B;**添加日期有效费率**。 输入时间期的每小时开单费率，并根据需要分配起始日期和终止日期。 第一个记帐费率没有开始日期，最后一个记帐费率没有结束日期。

   Workfront允许您在日期范围之间留下空白，但您将收到一则警告，确认这是有意为之。

   有关Workfront如何计算收入的信息，请参阅[账单和收入概述](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)。

   >[!TIP]
   >
   >编辑现有费率时，您可以对列表进行排序，以在费率列表的顶部查看最近的开始日期。

1. 单击&#x200B;[!UICONTROL **保存**]。

   >[!NOTE]
   >
   >项目上工作角色费率的更改将仅影响该项目。 公司级别的费率更改将影响公司分配的所有项目。 有关详细信息，请参阅[覆盖记帐费率和计算项目收入的概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

</div>

