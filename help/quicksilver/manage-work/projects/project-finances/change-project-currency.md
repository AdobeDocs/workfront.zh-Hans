---
product-area: projects
navigation-topic: financials
title: 更改项目货币
description: 作为项目经理，您可以将项目配置为使用Adobe Workfront系统默认货币以外的货币。 这允许您在计算人工成本和收入时以所需货币显示项目的财务信息。
author: Alina
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 更改项目货币

作为项目经理，您可以将项目配置为使用Adobe Workfront系统默认货币以外的货币。 这允许您在计算人工成本和收入时以所需货币显示项目的财务信息。

在您使用本节所述的替代货币之前，Workfront管理员必须首先启用并配置多种货币，如文章所述 [设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 在Workfront中更改项目货币时的注意事项

* 如果项目中包含任何财务信息，则无法更改项目的货币。
* 用于人工成本的费率；收入计算，并于未来用作报告用途。
* 如果您没有为项目指定其他货币，则Workfront会假定项目的货币是系统的默认货币。 有关系统级别默认货币的信息，请参阅 [设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* 默认情况下，所有完全许可证用户都有权查看货币和汇率。 Workfront管理员需要为 **汇率** 以允许用户设置项目的特定费率。
* Workfront的汇率并非动态的。 该值由管理员设置，并且必须在汇率发生更改时进行更新。
* 在创建报表以反映项目上的货币时，默认情况下，所有报表都会按项目的默认货币进行分组。 如果您创建的报表包含多个具有不同汇率的项目，则应用于该项目的任何分组都反映系统级别的默认汇率。 有关更多信息，请参阅文章 [使用独特的汇率创建财务数据报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## 配置项目的货币

1. 转到要更改默认货币的项目。

   >[!TIP]
   >
   >确保项目没有任何财务信息。 例如，确保没有与项目关联的计划成本或实际成本。

1. 单击 **项目详细信息** ，然后转到 **金融** 的上界。
1. 单击 **添加** 在 **货币** 字段，然后选择要用作项目默认货币的货币。 将显示Workfront管理员为Workfront实例设置的所有货币。

   ![](assets/currency-on-project-expanded-nwe.png)

1. （视情况而定）如果您选择的货币不是为Workfront系统设置的默认货币，请指定所选货币的汇率，因为它与系统中设置为基本货币的货币相关。
1. 单击 **保存更改**.
