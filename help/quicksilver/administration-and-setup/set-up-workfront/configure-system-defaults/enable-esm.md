---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 为您的组织启用Adobe企业存储
description: 您可以为贵企业启用Adobe企业级存储，以便为所有Adobe产品使用统一存储解决方案。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 97c351ca38a8b6075634b2f755f2330562bc8b52
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 7%

---

# 为您的组织启用Adobe企业存储

Adobe企业存储是一个适用于所有Adobe产品的统一存储解决方案。 它是一个基于云的存储解决方案，用作Adobe企业产品中资产的中央存储库。

默认情况下，新客户将启用Adobe企业存储，而现有客户在续订合同后也可启用。

有关Adobe企业存储的详细信息，请参阅[Adobe企业存储概述](/help/quicksilver/review-and-approve-work/esm-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront包</td> 
   <td><p>“任一”</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是Workfront管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为您的组织启用Adobe企业存储

要为您的组织启用Adobe企业存储，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**首选项**。
1. 向下滚动到&#x200B;**存储首选项**&#x200B;部分。
1. 在“默认”下拉菜单中，选择&#x200B;**Adobe企业存储**。
1. （可选）如果要使用Adobe企业级存储和旧版Workfront存储的组合，请选中&#x200B;**允许用户选择存储提供程序**&#x200B;复选框。

   >[!NOTE]
   >
   >启用此选项允许用户在创建新项目时选择存储提供程序。 企业存储标记为“新项目”，因为它是默认的存储提供商。 旧版Workfront存储已标记为“旧版项目”。
   >
   >![新项目和旧项目选项](assets/new-esm-project.png)

1. 单击&#x200B;**保存**。