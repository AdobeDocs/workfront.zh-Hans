---
title: 2026年第四季度财务管理增强功能
description: 2026年第四季度财务管理增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 2026年第四季度财务管理增强功能

本页介绍了在2026年第四季度发行的“预览”环境中执行的Financial Management增强功能。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第四季度发布周期中此时可用的所有更改列表，请参阅[2026年第四季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md)。

## 公司记帐费率的增强功能

>[!NOTE]
>
>预览： 2026年9月3日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日

已对公司记帐费率功能进行了多项更新。

### 适用于所有Workfront和工作流程包上的客户

* 我们更新了用于添加和编辑公司记帐费率的对话框，使其设计更加现代化，与Workfront的其他区域保持一致。
* “允许公司级别的记帐费率覆盖项目级别的记帐费率”设置可在将公司添加到项目时，正确添加费率覆盖，并且计划的收入计算使用公司级别的记帐费率。
* 无权在项目级别编辑常规财务和编辑记帐费率的用户无法再将公司添加到该项目。

### 仅适用于工作流Ultimate包中的客户

费率属性现在适用于公司级别的记帐费率。 有效日期也可应用于公司费率。

注：公司层费率尚未添加到费率层次结构。

有关详细信息，请参阅[覆盖公司级别的工作角色记帐费率](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)和[使用公司级别记帐费率覆盖项目级别记帐费率](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md)。

## 属性层次结构现在会自动保持连接

>[!NOTE]
>
>预览： 2026年9月3日
>生产快速发布： 2026年9月17日
>适用于所有人的生产： 2026年10月15日
>此功能仅适用于Workflow Ultimate包中的组织。

现在，在Workfront的各个区域（例如高级工作）中将费率属性用作过滤器时，会对父子过滤应用附加验证。

以前，如果您将一个属性链接到父级，而将该父级链接到祖级父级，则系统不会自动将原始属性识别为也属于该祖级父级。 现在，当您选择最低级别属性时，将自动分配该属性以上的每个级别。

有关属性的信息，请参阅[定义费率属性](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)。
