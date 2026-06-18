---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 将旧版项目组合转换为Adobe云存储
description: 将现有的旧版Workfront存储产品组合从“系统首选项”的“存储首选项”区域转换为Adobe云存储。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 1e6380b0422efdd98449ab1e74cadb4f330917f1
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 5%

---

# 将旧版项目组合转换为Adobe云存储

作为Workfront管理员，您可以从“系统首选项”的“存储首选项”区域，将现有的旧版Workfront存储产品组合转换为Adobe云存储。 在转换项目组合后，其行为与任何其他Adobe云存储项目组合类似。

有关已转换项目组合的行为方式及其子对象受到的影响的详细信息，请参阅[在Adobe云存储上移动到Workfront &#x200B;](/help/quicksilver/review-and-approve-work/workfront-storage.md)中的[对象可移植性](/help/quicksilver/review-and-approve-work/workfront-storage.md#object-portability)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>任何工作流包</p></td> 
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

## 转换项目组合之前

在转换旧版Workfront存储产品组合之前，请考虑以下事项：

* 转换仅影响投资组合本身。 使用旧版Workfront存储的子项目和程序将保留在旧版存储中。

  >[!NOTE]
  >
  >仅当有人手动将Adobe云存储项目添加到子旧程序时，它才会自动转换为Adobe云存储。
* 产品组合中的文档和文档文件夹在转换后仍保留在旧版Workfront存储中。
* 转换后，您无法将旧版Workfront存储项目添加到项目组合。

## 将旧版项目组合转换为Adobe云存储

要将一个或多个旧版Workfront存储产品组合转换为Adobe云存储，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**首选项**。

1. 向下滚动到&#x200B;**存储首选项**&#x200B;部分。

1. 在&#x200B;**选择要转换为Adobe云存储的项目组合**&#x200B;字段中，选择一个或多个旧版Workfront存储项目组合。

1. 单击&#x200B;**保存**。

   此时会显示一条确认消息，描述项目组合转换时发生的情况：

   * 不能再将旧版Workfront存储项目移入项目组合。
   * 在项目组合中创建的所有新项目都使用Adobe云存储。
   * Frame.io是项目组合的Adobe云存储项目中文档的查看器。
   * 使用旧版Workfront存储的子项目将保留在旧版存储中。
   * 子程序将保留在旧版存储中。

1. 单击&#x200B;**转换**&#x200B;以确认。

   所选项目组合将转换为Adobe云存储。
