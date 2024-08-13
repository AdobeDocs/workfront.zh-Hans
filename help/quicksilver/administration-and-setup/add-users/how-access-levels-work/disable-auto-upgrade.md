---
title: 对新许可计划中的非付费用户禁用自动升级选项
user-type: administrator
content-type: reference
product-area: system-administration
keywords: 访问，级别，系统，管理员，标准，轻量级，参与者
navigation-topic: access-levels
description: 每个用户都必须具有访问级别，才能在Workfront中登录和工作。 您可以使用访问级别来控制用户可以查看和处理某些Workfront对象和区域的内容。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 1%

---

# 对新许可计划上的非付费用户禁用自动升级选项

对于新计划上的所有未付费Workfront许可证，验证和文档决策受到限制。 当用户达到其分配数量的决策时，默认情况下会升级到轻量级许可证。

您可以从设置区域禁用自动升级选项。 要了解有关自动升级工作方式的更多信息，请参阅[非付费用户的有限文档和验证决策概述](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md)。

>[!IMPORTANT]
>
>禁用后，任何超出分配数量的决策的非付费用户都不会自动升级。

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
   <td>新计划：标准
   <p>或</p>
   <p>当前计划：计划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员。</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## 禁用非付费用户的自动升级

{{step-1-to-setup}}

1. 在左侧导航中展开&#x200B;[!UICONTROL **系统**]，然后单击&#x200B;[!UICONTROL **首选项**]。
1. 在&#x200B;[!UICONTROL **常规首选项**]&#x200B;部分中，选中&#x200B;[!UICONTROL **禁用访问级别内的自动升级**]&#x200B;框。
1. 单击&#x200B;[!UICONTROL **保存**]。
