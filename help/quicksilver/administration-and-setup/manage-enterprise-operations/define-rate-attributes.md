---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: 定义费率属性
description: 费率属性允许您在工作角色之外向费率添加其他维度，从而扩展Adobe Workfront的费率卡和费率功能。 然后，Workfront可以自动为分配选择正确的费率，确保财务准确性和项目间的一致性。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d570ef6a-935f-4dd0-9c54-a480163ec9d8
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 1%

---

# 定义费率属性

费率属性允许您在工作角色之外向费率添加其他维度，从而扩展Adobe Workfront的费率卡和费率功能。 这对于机构和企业而言至关重要，因为它们的费率不仅因工作角色而异，还因代理、地点、品牌、成本中心等因素而异。
通过组合这些属性，Workfront可以自动选择正确的分配率，确保财务准确性和项目间的一致性。

>[!IMPORTANT]
>
>费率属性是一次性基本设置。

一旦启用属性并将其应用于费率卡和费率，以后更改它们可能会危害整个财务设置中的数据完整性。

## 费率属性概览

费率属性被视为一次性设置，原因如下：

* 属性在启用后即成为财务数据模型的一部分。
* 费率、分配、计划值和实际值都取决于所选的属性值。
* 以后更改属性（重命名、删除或重新排序）可能会导致：

   * 费率与属性之间失去联系
   * 无效或“孤立”费率
   * 账单和报告不一致

出于这些原因，应在初始Workfront实施期间仔细设计属性，之后保持不变。

### 用作费率属性的对象

Workfront当前支持三个可用作费率属性的系统对象：

* **组**：通常重命名为&#x200B;_代理_&#x200B;或&#x200B;_业务部门_。
* **公司**：可以表示&#x200B;_品牌_、_客户端_&#x200B;或&#x200B;_客户_。
* **位置**：通常用作&#x200B;_市场_、_地区_&#x200B;或&#x200B;_办公室_。

  位置最多可分级定义3个级别。 （示例：如果您将“位置”定义为洛杉矶，则加利福尼亚和美国也将在费率匹配中使用。）

在设置属性时，可以重命名每个对象以匹配组织的术语。
例如：

* “代理”标签=组对象引用
* “成本中心”标签=子组对象引用
* “Location”标签=位置对象引用

这允许安装程序镜像您的业务结构，同时维护Workfront的数据模型完整性。

### 关于Workfront中费率属性的说明

* Workfront支持最多5个属性级别。 系统始终遵循属性层次结构，选择最具体的可用匹配。

   * 0 =通用基本费率
   * 1 - 5 =逐步提高具体比率

* 您可以重命名属性以反映您的业务（代理、品牌、市场、成本中心等）。
* 仅设置一次：以后更改属性可能会破坏财务数据的完整性。
* 可以安全地删除系统中任何位置未引用的属性。

  但是，如果属性已在使用中（在费率卡、用户配置文件、资源或分配中引用），将阻止删除以保护数据完整性。 在这些情况下，尝试删除属性（尤其是通过API调用）将导致错误。

* 上线前测试：创建试点费率卡并验证费率在分配中是否正确解析。
* 记录您的设置：与团队共享您的费率属性设置，以便他们了解费率的工作方式。

### 可在何处应用费率属性

在Workfront中存在费率的所有区域均支持费率属性：

* 费率卡：按工作角色和属性定义费率。
* 项目层覆盖：在项目层覆盖费率时应用属性。
* 工作角色（在设置中）：使用属性设置默认工作角色费率。
* 用户（用户配置文件）：将本地属性分配给个别用户，以便这些用户的分配自动解析为正确的费率。

<!--
BULLET POINT Staffing plan resources
BULLET POINT Non-labor resources: Attributes can also be defined on resources such as equipment or services.-->

<!--Non-labor resource categories and -->工作角色不支持直接在对象级别使用费率属性。 它们通过在其上定义的费率与费率属性相连。

如果您可以创建与正确属性值关联的占位符分配，则会相应地填充费率。

* 对于工作角色，当您以后使用实际用户替换占位符时，系统会自动将分配的属性重置为该用户配置文件上定义的属性。 此时，不能再在分配层编辑属性。 它们从用户继承而来，用于保持一致性并防止用户属性与应用率之间出现不一致的现象。

<!-- BULLET POINT For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

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
   <td><p>[！UICONTROL标准版]</p></td>
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>[！UICONTROL系统管理员]</td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 配置费率属性

每个属性都有一组可配置的选项，包括常规属性和过滤器。
过滤器控制如何在定义费率时建议和验证属性值。 它们对于保持属性选择一致、指导用户使用有效选项以及防止无效组合至关重要。

{{step-1-to-setup}}

1. 在左侧面板中，单击&#x200B;**费率属性**。
1. 单击图表中的加号图标可添加属性。

   >[!NOTE]
   >
   >图中最多可以有5个属性。 从上到下的顺序定义了属性应用方式的层次结构。 单击&#x200B;**旋转**&#x200B;图标![旋转图标](assets/rotate-attribute-view-icon.png)可按从左到右的方向显示图表。 您还可以放大或缩小，并使图表适合屏幕。

1. 选择属性以打开屏幕右侧的配置面板。

   ![配置费率属性](assets/configure-rate-attributes.png)

1. 将对象（“组”、“公司”、“位置”）重命名为您的业务所需的术语（如“代理”、“位置”、“成本中心”）。
1. 单击每个属性上的&#x200B;**保存**&#x200B;以保存您的命名约定。

   这些属性的名称将显示在系统中所有费率卡和费率上。

1. 在配置面板中设置每个属性的属性：

   * **必填**：选择属性是否为费率上的必填字段。
   * **用于收入计算**：在记帐费率计算中包括此属性。
   * **用于成本计算**：在成本费率计算中包括此属性。

     >[!NOTE]
     >
     >要使属性在财务计算中起作用，必须至少选择一个计算选项。

   * （可选） **层级**：允许属性遵循父子关系，如“城市”>“州/省”>“国家/地区”。

     此属性仅适用于Location对象。

### 定义属性的过滤器

属性可使用两种类型的过滤器：

* 建议过滤器根据系统逻辑或先前的属性选择缩小可用选项列表。 它们使下拉列表具有上下文感知并且易于使用。

  实例：机构>地点>成本中心

  在此设置中，“成本中心”属性应具有同时引用代理和地点的建议过滤器。

  添加费率时，如果您首先选择Agency = &quot;Star&quot; ，则“位置”下拉菜单将仅建议属于&quot;Star&quot;的位置。

  如果您随后在费率上选择“位置=芝加哥”，则“成本中心”下拉菜单将仅建议与“星级”和芝加哥关联的“成本中心”。

* 关系筛选器建立属性之间的依赖关系链。 它们可确保系统了解属性如何相互关联并强制执行有效的依赖关系。

  实例：机构>地点>成本中心

  在此设置中，“机构”属性应具有一个关系筛选器，以将其与有效地点和成本中心绑定。

必须始终双向配置过滤器。 如果属性A具有属性B的关系过滤器，则属性B应具有重新添加到属性A的建议过滤器。这可以确保数据完整性和干净的用户体验。

1. 在配置面板中选择用于定义属性的建议筛选器和关系筛选器的选项：

   * **筛选器类型**：

      * **标准**&#x200B;筛选器将通用条件应用于属性对象。 例如，Location > Is Active = True （只显示活动位置）。

        无论是否选择其他属性，始终应用“标准”筛选器。

      * **Attribute**&#x200B;筛选器将一个属性链接到链中的另一个属性。 例如，地点>参考=机构（只显示与选定机构关联的地点）。

        仅当引用的属性具有值时，才应用属性过滤器。 例如，如果选择“代理”，则仅建议有效的位置。 如果“代理”为空，则会显示所有位置（但仍会受到应用于该位置的标准过滤器的限制）。

   * **字段**：属性对象的直接字段，如位置ID或活动标志。
   * **运算符**：这些选项取决于所选的字段类型。 示例包括Equals、Not Equals、Is Blank、True/False。
   * （仅限标准筛选器类型）**值**：例如，Is Active = True。
   * （仅限属性筛选器类型） **引用**：此筛选器所依赖的属性，如Agency。
   * （仅限属性筛选器类型） **引用字段**：引用的属性上必须匹配的字段，如机构ID。

1. 单击每个属性上的&#x200B;**保存**&#x200B;以保存属性和筛选器。
