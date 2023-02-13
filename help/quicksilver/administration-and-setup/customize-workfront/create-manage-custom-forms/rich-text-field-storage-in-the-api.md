---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API中的富文本字段存储
description: 如果对象（如项目、问题或任务）包含富文本，则该对象将作为参数值通过Workfront API进行存储和访问。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# API中的富文本字段存储

如果对象（如项目、问题或任务）包含富文本，则该对象将作为参数值通过Workfront API进行存储和访问。

可以使用字段从包含富文本的项目对象请求文本信息 **parameterValues**.

例如，一个简单的HTTP请求可能如下所示：

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

如果此示例项目包含一个具有3个自定义字段的自定义表单：计算字段、段落文本和富1。 然后，上述请求将返回类似于以下内容的响应，其中字段“rich 1”是富文本参数字段，文本值为“**Hello** *世界！*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
				"blocks":[
				{
					"key":"7eibh",
					"text":"Hello Word!",
					"type":"unstyled",
					"depth":0,
					"inlineStyleRanges":[
					{
						"offset":0,
						"length":6,
						"style":"BOLD"
					},
					{
						"offset":6,
						"length":5,
						"style":"ITALIC"
					}
					],
					"entityRanges":[
					],
				"data":{
				}
				}
				],
			"entityMap":{
			}
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

有关如何存储富文本信息以及如何通过Adobe Workfront API进行检索的详细信息，请参阅 [Adobe Workfront API中的富文本字段](../../../wf-api/general/rich-text-field-api.md).
