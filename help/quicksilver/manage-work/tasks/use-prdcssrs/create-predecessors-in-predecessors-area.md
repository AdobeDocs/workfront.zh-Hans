---
product-area: projects
navigation-topic: use-predecessors
title: 使用前置任务区域创建前置任务关系
description: 您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。
author: Alina
feature: Work Management
exl-id: 68774286-da24-409a-bbd8-eb18dfe75063
TQID: https://experienceleague.adobe.com/BOZkyUl3TKCzpbjbLnUcMQZjM-1laW-TSsVptvBP-0U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 422
ht-degree: 4%

---

# 使用前置任务区域创建前置任务关系

<!-- Audited: 5/2025 -->

您可以使用前置任务（或只是前置任务）来链接依赖其他任务启动或完成的任务。 例如，在发送邀请（前置任务）之前，您不希望主持某方（依赖任务）。

本文介绍如何使用任务中的“前置任务”选项卡设置前置任务。

有关在任务列表中设置前置任务的信息，请参阅[在任务列表中创建前置任务关系](../../../manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md)。

您可以在Adobe Workfront的以下区域中查看任务的前置任务：

* 在相关任务的“前置任务”部分
* 在甘特图中
* 在“前置任务”列的任务列表中

有关前置任务的信息，请参阅[前置任务概述](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> 
   <p>规划</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对任务和项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务和项目的权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为任务创建前置任务

使用“前置任务”区域为项目任务创建前置任务与为模板上的模板任务创建前置任务类似。

要为项目任务创建前置任务，请执行以下操作：

1. 导航到要指定为从属任务的任务。

1. 在左侧面板中，单击&#x200B;**前置任务**。

1. 在&#x200B;**前置任务**&#x200B;部分中，单击&#x200B;**添加前置任务**。 将打开&#x200B;**添加前置任务**&#x200B;对话框。

1. （可选）要添加跨项目前置任务，请将&#x200B;**父项目**&#x200B;字段中的项目名称替换为其他项目。

   有关信息，请参阅[创建跨项目前置任务](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md)。

   >[!TIP]
   >
   >无法为模板任务创建跨模板前置任务。


1. 在&#x200B;**任务**&#x200B;字段中，键入要指定为前置任务的一个或多个任务的名称，然后在它们出现在下拉列表时将其选定。

1. 选择&#x200B;**依赖关系类型**。

   有关信息，请参阅[任务依赖关系类型概述](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)。

1. 输入&#x200B;**延迟**&#x200B;金额。

   有关信息，请参阅{&#x200B;0}滞后类型概述](../../../manage-work/tasks/use-prdcssrs/lag-types.md)。[

   ![添加前置任务对话框](assets/add-predecessor-dialog-box.png)

1. 如果要强制两个任务之间的前置任务关系，请选中&#x200B;**强制**&#x200B;复选框。

   有关信息，请参阅[强制执行前置任务](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md)。

1. 单击&#x200B;**保存**。

1. （可选）要删除前置任务，请从前置任务列表中将其选中，然后单击&#x200B;**删除**&#x200B;图标![删除图标](assets/remove-or-delete-icon.png)。

   前置任务将从列表中删除。 前置任务未从其项目中删除。
