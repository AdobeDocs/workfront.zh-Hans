---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 使用Adobe Workfront API添加高级验证选项
description: 使用Adobe Workfront API添加高级验证选项
author: Becky
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---


# 通过Adobe Workfront API创建验证时添加高级验证选项

在Workfront API中创建验证时，您可以添加高级验证选项。

使用以下工作流之一，通过API向验证添加验证选项：

* （推荐）使用Workfront API创建一个简单验证，然后使用ProofHQ API向验证添加高级验证选项

* 在Workfront API中使用JSON创建具有高级验证选项的验证

## 使用Workfront和ProofHQ API创建验证（推荐） {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

本节介绍如何使用Workfront和ProofHQ API的组合，通过Workfront API创建具有高级校对选项的校对。

ProofHQ API包含各种对Workfront API中的验证不可用的操作。 通过使用这些操作，您可以比Workfront API更准确地修改或配置验证。

有关ProofHQ API的概述，请参阅[PoofHQ概述](../../proofhq-api/general/overview.md)。 您还可以参阅[ProofHQ文档](https://api.proofhq.com/home.html)。

>[!NOTE]
>
>* Workfront API是一个REST-FUL API。 ProofHQ API是一个SOAP API。
>* 在ProofHQ API中创建的验证不会自动链接到Workfront。 因此，我们建议先在Workfront API中创建验证，然后再使用ProofHQ API更新它们。
>

### 使用高级校对选项创建校对

1. 使用Workfront API中的`Document createProof`操作创建验证。

   >[!NOTE]
   >
   >创建验证时，将`{}`设置为`advancedProofingOptions`参数的值。

1. 创建验证后，使用ProofHQ API添加任何高级选项。

### 示例

此部分显示您可以使用ProofHQ API进行的一些示例更新。

**示例：**

* [校对可以下载、有消息且已公开共享](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [更新阶段，使其不是私有的，不是强制的，并且只需要一次批准](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [将两个收件人添加到无主要决策者的验证](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**校对可以下载、有消息且已公开共享**

此端点的文档可在[ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html)页面上找到。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateProof>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{file_id}}</FileID>
            <OwnerID>0</OwnerID>
            <Name>{{proof_name}}}</Name>
            <Subject>Email subject here</Subject>
            <Message>Email message here</Message>
            <EnableDownload>true</EnableDownload>
            <EnableTeamURL>true</EnableTeamURL>
        </soap:updateProof>
    </soapenv:Body>
</soapenv:Envelope>
```

**更新阶段，使其不是私有的，不是强制的，并且只需要一次批准**

此端点的文档可在[ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html)页面上找到。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:updateWorkflowProofStage>
        <SessionID>{{session_id}}</SessionID>
        <FileID>{{proof_id}}</FileID>
        <Stage>
            <stage_id>{{stage_id}}</stage_id>
            <name>{{stage_name}}</name>
                <stage_one_decision_only>true</stage_one_decision_only>
                <stage_private>false</stage_private>
                <mandatory>false</mandatory>
            </Stage>
        </soap:updateWorkflowProofStage>
    </soapenv:Body>
</soapenv:Envelope>
```

**将两个收件人添加到无主要决策者的验证**

此端点的文档可在[ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html)页面上找到。

<!-- [Copy](javascript:void(0);) -->

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:soap="https://{{soap_host}}/">
    <soapenv:Header/>
    <soapenv:Body>
        <soap:addWorkflowProofReviewers>
            <SessionID>{{session_id}}</SessionID>
            <FileID>{{proof_id}}</FileID>
            <Recipients>
                <item>
                <email>{{recipient_email_1}}</email>
                <role>5</role>
                <name>{{recipient_name_1}}</name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
                <item>
                <email> {{recipient_email_2}} </email>
                <role>5</role>
                <name> {{recipient_name_2}} </name>
                <primary_decision_maker>false</primary_decision_maker>
                <stage_id>{{stage_id}}</stage_id>
                </item>
            </Recipients>
            <SuppressNewProofNotification></SuppressNewProofNotification>
        </soap:addWorkflowProofReviewers>
    </soapenv:Body>
</soapenv:Envelope>
```

## 在Workfront API中使用JSON创建验证

本节介绍如何在Workfront API中使用JSON作为参数值，通过Workfront API使用高级验证选项创建验证

### 使用高级校对选项创建校对

您可以使用`Document createProof`操作通过Workfront API创建验证。 此操作接受`advancedProofingOptions`参数，该参数的值类型为`string`。 要在您的`createProof`操作中包含高级校对选项，必须在`advancedProofingOptions`参数中以JSON格式输入选项。

>[!NOTE]
>
>可能很难预测要包含在advancedProofingOptions JSON中的字段。 在Workfront中使用高级校对时，您可能想要检查组织的网络数据，并将JSON基于组织常用的字段和值。
>
>由于这些字段可能难以预测，因此我们建议使用Workfront API创建验证，然后使用ProofHQ API更新它。 有关详细信息，请参阅本文中的[使用Workfront和ProofHQ API创建验证（推荐）](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended)

### 示例

此示例显示了在为`advancedProofingOptions`参数创建JSON时可以使用的字段和格式。 您的`advancedProofingOptions` JSON文件可以包含比此处显示更多或更少的字段。

**示例：**

<!-- [Copy](javascript:void(0);) -->

```
{
    "stages": [
        {
            "name": "stage1",
            "lockOn": 1,
            "position": 1,
            "isPrivate": false,
            "activateOn": 1,
            "recipients": [
                {
                    "name": "",
                    "role": 5,
                    "email": "user1_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": null
                },
                {
                    "name": "",
                    "role": 5,
                    "email": "user2_email@example.com",
                    "recipient_id": "",
                    "notifications": 0,
                    "isPrimaryDecisionMaker": false
                }
            ],
            "isMandatory": false,
            "deadlineDate": null,
            "deadlineTime": null,
            "isOneApproval": true,
            "activateOnDate": null,
            "parentPosition": null,
            "activateOnDecision": null,
            "deadlineCalculateOn": null,
            "deadlineBusinessDays": null
        }
    ],
    "message": "",
    "subject": "",
    "templates": [],
    "hasMessage": true,
    "canDownload": true,
    "customfields": [],
    "hasPublicSharing": true,
    "isAutomatedWorkflow": true,
    "stageBasedVisibility": 0
}
```
