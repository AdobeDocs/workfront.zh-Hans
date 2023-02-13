---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: 创建自定义费用类型
description: 作为 [!DNL Adobe Workfront] 管理员，您可以创建自定义费用类型，以定义和跟踪与任务和项目关联的费用。 费用是与任务或项目相关的非人工成本。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# 创建自定义费用类型

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

作为 [!DNL Adobe Workfront] 管理员，您可以创建自定义费用类型，以定义和跟踪与任务和项目关联的费用。 费用是与任务或项目相关的非人工成本。

您可以编辑或删除您创建的任何费用类型。 您无法删除或编辑内置 [!DNL Workfront] 费用类型。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 默认费用类型

位于 [!DNL Workfront] 默认情况下，无法删除或编辑包含以下内容：

* [!UICONTROL 广告]
* [!UICONTROL 咨询]
* [!UICONTROL 招待费]
* [!UICONTROL 常规]
* [!UICONTROL 材料]
* [!UICONTROL 差旅费]

## 创建自定义费用类型

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront].
1. 单击 **[!UICONTROL 费用类型]**.
1. 单击 **[!UICONTROL 新费用类型]**.
1. 在 **[!UICONTROL 新费用类型]** 框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL名称]</td> 
      <td>指定费用的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL描述]</td> 
      <td>指定费用的说明。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL计算单位]</td> 
      <td> <p>从下拉列表中选择费用类型的度量单位。</p> <p>可以使用以下测量单位：</p> 
       <ul> 
        <li>英里</li> 
        <li>千米</li> 
        <li>千克</li> 
        <li>美元</li> 
        <li>美元</li> 
        <li>天</li> 
        <li>其他 — 选择此选项将提示您命名测量单位，并将测量单位定义为组织所熟悉的内容。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">费率</td> 
      <td> <p>指定每件价格。 这是货币格式的字段，它表示在 <strong>[!UICONTROL计算单位]</strong> 字段。 </p> <p>该比率可包含一个在小数后最多包含4个数字的数值。 例如，1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 单击 **[!UICONTROL 创建费用类型]**.\
   费用类型现在可供用户将其与其项目和任务费用相关联。

## 修改自定义费用类型

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront].
1. 单击 **[!UICONTROL 费用类型]**.
1. 选择要修改的费用类型，然后单击 **[!UICONTROL 编辑]**.

   的 **[!UICONTROL 编辑费用类型]** 对话框。

1. 进行所需的更改，然后单击 **[!UICONTROL 保存更改]**.\
   费用类型现在可供用户将其与其项目和任务费用相关联。

有关如何使用费用以及费用如何影响项目成本的详细信息，请参阅文章 [管理项目费用](../../../manage-work/projects/project-finances/manage-project-expenses.md).
