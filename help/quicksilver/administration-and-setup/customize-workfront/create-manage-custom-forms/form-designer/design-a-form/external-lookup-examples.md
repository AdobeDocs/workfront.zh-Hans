---
title: 自定义表单中的外部查找字段示例
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 自定义表单中的外部查找字段调用外部API，并在下拉字段中作为选项返回值。 本文提供了使用外部查找字段调用Workfront或公共API的相同实例的示例。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 101a5a80d00a8113ce31222b92f77300a5b0ce8a
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# 自定义表单中的外部查找字段示例

自定义表单中的外部查找字段调用外部API，并在下拉字段中作为选项返回值。 使用自定义表单附加到的对象的用户可以从下拉菜单中选择一个或多个选项。

本文提供了使用外部查找字段调用Workfront或公共API的相同实例的示例。 您还可以使用外部查找与外部系统（如Jira、Salesforce或ServiceNow）通信。

外部查找字段仅在新的表单设计器中可用，在旧版表单生成器中不可用。 有关将外部查找字段添加到自定义表单以及外部查找组件的其他定义的更多信息，请参阅 [使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## 为同一Workfront实例设置外部查找字段

您可以使用外部查找将Workfront实例中的数据纳入自定义表单。

此示例说明如何调用Workfront API，并将现有“状态查询”字段中的数据引入外部查找字段。

1. 打开自定义表单。
1. 在屏幕左侧，查找 **外部查找** 然后将其拖动到画布上的某个部分。
1. 输入 **标签** 和 **名称** 用于字段。
1. 选择 **格式** 用于字段。
1. 在中输入API URL **基本API URL** 字段。

   * 您可以添加$$HOST以引用同一实例。
   * 可添加$$QUERY以根据查询其他字段来筛选结果。

   **示例**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. 查看 **依赖关系** 用于此查找字段在API中引用的字段。

   依赖项字段可以是对象详细信息页面中存在的任何自定义或本机字段。

   在此示例中， `{DE:StatusQuery}` 将被替换为StatusQuery自定义字段的值。

1. 选择 **HTTP方法**.

   这很有可能 **Get**.

1. 输入 **JSON路径** 以通过API调用获取结果。

   **示例**
   `$.data[*].name`

   >[!NOTE]
   >
   >**页眉** 调用同一Workfront实例不需要信息。

1. 单击 **应用**.

   ![以自定义表单设置对Workfront的API调用](assets/external-lookup-to-workfront.png)

   将自定义表单添加到Workfront对象（在本例中是项目）时，它类似于此。

   ![具有外部查找字段的自定义表单](assets/external-lookup-project-status-example1.png)

   ![基于状态的外部查找选项](assets/external-lookup-project-status-example2.png)

## 为公共API设置外部查找字段

您可以使用外部查找来调用外部公共API并检索数据。

此示例说明如何调用国家/地区的API(例如 <https://api.first.org/data/v1/countries>)以便您不必在下拉选项中硬编码所有国家/地区名称。

1. 打开自定义表单。
1. 在屏幕左侧，查找 **外部查找** 然后将其拖动到画布上的某个部分。
1. 输入 **标签** 和 **名称** 用于字段。
1. 选择 **格式** 用于字段。
1. 在中输入API URL **基本API URL** 字段。

   * 您可以添加$$QUERY来实施最终用户的查询筛选。

   **示例**
列出所有国家/地区： <https://api.first.org/data/v1/countries>

   允许用户在下拉字段中搜索任何国家/地区： <https://api.first.org/data/v1/countries?q=$$QUERY>

   允许用户搜索区域中的国家/地区： <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * 可用的区域在Workfront中的单独自定义字段中定义。
   * 当用户在表单上选择区域时，外部查找字段仅显示该区域中的国家（API中定义了该区域的国家/地区）。 用户还可以在所选区域中搜索国家/地区。

1. 查看 **依赖关系** 用于此查找字段在API中引用的字段。

   依赖项字段可以是对象详细信息页面中存在的任何自定义或本机字段。

   在此示例中， `{DE:Region}` 将被区域自定义字段的值替换。

1. 选择 **HTTP方法**.

   这很有可能 **Get**.

1. 输入 **JSON路径** 以通过API调用获取结果。

   此选项允许从API URL返回的JSON中提取数据。 它提供了一种方法，用于选择哪些值将从JSON内部显示在下拉选项中。

   **示例**
   `$.data[*].country`

1. （可选）单击 **添加标题**，然后键入或粘贴使用API进行身份验证所需的键值对。

   >[!NOTE]
   >
   >标头字段不是存储凭据的安全位置，您应该小心输入和保存的内容。

1. （可选）选择 **多选下拉列表** 以允许用户在下拉菜单中选择多个值。

1. 单击 **应用**.

   ![以自定义形式设置对公共API的API调用](assets/external-lookup-to-api-for-countries.png)

   将自定义表单添加到Workfront对象（在本例中是项目）时，它类似于此。

   ![具有外部查找字段的自定义表单](assets/external-lookup-countries-example1.png)

   ![基于区域的国家/地区的外部查找选项](assets/external-lookup-countries-example2.png)
