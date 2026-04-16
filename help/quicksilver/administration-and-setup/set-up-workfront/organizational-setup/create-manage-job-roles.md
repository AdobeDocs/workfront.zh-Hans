---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 创建和管理职位角色
description: 作为 [!DNL Adobe Workfront] 管理员或对工作角色具有管理访问权限的用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: df1d844346d7ed26dcb004ba1a10ec9e8d07422a
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 1%

---

# 创建和管理工作角色

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>在25.11版本中，工作角色的覆盖货币已在“生产”中被弃用。 （10月30日，在“预览”环境中弃用。） 工作角色现在可以使用一种货币，而不是使用基本货币和覆盖货币，并且成本和记帐费率使用该货币来定义。

作为[!DNL Adobe Workfront]管理员或具有工作角色编辑权限的标准用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。 有关[!DNL Workfront]中管理访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

>[!TIP]
>
>工作角色是管理资源的组成部分。 要使用资源计划工具，工作角色需要与其关联的成本和记帐费率。 有关信息，请参阅[资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>创建或编辑工作角色：任何Workfront或工作流包</p>
   <p>要应用费率属性并将自定义表单添加到工作角色，请执行以下操作：工作流Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td><p>[！UICONTROL标准版]</p>
       <p>[！UICONTROL计划]</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>对工作角色的管理访问权限</td>
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建工作角色

要创建工作角色，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 工作角色]**。
1. 单击&#x200B;**[!UICONTROL 新建工作角色] >新建工作角色**。
1. 在以下字段中输入信息：

   * **名称**：指示工作角色的名称。 该名称会显示Workfront中工作角色字段显示的所有位置。

     >[!TIP]
     >
     >工作角色的名称最多可包含255个字符。 但是，在Workfront的某些区域，较长的名称可能会被截断。

   * **描述**：输入角色的描述，以指示该角色的独特性。
   * **处于活动状态**：如果希望该角色处于活动状态并且在Workfront中的所有位置都可用，以便与用户、工作项等关联，请选择&#x200B;**是**。 如果希望停用该角色且不能将其分配给用户、工作项等，请选择&#x200B;**否**。

     有关停用工作角色的信息，请参阅[停用工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

1. 单击&#x200B;**[!UICONTROL 创建工作角色]**。 工作角色现在可以分配给任务、问题、批准，或者您可以与其共享布局模板或其他对象。 有关[!DNL Workfront]中所有工作角色用途的信息，请参阅[工作角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。 有关删除工作角色的信息，请参阅[删除工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)。

## 将费率和属性添加到工作角色

工作角色的计费和成本费率用于财务计算。

存在费率的Workfront区域（如工作角色和用户）支持费率属性。 对工作角色应用属性后，其分配会自动解析为正确的费率。

有关详细信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 工作角色]**。
1. 单击现有工作角色的名称以对其进行编辑。
1. 要更新工作角色详细信息，请单击左侧面板中的&#x200B;**详细信息**。
1. （可选）要将自定义表单附加到工作角色，请单击“详细信息”页面右上角的&#x200B;**添加自定义表单**&#x200B;字段，然后从显示的列表中选择自定义表单。

   有关附加自定义表单的详细信息，请参阅[将自定义表单添加到对象](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)。

1. 单击左侧面板中的&#x200B;[!UICONTROL **费率**]。
1. 单击&#x200B;[!UICONTROL **计费**]&#x200B;或&#x200B;[!UICONTROL **成本**]&#x200B;以选择费率类型。
1. 单击&#x200B;[!UICONTROL **添加费率**]&#x200B;以添加新费率。

   或

   选择现有费率，然后单击&#x200B;**编辑**&#x200B;图标![编辑图标](assets/edit-icon.png)进行更新。

   >[!NOTE]
   >
   >由于每个费率都与角色和属性的组合相关联以创建唯一费率，因此在编辑费率时无法更改属性。

1. 在&#x200B;**新费率**&#x200B;框中，选择费率属性，例如“代理”、“地点”或“成本中心”。

   >[!NOTE]
   >
   >这些属性是单独定义的，可能会影响收入和成本的计算。 有关详细信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。

1. 为汇率选择&#x200B;**货币**。 Workfront管理员在“设置”区域添加基本货币。 您可以将所选内容更改为其他可用货币，也可以更改有效日期时间范围内的货币。

   >[!TIP]
   >
   >此字段仅提供系统中汇率区域中可用的货币。 如果只设置一种货币，则只有该货币可用。

   有关在Workfront中设置基础货币的信息，请参阅[设置汇率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

   有关更改项目货币的信息，请参阅[更改项目货币](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)。

1. （视情况而定）对于记帐费率，输入此工作角色的&#x200B;**记帐费率**。

   这是工作角色的每小时记帐费率。 此值计算与角色相关的任务和问题的计划收入和实际收入，最终计算项目的计划收入和实际收入。 使用选定币种输入汇率。

   如果使用属性，则属性和工作角色将组合起来定义唯一费率。 例如，A代理人在纽约的Designer角色可以与B代理人在巴黎的Designer角色具有不同的费率。

   对于日期有效记帐费率，请单击&#x200B;**添加费率**。 输入时间期的记帐/小时值，并根据需要分配起始日期和终止日期。 第一个记帐费率没有开始日期，最后一个记帐费率没有结束日期。

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   Workfront允许您在日期范围之间留下空白，但您将收到一则警告，确认这是有意为之。

   有关Workfront如何计算收入的信息，请参阅[账单和收入概述](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)。

   >[!TIP]
   >
   >编辑现有工作角色时，您可以对列表进行排序，以在费率列表顶部查看最近的开始日期。

1. （视情况而定）对于成本费率，输入此工作角色的&#x200B;**成本费率**。

   这是工作角色的每小时成本率。 此值计算与角色相关的任务和问题的计划成本和实际成本，并最终计算项目的计划和实际成本。 使用选定币种输入汇率。

   如果使用属性，则属性和工作角色将组合起来定义唯一费率。 例如，A代理人在纽约的Designer角色可以与B代理人在巴黎的Designer角色具有不同的费率。

   对于日期有效成本费率，请单击&#x200B;**添加费率**。 输入时间期的成本/小时值，并根据需要分配起始日期和终止日期。 第一个成本费率没有起始日期，最后一个成本费率没有终止日期。

   某些日期会自动添加。 例如，如果第一个成本费率没有终止日期，并且您添加了一个起始日期为5月1日的第二个成本费率，则终止日期为4月30日将添加至第一个成本费率，因此不存在任何间隔。

   有关Workfront如何计算成本的信息，请参阅[跟踪成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

   >[!TIP]
   >
   >编辑现有工作角色时，您可以对列表进行排序，以在费率列表顶部查看最近的开始日期。

1. 单击&#x200B;[!UICONTROL **保存**]。

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



