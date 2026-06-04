---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API中的富文本字段存储
description: 如果项目、问题或任务等对象包含富文本，则会通过Workfront API将该对象作为参数值存储和访问。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
TQID: https://experienceleague.adobe.com/lLZZugNI5odziqyz7uBMnkiVoOdGcT-jKb90j9TUG1Q
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 174
ht-degree: 0%

---

# API中的富文本字段存储

如果项目、问题或任务等对象包含富文本，则会通过Workfront API将该对象作为参数值存储和访问。

可以使用字段&#x200B;**parameterValues**&#x200B;从包含富文本的项目对象请求文本信息。

例如，一个简单的HTTP请求可能类似于以下内容：

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

如果此示例项目包含具有3个自定义字段的自定义表单：计算字段、段落文本和富文本1。 然后，上述请求将返回类似于以下内容的响应，其中字段“rich 1”是富文本参数字段，文本值为“**Hello** *World！*”：

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
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
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

要更深入地了解如何通过Adobe Workfront API存储和检索富文本信息，请参阅Adobe Workfront API中的[富文本字段](../../../wf-api/general/rich-text-field-api.md)。
