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
source-git-commit: a30e505aa2061240f92642fda274be66e4947bce
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 0%

---

# 创建和管理工作角色

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>在25.11版本中，工作角色的覆盖货币已在“生产”中被弃用。 （10月30日，在“预览”环境中弃用。） 工作角色现在可以使用一种货币，而不是使用基本货币和覆盖货币，并且成本和记帐费率使用该货币来定义。

作为[!DNL Adobe Workfront]管理员或对工作角色具有管理访问权限的用户，您可以创建可分配给用户的工作角色，并删除与您的组织无关的默认工作角色。 有关[!DNL Workfront]中管理访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

>[!TIP]
>
>工作角色是管理资源的组成部分。 要使用资源计划工具，工作角色需要与其关联的成本和记帐费率。 有关信息，请参阅[资源管理入门](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td><p>任何</p></td> 
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

1. 在左侧面板中，单击&#x200B;**[!UICONTROL 工作角色]。**
1. 单击&#x200B;**[!UICONTROL 新建工作角色].**
1. 配置以下字段：

   * **名称**：指示工作角色的名称。 该名称会显示Workfront中工作角色字段显示的所有位置。

     >[!TIP]
     >
     >工作角色的名称最多可包含255个字符。 但是，在Workfront的某些区域，较长的名称可能会被截断。

   * **描述**：输入角色的描述，以指示该角色的独特性。
   * **处于活动状态**：如果希望该角色处于活动状态并且在Workfront中的所有位置都可用，以便与用户、工作项等关联，请选择&#x200B;**是**。 如果希望停用该角色且不能将其分配给用户、工作项等，请选择&#x200B;**否**。

     有关停用工作角色的信息，请参阅[停用工作角色](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)。

   * **Currency**：默认显示基本货币。 Workfront管理员在“设置”区域添加基本货币。 您可以将所选内容更改为其他可用货币，也可以更改有效日期时间范围内的货币。

     >[!TIP]
     >
     >此字段仅提供系统中汇率区域中可用的货币。 如果只设置一种货币，则只有该货币可用。

     有关在Workfront中设置基础货币的信息，请参阅[设置汇率](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。

     有关更改项目货币的信息，请参阅[更改项目货币](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)。

   * **成本费率**：这是工作角色的每小时成本费率。 此值计算与角色相关的任务和问题的计划成本和实际成本，并最终计算项目的计划和实际成本。 使用选定币种输入汇率。

     对于日期有效成本费率，请单击&#x200B;**添加费率**。 输入时间期的成本/小时值，并根据需要分配起始日期和终止日期。 第一个成本费率没有起始日期，最后一个成本费率没有终止日期。

     某些日期会自动添加。 例如，如果第一个成本费率没有结束日期，并且您添加了一个起始日期为2025年5月1日的第二个成本费率，则结束日期为2025年4月30日的成本费率将添加到第一个成本费率中，这样就不会存在任何差距。

     有关Workfront如何计算成本的信息，请参阅[跟踪成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

     >[!TIP]
     >
     >编辑现有工作角色时，您可以对列表进行排序，以在费率列表顶部查看最近的开始日期。

   * **记帐费率**：这是工作角色的每小时记帐费率。 此值计算与角色相关的任务和问题的计划收入和实际收入，最终计算项目的计划收入和实际收入。 使用选定币种输入汇率。

     对于日期有效记帐费率，请单击&#x200B;**添加费率**。 输入时间期的记帐/小时值，并根据需要分配起始日期和终止日期。 第一个记帐费率没有开始日期，最后一个记帐费率没有结束日期。

     某些日期会自动添加。 例如，如果第一个记帐费率没有结束日期，而您添加第二个记帐费率的开始日期为2025年5月1日，则结束日期为2025年4月30日将添加到第一个记帐费率，这样就不会存在任何间隔。

     有关Workfront如何计算收入的信息，请参阅[账单和收入概述](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)。

     >[!TIP]
     >
     >编辑现有工作角色时，您可以对列表进行排序，以在费率列表顶部查看最近的开始日期。

1. 单击&#x200B;**[!UICONTROL 创建工作角色]**。 工作角色现在可以分配给任务、问题、批准，或者您可以与其共享布局模板或其他对象。 有关[!DNL Workfront]中所有工作角色用途的信息，请参阅[工作角色概述](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)。 有关删除工作角色的信息，请参阅[删除工作角色](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)。

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


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->



