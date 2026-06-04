---
product-area: projects
navigation-topic: financials
title: 设置绩效指数方法(PIM)
description: 项目的绩效指数方法(PIM)控制Adobe Workfront用于计算项目绩效指标的方法，例如成本绩效指数(CPI)、成本计划绩效指数(CSI)、计划绩效指数(SPI)和完工估算(EAC)。
author: Lisa
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
TQID: https://experienceleague.adobe.com/g4FYe8k1psS9xuL6Z40teAyJ-SV4UD6ThnWvnvl8au4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 418
ht-degree: 5%

---

# 设置绩效指数方法(PIM)

项目的绩效指数方法(PIM)控制Adobe Workfront用于计算项目绩效指标的方法，例如成本绩效指数(CPI)、成本计划绩效指数(CSI)、计划绩效指数(SPI)和完工估算(EAC)。

Workfront使用以下方式计算这些值：

* 小时
* 成本

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>“任一” </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对项目和财务数据的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理具有编辑General Finance权限的项目权限</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于Workfront中PIM的注意事项

* 您的Workfront管理员或组管理员将设置绩效指数方法(PIM)是基于小时还是基于成本的默认值。 性能量度的计算会根据此默认值的设置而变化。 有关如何更改计算PIM的默认值的详细信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 项目经理还可以在项目的“财务”子标签中更改单个项目的PIM设置。 您必须具有项目的“管理”权限才能编辑项目的“财务”子选项卡。

## 为项目设置绩效指数方法(PIM)

1. 转到您拥有的项目。

   >[!IMPORTANT]
   >
   >您需要具有项目管理权限才能执行以下步骤。 我们还建议仅项目所有者应对项目的财务区域进行更改。

1. 单击左侧面板中的&#x200B;**项目详细信息**，然后转到&#x200B;**财务**&#x200B;区域。
1. 双击&#x200B;**绩效指数方法**&#x200B;字段中的值以进行编辑。
1. 从&#x200B;**绩效指数方法**&#x200B;字段中的以下选项中选择：

   | 基于小时 | Workfront使用计划小时数来计算项目的CPI和EAC，并且项目的EAC显示为数字（以小时为单位）。 |
   |---|---|
   | 基于成本 | Workfront使用计划劳力成本计算项目的CPI和EAC，并且EAC显示为货币值。 选择此选项时，请确保您的任务受分配人（职位角色或用户）与成本费率相关联。 |

   {style="table-layout:auto"}

1. 单击&#x200B;**保存** **更改**。
