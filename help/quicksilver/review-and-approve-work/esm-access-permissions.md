---
product-area: documents
navigation-topic: approvals
title: Adobe企业存储模型的对象权限和访问级别概述
description: Adobe企业存储权限和访问概述
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
source-git-commit: 89dcc972e2e29890763dba6b5f7a44489a2eee5a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---


# Adobe企业存储模型的对象权限和访问级别概述

<!--linked in UI -->

Adobe企业存储是一种基于云的存储解决方案，它用作Adobe企业产品中资产的中央存储存储库。 使用Adobe企业存储的Workfront环境的对象权限和访问级别行为与使用旧版Workfront文档存储的环境略有不同。

## 访问级别

Workfront访问级别仅适用于Workfront。 Workfront中的项目和文档限制并不总是适用于其他Adobe应用程序。

### 同时使用Adobe企业级存储和旧版Workfront存储的环境

根据项目是在Adobe企业存储上还是在旧版Workfront存储上，文档访问的行为有所不同：

* **旧版Workfront存储**：使用旧版Workfront存储的项目、程序、项目组合和模板遵循标准Workfront访问级别逻辑进行文档访问。 当访问级别为文档选择了&#x200B;**无访问权限**&#x200B;时，他们将无法在Workfront或其他Adobe产品(如Frame.io或Creative Cloud)中查看文档。
* **Adobe企业存储**：使用Adobe企业存储的项目、程序、项目组合和模板遵循Adobe其他产品的Adobe企业存储访问级别逻辑。


   * **项目、程序、项目组合和模板对象权限**：当访问级别对项目、程序、项目组合和模板选择&#x200B;**无访问权限**，但该对象与他们共享时，用户无法在Workfront中查看该对象，但在其他Adobe工具(如Frame.io和Adobe Creative Cloud)中仍可以查看对象名称和任何关联文档。
   * **文档权限**：当访问级别对文档选择&#x200B;**无访问权限**&#x200B;时，用户无法查看Workfront中项目的文档，但仍可以查看和管理在其他Adobe工具(如Frame.io和Adobe Creative Cloud)中与用户共享的项目文档。 这是因为文档访问由Adobe企业存储中的项目级权限决定，而不是仅由Workfront访问级别决定。

如果您在Workfront环境中启用了Adobe企业级存储，则可以创建Adobe企业级存储项目和旧版Workfront存储项目。 旧版Workfront存储项目在Workfront中项目名称旁边会显示一个图标。 Adobe企业存储项目不显示图标。

项目名称旁边的![旧版workfront存储图标](assets/legacy-project-icon.png)


### 仅使用Adobe企业存储的环境

您无法修改使用Adobe企业存储的项目、项目和项目组合的访问级别文档权限。

所有访问级别都具有文档的编辑权限。 项目级别的权限可决定其他Adobe工具中的文档访问权限。

您无法限制文档继承访问权限。


### 仅使用旧版Workfront存储的环境

不更改文档访问级别或行为。


## 项目

具有项目级别权限的用户可以查看和管理其他Adobe产品(如Frame.io和Adobe Creative Cloud)中的项目文档。

对于ESM项目，项目名称在Workfront外部也可见。

对于ESM项目，财务数据在Workfront外部不可见。

## 任务和问题

文档存储在项目级别，但可以根据需要共享给各个任务和问题。 具有任务和问题访问权限的用户自动从项目继承文档访问权限。 您无法修改其访问级别。 他们具有管理访问权限或无权访问。