---
content-type: overview
product-area: projects
navigation-topic: financials
title: 覆盖项目层的用户成本费率
description: 本文介绍了如何覆盖项目的系统用户成本费率。
author: Lisa
feature: Work Management
exl-id: ff1110fd-2d24-48a7-8000-712e551ca61a
source-git-commit: e3d4ffe2d42f9de3000df0ba1a924ca36fea9248
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 3%

---

# 覆盖项目级别的用户成本率

您可以指定特定项目中的用户的成本费率。 此项目层成本费率将覆盖此用户系统层的成本费率。 Workfront使用工作角色的项目层成本费率来计算成本，而不使用系统层成本费率。

本文介绍了如何覆盖项目的系统用户成本费率。

有关计算项目成本的更多信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)和[跟踪成本](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)。

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
   <td> <p>编辑对项目和财务数据的访问权限</p>
       <p><p>您还必须具有下列任一属性：</p> 
        <ul> 
          <li> <p>系统管理员访问级别。 </li> 
          <li> <p>访问级别中的<b>用户</b>设置配置为<b>编辑</b>访问，其中<b>创建</b>以及<b>微调设置</b> <b>下至少启用</b>用户管理员<img src="assets/gear-icon-in-access-levels.png">选项之一。 </p> <p>在这两个选项中，如果启用了<b>用户管理员（组用户）</b>，您必须是该用户所属组的组管理员。</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理包含编辑成本费率的项目权限 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

用户必须在其用户配置文件中启用&#x200B;**允许成本费率覆盖**&#x200B;字段。 当用户未启用“成本改写”字段时，不允许该用户在任何项目上进行成本改写，并且系统使用用户配置文件上的费率来计算成本。

有关详细信息，请参阅[编辑用户配置文件](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)。

## 覆盖项目级别的用户成本率

1. 转至要覆盖成本率的项目。
1. 单击左侧面板中的&#x200B;**费率**。 您可能需要先单击&#x200B;**显示更多**。
1. 单击&#x200B;**成本**&#x200B;选项卡（如果尚未选择）。
1. 单击&#x200B;**添加成本费率** > **新用户成本费率**。

   此时将打开“新建用户成本费率”框。

1. 在&#x200B;**用户**&#x200B;字段中，选择要更改其成本费率的用户。
1. 为成本费率覆盖选择&#x200B;**货币**。
1. 在&#x200B;**成本费率**&#x200B;字段中，输入第一个成本费率覆盖。
1. （可选）单击&#x200B;**添加日期有效费率**&#x200B;以添加更多成本费率覆盖。

   >[!NOTE]
   >
   >如果输入单个费率改写，它将适用于项目的整个生命周期。
   >如果您希望在一段时间内具有不同的费率，则可以添加多个生效日期覆盖。

1. （视情况而定）如果要添加多个成本费率改写，请为每个行指定以下信息：

   * **成本费率**：指定时间段内的成本费率的值。
   * **开始日期**：成本费率覆盖开始的日期。
   * **结束日期**：成本费率覆盖结束的日期。

   ![新用户成本费率框显示有效日期](assets/new-user-cost-rate-box.png)

   在计算项目成本时，Workfront会将覆盖工作角色费率应用于这些时间范围内发生的小时数。

   Workfront允许您在覆盖时间范围之间保留间隔，但您将收到一则警告消息，确认这是有意为之。

   您无需为第一个覆盖率指定开始日期，也不需要为最后一个覆盖率指定结束日期。

   我们建议您为第一个覆盖率使用默认覆盖率。

   Workfront假定第一个覆盖率适用于日期早于第一个覆盖的结束日期的所有小时，最后一个覆盖率适用于日期早于最后一个覆盖的开始日期的所有小时。

   如果在项目的计划开始日期之前记录了一个小时，则使用第一个成本率。

   如果在项目的计划完成日期后记录了一个小时，则使用最后的成本率。

1. 单击&#x200B;**保存**。
