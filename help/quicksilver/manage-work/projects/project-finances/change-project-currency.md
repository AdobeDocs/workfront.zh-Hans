---
product-area: projects
navigation-topic: financials
title: 更改项目货币
description: 作为项目经理，您可以将项目配置为使用Adobe Workfront系统默认货币以外的货币。 这样，您就可以在计算人工成本和收入时，按所需的货币显示项目的财务信息。
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
source-git-commit: e5a87b92bf1f6c2e0485ba8a2eb73e52c422b2fc
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# 更改项目货币

作为项目经理，您可以将项目配置为使用Adobe Workfront系统默认货币以外的货币。 这样，您就可以在计算人工成本和收入时，按所需的货币显示项目的财务信息。

使用本节所述的备用货币之前，Workfront管理员必须先启用并配置多个货币，如[设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)一文中所述。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准</p>
   <p>或</p>
   <p>当前：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>编辑对项目的访问权限</td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td>管理项目的权限</td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 在Workfront中更改项目货币时的注意事项

* 如果项目中存在任何财务信息，则无法更改项目的货币。
* 比率用于劳工成本；收入计算，并用于未来报告目的。
* 如果没有为项目指定其他货币，Workfront会假定项目的货币是系统的默认货币。 有关系统级别默认货币的信息，请参阅[设置汇率](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)。
* 默认情况下，所有完全许可用户都有权查看货币和汇率。 Workfront管理员需要授予&#x200B;**汇率**&#x200B;的附加管理权限，以允许用户设置项目的特定汇率。
* Workfront的汇率并非动态的。 该值由管理员设置，并且必须在汇率发生更改时更新。
* 在创建报告以在项目上反映货币时，默认情况下，所有报告按项目的默认货币分组。 如果您创建一个报表，其中多个项目的汇率不同，则应用于该项目的任何组都会反映系统级别的默认汇率。 有关详细信息，请参阅文章[创建具有唯一汇率的财务数据报表](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)。

## 配置项目的货币

1. 转到要更改默认货币的项目。

   >[!TIP]
   >
   >确保项目还没有任何财务信息。 例如，确保没有与项目相关的计划或实际成本。

1. 单击左侧面板中的&#x200B;**项目详细信息**，然后转到&#x200B;**财务**&#x200B;区域。
1. 单击&#x200B;**货币**&#x200B;字段中的&#x200B;**添加**，然后选择要用作项目默认货币的货币。 显示Workfront管理员为Workfront实例设置的所有货币。

   ![](assets/currency-on-project-expanded-nwe.png)

1. （视情况而定）如果您选择的货币不是为Workfront系统设置的默认货币，请指定所选货币的汇率，因为该汇率与系统中设置为基础货币的货币相关。
1. 单击&#x200B;**保存更改**。
