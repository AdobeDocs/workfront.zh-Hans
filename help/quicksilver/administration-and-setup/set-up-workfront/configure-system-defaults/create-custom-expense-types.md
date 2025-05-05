---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 创建自定义费用类型
description: 作为 [!DNL Adobe Workfront] 管理员，您可以创建自定义费用类型以定义和跟踪与任务和项目关联的费用。 费用是可与任务或项目关联的非人工成本。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 428e6a9365c793ce5944941ec5368a674c208c78
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 4%

---

# 创建自定义费用类型

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为[!DNL Adobe Workfront]管理员，您可以创建自定义费用类型以定义和跟踪与任务和项目关联的费用。 费用是可与任务或项目关联的非人工成本。

您可以编辑或删除您创建的任何费用类型。 您无法删除或编辑内置[!DNL Workfront]费用类型。

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
   <td><p>新文档： [!UICONTROL Standard]</p>
   或
   <p>当前： [!UICONTROL 计划]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>[!UICONTROL 系统管理员]</td>
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 默认费用类型

[!DNL Workfront]中无法删除或编辑的默认费用类型包括：

* [!UICONTROL Advertising]
* [!UICONTROL 咨询]
* [!UICONTROL 娱乐]
* [!UICONTROL 常规]
* [!UICONTROL 材料]
* [!UICONTROL 旅游]

## 创建自定义费用类型

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 费用类型]**。
1. 单击&#x200B;**[!UICONTROL 新建费用类型]**。
1. 在&#x200B;**[!UICONTROL 新建费用类型]**&#x200B;对话框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名称]</td> 
      <td>指定支出的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 描述]</td> 
      <td>指定费用的描述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 计算单位]</td> 
      <td> <p>从下拉列表中选择费用类型的度量单位。</p> <p>可使用以下测量单位：</p> 
       <ul> 
        <li>英里</li> 
        <li>千米</li> 
        <li>千克</li> 
        <li>美元</li> 
        <li>美元</li> 
        <li>天</li> 
        <li>其他 — 选择此选项将提示您命名度量单位，并将度量单位定义为组织所熟悉的单位。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费率</td> 
      <td> <p>指定单价。 这是一个货币格式字段，它表示在<strong>[!UICONTROL 计算单位]</strong>字段中建立的每个单位的成本。 </p> <p>比率可以包含小数点后最多4个数字的数值。 例如，1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**[!UICONTROL 保存]**。

   费用类型现在可供用户将其与他们在项目和任务中的费用相关联。

## 修改自定义费用类型

{{step-1-to-setup}}

1. 单击&#x200B;**[!UICONTROL 费用类型]**。
1. 选择要修改的支出类型，然后单击&#x200B;**[!UICONTROL 编辑]**。

   出现&#x200B;**[!UICONTROL 编辑费用类型]**&#x200B;对话框。

1. 进行所需的更改，然后单击&#x200B;**[!UICONTROL 保存]**。

   费用类型现在可供用户将其与他们在项目和任务中的费用相关联。

有关如何使用费用以及它们如何影响项目成本的更多信息，请参阅文章[管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md)。
