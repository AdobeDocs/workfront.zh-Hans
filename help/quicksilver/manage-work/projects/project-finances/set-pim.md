---
product-area: projects
navigation-topic: financials
title: 设置性能索引方法(PIM)
description: 项目的绩效指数方法(PIM)控制Adobe Workfront用于计算项目绩效指标的方法，例如成本绩效指数(CPI)、成本计划绩效指数(CSI)、计划绩效指数(SPI)和完成时估计(EAC)。
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 1%

---

# 设置性能索引方法(PIM)

项目的绩效指数方法(PIM)控制Adobe Workfront用于计算项目绩效指标的方法，例如成本绩效指数(CPI)、成本计划绩效指数(CSI)、计划绩效指数(SPI)和完成时估计(EAC)。

Workfront会使用以下方法计算这些值：

* 小时
* 成本

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
   <td> <p>编辑对项目和财务数据的访问</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理项目的权限，并具有管理财务的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 关于Workfront中PIM的注意事项

* 您的Workfront管理员或组管理员将设置默认值，以确定性能索引方法(PIM)应基于小时还是基于成本。 性能量度的计算会根据此默认值的设置方式而发生变化。 有关如何更改如何计算PIM的默认值的更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* 项目经理还可以在项目层更改项目“财务”子标签中各个项目的PIM设置。 您必须具有项目的“管理”权限，才能编辑项目的“财务”子选项卡。

## 为项目设置性能索引方法(PIM)

1. 转到您所有者的项目。

   >[!IMPORTANT]
   >
   >您需要对项目的“管理”权限才能执行以下步骤。 我们还建议，只有项目所有者才应该更改项目的“财务”区域。

1. 单击 **项目详细信息** ，然后转到 **金融** 的上界。
1. 双击 **性能指数方法** 字段进行编辑。
1. 从 **性能指数方法** 字段：

   | 基于小时 | Workfront在计算项目的CPI和EAC时使用计划小时，项目的EAC显示为数字（以小时为单位）。 |
   |---|---|
   | 基于成本 | Workfront在计算项目的CPI和EAC时使用计划人工成本，EAC显示为货币值。 选择此选项时，请确保任务分配人（职务角色或用户）与成本费率关联。 |

   {style=&quot;table-layout:auto&quot;}

1. 单击 **保存** **更改**.
