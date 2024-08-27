---
title: Adobe Workfront规划API基础知识
description: Adobe Workfront Planning API的目标是通过引入通过HTTP运行的REST-ful架构来简化与Planning的构建集成。 本文档假定您熟悉REST和JSON响应，并介绍了Planning API采用的方法。
author: Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: afb58d04-fa75-4eb7-9c19-2a8c1748fbc2
source-git-commit: 20e8d45264f9441d9576c7d4d5521e4f6053a7f3
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 1%

---


# Adobe Workfront规划API基础知识

{{planning-important-intro}}

Adobe Workfront Planning API的目标是通过引入通过HTTP运行的REST-ful架构来简化与Planning的构建集成。 本文档假定您熟悉REST和JSON响应，并介绍了Planning API采用的方法。

熟悉Workfront Planning架构将有助于了解可用于从Workfront Planning中提取数据以进行集成的数据库关系。

您可以从Workfront自定义表单中的外部查找字段调用Planning API。

有关外部查找字段的详细信息，请参阅自定义表单中外部查找字段的[示例](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/external-lookup-examples.md)。

## Workfront规划API URL

<!--For more details and examples of each operation, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

### 运营

通过将HTTP请求发送到对象的唯一URI来控制对象。 要执行的操作由HTTP方法指定。

标准HTTP方法对应于以下操作：

* **GET** — 按ID检索对象，按查询搜索所有对象
* **POST** — 插入新对象
* **PUT** — 编辑现有对象
* **DELETE** — 删除对象

有关每个操作的更多详细信息和示例，请参阅[Workfront Planning API开发人员文档](https://developer.adobe.com/wf-planning/)。

### 字段类型和与其一起使用的搜索修饰符

您可以使用带有字段的修饰符和过滤器来控制在结果中返回哪些数据。

<!--For examples, see the [Workfront Planning API developer documentation](https://developer.adobe.com/wf-planning/).-->

#### 使用搜索修饰符

Workfront Planning支持以下搜索修饰符：

<table>
    <tr>
        <td><b>修改者</b></td>
        <td><b>示例</b></td>
        <td><b>描述</b></td>
        <td><b>可能值</b></td>
    </tr>
    <tr>
        <td>$contain </td>
        <td><code>"fieldId": { "$contains": "product" } </code> </td>
        <td>返回其字段值包含过滤器的记录  </td>
        <td>"新产品发布"  </td>
    </tr>
    <tr>
        <td>$doesNotContain</td>
        <td><code>"fieldId": { "$doesNotContain": "product" } </code> </td>
        <td>返回字段值不包含过滤器的记录  </td>
        <td>"新启动项"  </td>
    </tr>
    <tr>
        <td>$is </td>
        <td><ul><li><code>"fieldId" : { "$is": "new product launch" } </code></li><li><code>"fieldId" : { "new product launch" } </code></li><ul> </td>
        <td>返回字段值与过滤器完全匹配的记录  </td>
        <td>"新产品发布"  </td>
    </tr>
    <tr>
        <td>$isNot </td>
        <td><code>"fieldId": { "$isNot": "product" } </code> </td>
        <td>返回字段值完全不匹配过滤器的记录  </td>
        <td>"新产品发布"  </td>
    </tr>
    <tr>
        <td>$isEmpty </td>
        <td><ul><li><code>"fieldId": "$isEmpty" </code></li><li><code>"fieldId": { "$isEmpty": null } </code></li><ul> </td>
        <td>返回字段值不为空的记录  </td>
        <td><ul><li>"" </li><li>null </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotEmpty </td>
        <td><ul><li><code>"fieldId": "$isNotEmpty"  </code></li><li><code>"fieldId": { "$isNotEmpty": null } </code></li><ul> </td>
        <td>返回字段值不为空的记录  </td>
        <td>"新产品发布"  </td>
    </tr>
    <tr>
        <td>$greaterThan </td>
        <td><code>"fieldId": { "$greaterThan": 10 } </code> </td>
        <td>返回字段值大于筛选器的记录  </td>
        <td><ul><li>20</li><li>25</li><ul> </td>
    </tr>
    <tr>
        <td>$greaterThanOrEqual </td>
        <td><code>"fieldId": { "$greaterThanOrEqual": 10 } </code> </td>
        <td>返回字段值大于或等于过滤器的记录  </td>
        <td><ul><li>10</li><li>20</li><li>25</li> </ul></td>
    </tr>
    <tr>
        <td>美元小于 </td>
        <td><code>"fieldId": { "$lessThan": 10 } </code> </td>
        <td>返回字段值小于筛选器的记录  </td>
        <td><ul><li>5</li><li>9</li></td></ul> 
    </tr>
    <tr>
        <td>$lessThanOrEqual </td>
        <td><code>"fieldId": { "$lessThanOrEqual": 10 } </code> </td>
        <td>返回字段值小于或等于过滤器的记录 </td>
        <td><ul><li>5</li><li>9</li><ul><li>10</li> </td>
    </tr>
    <tr>
        <td>$isAfter </td>
        <td><code>"fieldId": { "$isAfter": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>返回字段值在筛选器之后的记录  </td>
        <td>“2024-05-15T20:00:00.000Z”  </td>
    </tr>
    <tr>
        <td>$isBefore </td>
        <td><code>"fieldId": { "$isBefore": "2024-05-14T20:00:00.000Z" } </code> </td>
        <td>返回字段值在筛选器之前的记录 </td>
        <td>“2024-05-12T20:00:00.000Z” </td>
    </tr>
    <tr>
        <td>$isBetween </td>
        <td><code>"fieldId": { "$isBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>返回字段值介于过滤器之间的记录  </td>
        <td><ul><li>“2024-05-12T20:00:00.000Z” </li><li>“2024-05-14T20:00:00.000Z” </li><ul>  </td>
    </tr>
    <tr>
        <td>$isNotBetween </td>
        <td><code>"fieldId": { "$isNotBetween": ["2024-05-10T20:00:00.000Z", "2024-05-15T20:00:00.000Z"] } </code> </td>
        <td>返回字段值不在过滤器之间的记录  </td>
        <td><ul><li>“2024-05-09T20:00:00.000Z”  </li><li>“2024-05-17T20:00:00.000Z”  </li><ul>  </td>
    </tr>
    <tr>
        <td>$isAnyOf </td>
        <td><code>"fieldId": { "$isAnyOf": ["active", "completed"] } </code> </td>
        <td>返回字段值为任意过滤器的记录  </td>
        <td><ul><li>"active" </li><li>"completed" </li><ul> </td>
    </tr>
    <tr>
        <td>$isNoneOf </td>
        <td><code>"fieldId": { "$isNoneOf": ["active", "completed"] } </code> </td>
        <td>返回字段值不为任何过滤器的记录 </td>
        <td><ul><li>“已完成”  </li><li>"fixed"  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAnyOf </td>
        <td><code>"fieldId": { "$hasAnyOf": ["active", "completed"] } </code> </td>
        <td>返回字段值具有任何过滤器的记录  </td>
        <td><ul><li>["active"， "fixed"]  </li><li>[“已修复”、“已完成”、“已完成”]  </li><ul> </td>
    </tr>
    <tr>
        <td>$hasAllOf </td>
        <td><code>"fieldId": { "$hasAllOf": ["active", "completed"] } </code> </td>
        <td>返回其字段值具有所有过滤器的记录  </td>
        <td><ul><li>[“活动”，“已完成”]   </li><li>[“活动”、“已完成”、“已完成”]   </li><ul> </td>
    </tr>
    <tr>
        <td>$hasNoneOf </td>
        <td><code>"fieldId": { "$hasNoneOf": ["active", "completed"] } </code> </td>
        <td>返回字段值不含任何过滤器的记录 </td>
        <td>[“已修复”，“已完成”]  </td>
    </tr>
    <tr>
        <td>$isExactly </td>
        <td><code>"fieldId": { "$isExactly": ["active", "completed"] } </code> </td>
        <td>返回字段值完全为过滤器的记录  </td>
        <td>[“活动”，“已完成”]  </td>
    </tr>
</table>

#### 字段类型

以下是受支持的字段类型的列表，以及对于这些字段类型可以使用的搜索修饰符

| 字段类型 | 支持的搜索修饰符 |
|---|---|
| 文本 | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| 长文本 | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| 数字 | $is， $isNot， $greaterThan， $greaterThanOrEqual， $lessThan， $lessThanOrEqual， $isEmpty， $isNotEmpty |
| 百分比 | $is， $isNot， $greaterThan， $greaterThanOrEqual， $lessThan， $lessThanOrEqual， $isEmpty， $isNotEmpty |
| 货币 | $is， $isNot， $greaterThan， $greaterThanOrEqual， $lessThan， $lessThanOrEqual， $isEmpty， $isNotEmpty |
| 日期 | $is， $isNot， $isAfter， $isBefore， $isBetween， $isNotBetween， $isEmpty， $isNotEmpty |
| 单选 | $is， $isNot， $isAnyOf， $isNoneOf， $isEmpty， $isNotEmpty |
| 多选 | $hasAnyOf， $hasAllOf， $isExactly， $hasNoneOf， $isEmpty， $isNotEmpty |
| 布尔值 | $is |
| 用户 | $hasAnyOf， $hasAllOf， $isExactly， $hasNoneOf， $isEmpty， $isNotEmpty |
| 公式 | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| url | $contains， $doesNotContain， $is， $isNot， $isEmpty， $isNotEmpty |
| 创建者 | $is， $isNot， $isAnyOf， $isNoneOf |
| created-at | $is， $isNot， $isAfter， $isBefore， $isBetween， $isNotBetween |
| 更新者 | $is， $isNot， $isAnyOf， $isNoneOf， $isEmpty， $isNotEmpty |
| 更新时间 | $is， $isNot， $isAfter， $isBefore， $isBetween， $isNotBetween， $isEmpty， $isNotEmpty |
| 引用 | $hasAnyOf， $hasAllOf， $isExactly， $hasNoneOf， $isEmpty， $isNotEmpty |
| 查找 | 取决于链接的字段 |

### 使用“And”和“Or”语句

在API调用中，您可以具有基于由$and和“$or”语句组合而成的多个条件的过滤器

```
{
  "recordTypeId": "recordTypeId",
  "offset": "integer",
  "limit": "integer",
  "filters": [
    {
      "$or": [
        {
          "launch_date": {
            "$isBetween": [
              "2024-03-31T20:00:00.000Z",
              "2024-04-01T20:00:00.000Z"
            ]
          }
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-03-31T20:00:00.000Z",
                  "2024-04-01T20:00:00.000Z"
                ]
              }
            },
            {
              "status": "active"
            }
          ]
        },
        {
          "$and": [
            {
              "launch_date": {
                "$isBetween": [
                  "2024-04-15T00:00:00.000Z",
                  "2024-04-16T00:00:00.000Z"
                ]
              }
            },
            {
              "status": "planned"
            }
          ]
        }
      ]
    }
  ]
}
```

### 使用字段请求参数

您可以使用字段请求参数指定应返回的特定字段的逗号分隔列表。 这些字段名称区分大小写。

例如，请求

`/v1/records/search?attributes=data,createdBy`

```
{
    "records": [
        {
            "id": "Rc6527ecb35df57c441d92ba00",
            "createdBy": "61a9cc0500002f9fdaa7a6f824f557e1",
            "createdAt": null,
            "updatedBy": null,
            "updatedAt": null,
            "customerId": null,
            "imsOrgId": null,
            "recordTypeId": null,
            "data": {
                "F666c0b58b6fee61a2ea6ea81": [
                    {
                        "externalId": null,
                        "id": "Rc665728ff95730b58bc757b13",
                        "value": null
                    },
....
```

返回类似于以下内容的响应：


```
{ 
    "priority": 2, 
    "name": "first task", 
    "ID": "4c7c08fa0000002ff924e298ee148df4", 
    "plannedStartDate": "2010-08-30T09:00:00:000-0600" 
} 
```

### 在API中对查询结果进行排序

如果将以下内容附加到API调用，则可以按任何字段对结果进行排序：


`/v1/records/search`

请求正文：

```
{
    "recordTypeId": "Rt6527ecb25df57c441d92b9fa",
    "filters": [],
    "sorting": [
        {
            "fieldId": "F6527ecb25df57c441d92b9fc",
            "direction": "asc"
        },
        {
            "fieldId": "F658afcbd4a0273c67c346fd5",
            "direction": "desc"
        }
    ],
    "limit": 500,
    "offset": 0,
    "rowOrderViewId": "V6527ecb75df57c441d92ba03",
    "groupingFieldIds": []
}
```

### 查询限制和分页响应

默认情况下，Planning API请求从列表开头返回500个结果。 要覆盖结果数的默认限制，您可以在请求中使用`limit`参数，并将其设置为其他数字，最多2000个结果。

我们建议您考虑将`offset`参数添加到请求，以对大型数据集使用分页响应。 分页响应允许您指定应返回的第一个结果的位置。

例如，如果要返回结果2001-4000，可以使用以下请求。 此示例返回2000条处于活动状态的记录，从2001年的结果开始：

`POST /v1/records/search `



请求正文：

```
{ 
    "recordTypeId": "recordTypeId", 
    "offset": "2001", 
    "limit": "2000", 
    "filters": [ 
        { "status": "active" } 
    ] 
} 
```

要确保结果正确分页，请使用排序参数。 这样可按相同顺序返回结果，以便分页不会重复或跳过结果。

有关排序的详细信息，请参阅本文中的[在API中对查询结果进行排序](#sorting-query-results-in-the-api)。
