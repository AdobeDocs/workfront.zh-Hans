---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 编辑和创建风险类型
description: 您可以在计划阶段为项目添加风险，以在批准任何工作之前确定潜在障碍。 风险是可能会阻止项目按时完成或在预算内完成的事件。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 2%

---

# 编辑和创建风险类型

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

您可以在计划阶段为项目添加风险，以在批准任何工作之前确定潜在障碍。 风险是可能会阻止项目按时完成或在预算内完成的事件。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任何</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td><p>新文档： [！UICONTROL Standard]</p>
   或
   <p>当前： [！UICONTROL计划]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td>
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 风险类型

风险类型是用于风险分类的标签，用于对它们进行分类以用于报告目的。 它们由[!DNL Adobe Workfront]管理员在&#x200B;**[!UICONTROL 设置]**&#x200B;区域创建。 在您的&#x200B;**[!UICONTROL 设置]**&#x200B;区域建立风险类型后，它们对于您的系统具有普遍性。 所有项目所有者均可为他们的项目使用相同的风险类型。

## 编辑和创建风险类型

默认情况下，[!DNL Workfront]中已存在某些风险类型。 要反映贵组织的需求，您可以编辑现有的风险类型或创建新风险类型。

* [编辑现有风险类型](#edit-existing-risk-types)
* [创建新的风险类型](#create-new-risk-types)

### 编辑现有风险类型 {#edit-existing-risk-types}

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 风险类型]**。
1. 选择要编辑的风险类型。
1. 单击&#x200B;**[!UICONTROL 编辑]**。
1. （可选）更改风险类型的名称和描述。

   **[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;字段的字符限制为50个字符。

1. 单击&#x200B;**[!UICONTROL 保存更改]。**

### 创建新的风险类型 {#create-new-risk-types}

除了默认风险类型之外，您还可以创建新的风险类型以反映贵组织的需求。

要创建新的风险类型，请执行以下操作：

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 风险类型]**。
1. 单击&#x200B;**[!UICONTROL 新建风险类型]**。
1. 键入风险类型的&#x200B;**[!UICONTROL Name]**（必需）和&#x200B;**[!UICONTROL Description]**（可选）。

   **[!UICONTROL Name]**&#x200B;和&#x200B;**[!UICONTROL Description]**&#x200B;字段的字符限制为50个字符。

1. 单击&#x200B;**[!UICONTROL 创建风险类型]**。 如果您使用内联编辑来添加风险类型，请在完成时单击&#x200B;**[!UICONTROL Enter]**。

   >[!NOTE]
   >
   >如果需要编辑自定义风险类型，请参阅本文中的[[!UICONTROL 编辑现有]风险类型](#edit-existing-risk-types)部分。

## 将风险与项目中的风险类型相附加

风险类型可用于标记添加到项目的风险。 有关如何向项目添加风险的更多信息，请参阅[创建和编辑项目中的风险](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md)。
