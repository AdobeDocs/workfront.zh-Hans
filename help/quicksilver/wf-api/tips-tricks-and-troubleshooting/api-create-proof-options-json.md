---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: 通过Adobe Workfront API添加高级校对选项
description: 通过Adobe Workfront API添加高级校对选项
author: Becky
feature: Workfront API, Workfront Proof
exl-id: 5fcdf07e-d077-4d6a-bc3f-973983877c7c
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# 通过Adobe Workfront API创建校样时，添加高级校样选项

在Workfront API中创建校样时，您可以添加高级校样选项。

使用以下工作流之一，使用API向校样添加校样选项：

* （推荐）使用Workfront API创建简单校样，然后使用ProofHQ API向校样添加高级校样选项

* 在Workfront API中使用JSON通过高级校对选项创建校样

## 使用Workfront和ProofHQ API创建校样（推荐） {#create-a-proof-using-the-workfront-and-proofhq-apis-recommended}

本节介绍如何使用Workfront API和Workfront API的组合，通过高级校样选项创建校样。

ProofHQ API包含许多无法在Workfront API中进行校样的操作。 通过使用这些操作，您可以修改或配置校样的精度比Workfront API中提供的更高。

有关ProofHQ API的概述，请参阅 [PoofHQ概述](../../proofhq-api/general/overview.md). 您还可以将 [ProofHQ文档](https://api.proofhq.com/home.html).

>[!NOTE]
>
>* Workfront API是一个RESTful API。 ProofHQ API是一个SOAP API。
>* 在ProofHQ API中创建的校样不会自动链接到Workfront。 因此，我们建议先在Workfront API中创建校样，然后再使用ProofHQ API更新校样。
>


### 使用高级校对选项创建校样

1. 使用创建校样 `Document createProof` 操作。Workfront API中的。

   >[!NOTE]
   创建校样时，请勿包含advancedPoofingOptions参数的值。

1. 创建校样后，使用ProofHQ API添加任何高级选项。

### 示例

此部分显示您可以使用校样HQ API进行的一些示例更新。

**示例:**

* [校样可以下载、包含消息并公开共享](#proof-can-be-downloaded-has-a-message-and-is-shared-publicly)
* [更新阶段，使其不是私有的，而不是强制的，并且只需要一次批准](#update-a-stage-so-that-it-is-not-private-not-mandatory-and-requires-only-one-approval)
* [在没有主要决策者的校样中添加两个收件人](#add-two-recipients-to-a-proof-with-no-primary-decision-maker)

**校样可以下载、包含消息并公开共享**

有关此端点的文档可在 [ProofHQ API updateProof](https://api.proofhq.com/home/proofs/updateproof.html) 页面。

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

**更新阶段，使其不是私有的，而不是强制的，并且只需要一次批准**

有关此端点的文档可在 [ProofHQ API updateWorkflowProofStage](https://api.proofhq.com/updateworkflowproofstage.html) 页面。

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

**在没有主要决策者的校样中添加两个收件人**

有关此端点的文档可在 [ProofHQ API addWorkflowProofReviewers](https://api.proofhq.com/addworkflowproofreviewers.html) 页面。

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

## 在Workfront API中使用JSON创建校样

本节介绍如何使用Workfront API中的JSON作为参数值，通过高级校对选项创建校样

### 使用高级校对选项创建校样

您可以使用 `Document createProof` 操作。 此操作接受 `advancedProofingOptions` 参数，其值类型为 `string`. 要在 `createProof` 操作时，必须在 `advancedProofingOptions` 参数。

>[!NOTE]
很难预测advancedPoofingOptions JSON中包含的字段。 您可能希望在Workfront中使用高级校对时检查贵组织的网络数据，并将JSON基于贵组织常用的字段和值。
由于这些字段可能很难预测，因此我们建议先使用Workfront API创建校样，然后使用ProofHQ API更新它。 有关更多信息，请参阅 [使用Workfront和ProofHQ API创建校样（推荐）](#create-a-proof-using-the-workfront-and-proofhq-apis-recommended) 在本文中

### 示例

此示例显示了在为 `advancedProofingOptions` 参数。 您的 `advancedProofingOptions` JSON文件中的字段可能多于或少于此处显示的字段。

**示例:**

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
