---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: 将旧版对象转换为Adobe云存储
description: 了解可将旧版Workfront存储对象转换为Adobe云存储的三种情况，并了解在每次转换期间哪些内容会移动以及会保留哪些内容。
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---
# 将旧版对象转换为Adobe云存储

在大多数情况下，您只能在类似存储模型之间移动、复制和转换Workfront对象。 例如，您可以将任务从一个Adobe云存储项目移动到另一个Adobe云存储项目。 在以下三个特定用例中，您可以将旧版Workfront存储对象转换为Adobe云存储：

* 将旧版Workfront存储任务转换为Adobe云存储项目
* 将旧版Workfront存储产品组合转换为Adobe云存储产品组合
* 从旧版Adobe存储模板创建一个Workfront云存储项目

有关移动方向以及Adobe云存储的不同之处，请参阅[在Adobe云存储上移动到Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## 将旧版任务转换为Adobe云存储项目

要将旧版Workfront存储任务转换为Adobe云存储项目，请在该任务上使用现有的项目转换流程。 转换期间：

* 子任务和问题移至新项目。
* 附加到任务的文档及其审批工作流仍保留在原始项目中。
* 已删除工作审批和解析对象链接。
* 已删除原始任务。

## 将旧版产品组合转换为Adobe云存储产品组合

Workfront管理员可以从设置区域将旧版Workfront存储产品组合转换为Adobe云存储产品组合。 转换后：

* 不能再将旧版Workfront存储项目移入项目组合。
* 在项目组合中创建的所有新项目都使用Adobe云存储。
* Frame.io是项目组合的Adobe云存储项目中文档的查看器。
* 使用旧版Workfront存储的子项目将保留在旧版存储中。
* 子程序将保留在旧版存储中。

>[!NOTE]
>
>仅当有人手动将Adobe云存储项目添加到子旧程序时，它才会自动转换为Adobe云存储。

有关详细信息，请参阅[将旧项目组合转换为Adobe云存储](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md)。

## 从旧模板创建Adobe云存储项目

从旧版Workfront存储模板创建项目时，“项目创建”对话框中的&#x200B;**在Adobe云存储上创建此项目**&#x200B;复选框决定了新项目的存储类型。 复选框行为取决于您创建项目的位置：

* **在项目组合外**：该复选框默认可用并清除。 选择它可在Adobe云存储上创建新项目。
* **在Adobe云存储产品组合中**：复选框已选中并已锁定。 新项目必须与产品组合的存储类型匹配。
* **在旧版Workfront存储产品组合中**：该复选框不可用。 新项目使用旧版Workfront存储。

有关详细信息，请参阅[创建项目](/help/quicksilver/manage-work/projects/create-projects/create-project.md)。
