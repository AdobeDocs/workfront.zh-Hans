---
title: 将费率卡附加到项目
description: 在项目附上费率卡后，按地点及其关联记帐费率列出的所有角色都将添加到项目中。
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 58d3f084c343bcc404f30edd270017fa5f86eb58
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 3%

---

# 将费率卡附加到项目

{{highlighted-preview-article-level}}

费率卡根据属性存储每个工作角色的多个记帐费率。 例如，代理机构A的工作角色是驻巴黎的Designer，代理机构B的工作角色是驻巴黎的其他Designer，而驻纽约的第三个Designer的工作角色不是分派给代理机构，每个代理机构的计费率各不相同。 但是，费率卡上的工作角色不需要属性。 属性用作建立更精细速率的工具。 费率卡上的记帐费率也可以是生效日期，以便费率在指定日期开始和结束。

在项目附上费率卡后，所有角色及其关联的记帐费率都将添加到项目中。

>[!NOTE]
>
>附加费率卡会覆盖项目上任何现有的费率卡记帐费率。 直接添加到项目的记帐费率覆盖不会删除。

有关创建费率卡的信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

有关覆盖项目的工作角色记帐费率和计算项目收入的一般信息，请参阅[覆盖记帐费率和计算项目收入的概述](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)。

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
   <td>编辑对项目、财务数据和费率卡的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td>管理具有编辑计费费率权限的项目权限</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将费率卡附加到项目

1. 转到项目。
1. 单击左侧面板中的&#x200B;**费率**，然后选择&#x200B;**帐单**。
1. 单击&#x200B;**添加记帐费率>附加费率卡**。

   将打开&#x200B;**附加费率卡**&#x200B;框。 您可以在列表中搜索费率卡。

   ![附加费率卡盒](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >费率卡上的组和公司用作此列表上的筛选器。 由于项目也包含“组”和“公司”字段，因此Workfront使用这些值将可用费率卡列表缩小到与项目上下文相关的那些字段，而不是整个系统中的所有费率卡。
   >
   >匹配项不一定是准确的。 带有空白组和/或公司值的费率卡可能仍会出现，具体取决于项目的组/公司配置。 例如，如果项目选择了组但公司为空，您可能会看到与该组关联的费率卡，即使费率卡的公司不同或为空。

1. 选择要添加到项目的费率卡，然后单击&#x200B;**附加**。

   费率卡及其所有工作角色费率将添加到计费费率列表。

   ![将评价卡添加到项目](assets/rate-card-on-project.png)

## 从项目中删除费率卡

从项目中删除费率卡时，将删除其所有工作角色费率。 您无法从项目中移除来自费率卡的单个费率。

您可以删除直接添加到项目中的用户或工作角色的记帐费率覆盖，而无需删除整个费率卡。

1. 转到项目。
1. 单击左侧面板中的&#x200B;**费率**，然后选择&#x200B;**帐单**。
1. 单击&#x200B;**删除**&#x200B;图标![删除图标](assets/remove-icon.png)。
1. 单击确认消息上的&#x200B;**确认**&#x200B;以删除费率卡。

