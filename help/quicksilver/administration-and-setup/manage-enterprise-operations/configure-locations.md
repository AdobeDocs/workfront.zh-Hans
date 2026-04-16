---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 配置位置
description: 您可以配置默认位置，以便在费率卡中将其指定为工作角色的属性。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 69233499-fbcb-44a4-a247-d5051f9bc8b9
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 5%

---

# 配置位置

您可以配置默认位置，以便在费率卡中将其指定为工作角色的属性。 这可确保费率卡准确反映每个位置的市场费率。

费率卡允许贵组织轻松管理项目的计费费率。 有关详细信息，请参阅[管理费率卡](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL 标准版]</td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 添加位置

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **位置**]。
1. 单击列表底部的&#x200B;[!UICONTROL **添加更多位置**]。
1. 输入地点名称和说明。
1. 单击输入区域外部以保存位置。
1. 要删除某个位置，请在列表中选择该位置，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/delete.png)。

>[!NOTE]
>
>无法删除与费率卡上的工作角色关联的位置。

## 添加子位置

可以将子位置添加到现有位置。 例如，如果您已经在英国有一个位置，则伦敦可以是子位置。

允许使用三个级别的子位置。 国家/地区、省/市/自治区以及城市是子位置的常见用法。

每个子位置都可以作为属性添加到费率卡上，其方式与顶级位置相同，以便为该位置的特定工作角色定义费率。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;[!UICONTROL **位置**]。
1. 选择列表中的现有位置，然后单击&#x200B;**添加子位置**。
1. 输入地点名称和说明。
1. 单击输入区域外部以保存位置。

   子位置缩进到顶层位置下。

   ![位置和子位置](assets/locations-sublocations.png)


