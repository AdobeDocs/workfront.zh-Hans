---
content-type: api
navigation-topic: api-navigation-topic
title: 事件订阅资源字段
description: 事件订阅资源字段
author: Becky
feature: Workfront API
role: Developer
exl-id: 54859930-7619-4b93-8dff-29b10e43d6d5
source-git-commit: e53f845a00245049ac78616848d243453b2d57eb
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 9%

---

# 事件订阅资源字段

事件订阅资源字段表示事件的触发器，这些事件会导致事件订阅向配置的端点发送出站消息。 编辑资源字段时，会触发UPDATE事件。

请注意，可使用嵌套筛选功能筛选数据。 有关详细信息，请参阅文章事件订阅API中的[使用嵌套筛选器](/help/quicksilver/wf-api/general/event-subs-api.md#using-nested-filters)。

下表列出了可用于事件订阅资源的字段：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>资源</th> 
   <th>对象代码</th> 
   <th>字段</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>任务分配</td> 
   <td>分配</td> 
   <td>actualWorkCompleted</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>actualWorkPerDayStartDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> assignmentpercent </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> avgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 类别ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> classifierID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 客户ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> financeLastUpdateDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isPrimary</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> isteamassignment </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdateDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 对象代码 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 对象类别 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> opTaskID </td> 
  </tr>
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parametervalues </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedAvgWorkPerDay </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectedUserAllocationPercentage </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> projectID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> securityRootID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>状态</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>工作</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDate <p>[!BADGE 已删除]{type=negative tooltip="此字段已于2023年10月26日删除。"}</span></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workPerDayList</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>所需工作</td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>CMPY</td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> ID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> extRefId </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> groupID </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 对象代码 </td> 
  </tr> 
  <tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> parametervalues </td> 
  </tr> 
  <tr> 
  <tr> 
   <td>仪表板</td> 
   <td>PTLTAB</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>docID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>lastUpdateDate</p> <p>注意：LastUpdateDate仅在每日首次更新时触发事件。 </p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portalProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>DOCU</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>当前版本ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户：isAdvancedDocMgmtEnabled</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentRequestId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>组<p><b>注意</b>：此字段不可过滤。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>迭代标识</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lastUpdatedByID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>注释ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parametervalues</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>项目组合ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> <p>referencenumber</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>发行版本ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>顶对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>DocumentVersion</span> </td> 
   <td><span>文档</span> </td> 
   <td><span>accessorIDs</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>activeProofStages</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>documentProviderId</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>docSize</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>entryDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>enteredByID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>分机</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalIntegrationType</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>externalStorageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>文件名</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>文件类型</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>位置</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofApprovalStatusID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofedByUserID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDeadlineDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofName</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofOwnerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofPages</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofProgress</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofStageID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>版本</span> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>展开</td> 
   <td> 实际金额 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> actualUnitAmount </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> billingRecordID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 类别ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customFormsIDs</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>effectiondate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>expObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>费用类型ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isBillable</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 是可退还 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 已退还 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象类别</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedAmou</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedunitamount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjectName</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>顶对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>topReferenceObjID</td> 
  </tr> 
  <tr> 
   <td>字段</td> 
   <td>字段</td> 
   <td>createdat</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> createdby </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> customerId </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> dateOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 描述 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 显示名称 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 公式选项 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> hasError </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> linkedField </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> lookupOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 数字选项 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 对象代码 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> options </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> referenceOptions </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 类型 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 更新时间 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 更新者 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> userOptions </td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td>HOUR</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> 实际成本 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvedOnDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>dupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externalTimesheetID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>小时</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectOverheadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>状态</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>工时表ID</td> 
  </tr> 
  <tr> 
   <td>问题</td> 
   <td>OPTASK</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>迭代标识</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>优先次序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueTopicID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referencenumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referenceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveProjectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolveTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resolvingObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceObjId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>sourceTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>状态</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr> 
   <td>注释</td> 
   <td>注释</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachDocumentID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachObjID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachWorkUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>auditRecordId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>文档ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>外部服务ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>迭代标识</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>注释文本</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>opTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentInvaldationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentJournalEntryID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentNoteId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>项目组合ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>proofactionid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>richTextNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>主题</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>threadID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>工时表ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>顶对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>端口</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignmentScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>PRGM</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>项目组合ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td>项目</td> 
   <td>项目</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>alignmentScoreCardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>attachedRateCardID </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>货币</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverablescorecardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
    <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
<tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>里程碑路径ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>popaccountid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>preserveBilling</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>优先次序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referencenumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>subscriptorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>状态</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>校对审批</span> </td> 
   <td><span>PRFAPL</span> </td> 
   <td><span>accessorIDs</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>approverID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>customerID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>documentVersionID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>ID</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>isWaitingDecision</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>objCode</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>proofCreationDate</span> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> </td> 
   <td> </td> 
   <td><span>请求者ID</span> </td> 
  </tr> 
  <tr> 
   <td>记录</td> 
   <td>记录</td> 
   <td>createdat</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdby</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>数据<p><b>注意</b>：此字段不可过滤。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordExternalOptions</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordTypeId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新时间</td> 
  </tr> 
  <tr> 
   <td>记录类型 </td> 
   <td>记录类型 </td> 
   <td>颜色</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdat</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdby</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>数据<p><b>注意</b>：此字段不可过滤。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>显示名称</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>externaloptions</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>字段<p><b>注意</b>：此字段不可过滤。</p></td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>图标</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isExternal</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isTaxonomy</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>权限</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>primaryFieldId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordscount</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新时间</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新者</td> 
  </tr> 
  <tr> 
   <td>报告</td> 
   <td>PTLSEC</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>appGlobalID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>filterId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastViewedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>preferenceID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>publicRunAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>报告文件夹ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>runAsUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduledReportID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiObjCode</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>viewID</td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>任务</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>assignedToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>billingRecordID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>convertedOpTaskOriginatorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>currentApprovalStepID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>迭代标识</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>kanbanBoardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastConditionNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>里程碑ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>parentid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>plannedCompletionDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>优先次序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>projectID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recurrenceRuleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referencenumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rejectionIssueID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>rootGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>securityRootID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>状态</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>submittedById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>templateTaskID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr> 
   <td>模板</td> 
   <td>模板</td> 
   <td>accessourcides</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>approvalProcessID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>deliverablescorecardID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>描述</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>entryDate</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>groupID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>issueWorkflowAutomationId</td> 
  </tr> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>里程碑路径ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ownerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>优先次序</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>programID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>queueDefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>项目组合ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>referencenumber</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>subscriptorID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>taskWorkflowAutomationID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>teamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>Workflowautomationid</td> 
  </tr> 
  <tr> 
   <td>时间表</td> 
   <td>TSHET</td> 
   <td>approverID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>批准者列表字符串</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>显示名称</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>endDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hasnotes</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>hoursDuration</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>可编辑</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>overtimeHours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>regulathours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>startDate </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>状态</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>totalhours</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>userID</td> 
  </tr> 
  <tr> 
   <td>用户</td> 
   <td>用户</td> 
   <td>accessLevelID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>类别ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>companyID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>客户ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>defaultHourTypeID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>delegationToID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>eauthUserID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>电子邮件地址</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>enteredById</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>extRefId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeGroupID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>homeTeamID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>ID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>isActive</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastEnteredNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastLoginDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdateDate</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>lastUpdatedByID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>latestUpdateNoteID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>布局模板标识</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>logTimeInDays</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>managerID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>参数值*</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>portalProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>resourcePoolId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>roleID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>scheduleid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>timesheetProfileID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>标题</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uiTemplateID</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>uumuserid</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>workHoursPerDay </td> 
  </tr> 
  <tr> 
   <td>Workspace</td> 
   <td>Workspace</td> 
   <td>颜色</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdat</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>createdby</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>customerId</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>图标 </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>id</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>name</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>对象代码</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>权限</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>recordType</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新时间</td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td>更新者</td> 
  </tr> 
 </tbody> 
</table>

&#42;parameterValue是与各种Workfront资源（或对象）关联的自定义字段值。 事件订阅出站消息包含填充的parameterValues（自定义字段）的完整列表。
