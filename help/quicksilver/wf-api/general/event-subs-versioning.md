---
content-type: api
navigation-topic: general-api
title: 事件订阅版本控制
description: 事件订阅API
author: Becky
feature: Workfront API
role: Developer
exl-id: 151b9d0d-0dd6-4ece-9601-dda04356b436
source-git-commit: e4ff9c9c44c75518e75b14209a18586363cdf4f5
workflow-type: tm+mt
source-wordcount: '1259'
ht-degree: 0%

---

# 事件订阅版本控制

Workfront提供两个版本的活动订阅。 本文介绍了它们之间的区别。

新版本不是对Workfront API的更改，而是对事件订阅功能的更改。

升级或降级事件订阅的功能确保在对事件结构做出更改时，现有订阅不会中断，从而允许您测试和升级到新版本，而不会在事件订阅中出现间隙。


将事件订阅升级或降级到另一个版本时，您在版本更改后的五分钟内，会收到每个事件交付的重复事件。 重复项包括事件订阅版本1和版本2中的一个。 这可确保不会因更改事件订阅版本而错过任何事件。

有关用于升级或降级事件订阅的端点的信息，请参阅事件订阅API一文中的[事件订阅版本控制](/help/quicksilver/wf-api/general/event-subs-api.md#event-subscription-versioning)。

>[!IMPORTANT]
>
>以下版本将影响事件订阅版本控制：
>
>* **25.2版本**（2025年4月10日）：在25.2版本之后创建的所有新订阅都创建为版本2。
>* **2026年1月15日**：所有剩余版本1订阅迁移到版本2。

## 版本1与版本2之间的更改

已对事件订阅版本2进行以下更改：


### 一般更改


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><b>受影响的字段</b></p> </th> 
   <th> <p><b>版本1（以前的行为）</b></p> </th> 
   <th> <p><b>版本2（更改）</b></p> </th> 
   <th> <p><b>修正操作</b></p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>计算参数值</p> </td> 
   <td> <p>从模板创建的任何对象，如果包含具有计算参数值的自定义表单，则将发送<code>CREATE</code>事件，然后随参数值（包括计算字段及其值）发送<code>UPDATE</code>。 </p> </td> 
   <td> <p>当从包含具有已计算参数值的自定义表单的模板创建对象时，将只发送<code>CREATE</code>事件，并将包含包括已计算字段的参数值。</p> </td> 
   <td> <p>如果您订阅了<code>UPDATE</code>个事件，并希望在使用计算的参数值创建对象后接收<code>UPDATE</code>事件，则您将不再接收该<code>UPDATE</code>事件。 如果您希望在创建对象时查看计算参数值，则必须创建其他<code>CREATE</code>订阅。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>多选类型字段</p> </td> 
   <td> <p>对于包含多选类型字段更改的任何类型事件，如果该字段仅包含一个值，则它将转换为并以字符串形式发送。 否则，它将作为数组发送。 </p><p>示例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> 已转换并作为<code>myMultiSelectField: "oneValue"</code>发送。</li><li><code>myMultiSelectField: ["first", "second"]</code> 作为<code>myMultiSelectField: ["first", "second"]</code>发送。</li></ul> </td> 
   <td> <p>无论数组中有多少值，它都将作为数组发送。 </p><p>示例：</p><ul><li><code>myMultiSelectField: ["oneValue"]</code> 作为<code>myMultiSelectField: ["oneValue"]</code>发送。</li><li><code>myMultiSelectField: ["first", "second"]</code> 作为<code>myMultiSelectField: ["first", "second"]</code>发送。</li></ul> </td> 
   <td> <p>如果您有一个预订，该预订在多选字段上具有筛选器，且值为字符串，则必须使用具有值为数组的相同筛选器创建新预订。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 对象特定的更改

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <b>对象代码</b> </th> 
   <th> <b>受影响的字段</b> </th> 
   <th> <b>版本1（上一个行为）</b></th> 
   <th> <b>版本2（更改）</b> </th> 
   <th> <b>修正操作</b> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th rowspan="1">分配</th> 
   <td>
    <ul>
     <li><code>projectID</code></li>
     <li><code>taskID</code></li>
     <li><code>opTaskID</code></li>
     <li><code>customerID</code></li>
    </ul> 
   </td> 
   <td>更新此对象时，<code>UPDATE</code>事件有时错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果对受影响的字段应用了过滤器，则只有在这些字段实际发生更改时，而不是任何其他值发生更改时，您才会收到<code>UPDATE</code>事件。
   </td> 
  </tr> 
  <tr> 
   <th rowspan="2">DOCU</th> 
   <td>
    <ul>
     <li><code>referenceObjID</code></li>
    </ul> 
   </td> 
   <td>在此对象上更新任何参数值时，<code>UPDATE</code>事件错误地显示受影响的字段从<code>null</code>更改为<code>object id</code>。 </td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果对受影响的字段应用了过滤器，则只有在这些字段实际发生更改时，而不是任何其他值发生更改时，您才会收到<code>UPDATE</code>事件。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>groups</code></li>
    </ul> 
   </td> 
   <td>删除文档时，<code>DELETE</code>事件将受影响的字段错误地显示为处于before状态的空数组。    </td> 
   <td><code>DELETE</code>事件正确显示了处于“之前”状态的受影响字段。</td> 
   <td>无。 <code>DELETE</code>事件仍将被发送，但现在显示受影响字段的正确数据。 
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">DOCV</th> 
  <td>
    <ul>
     <li><code>proofDecision</code></li>
     <li><code>proofName</code></li>
     <li><code>proofProgress</code></li>
    </ul> 
   </td> 
   <td>更新此对象时，将发送两个<code>UPDATE</code>事件。 第一个事件不包含受影响的字段，而第二个事件包含。</td> 
   <td>所有字段更新（包括受影响的字段）都仅存在于一个<code>UPDATE</code>事件中，并且不会发送第二个不必要的事件。     </td> 
   <td>无。 如果对受影响的字段应用了过滤器，则事件将在第一个事件中交付。 
</td> 
  </tr> 
  <tr> 
   <th rowspan="2">展开</th> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>为费用更新任何参数值时，<code>UPDATE</code>事件错误地显示了topReferenceObjCode从<code>EXPNS</code>更改为<code>PROJ</code>，<code>referenceObjectName</code>从<code>null</code>更改为<code>string value of project name</code>。      </td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果对受影响的字段应用了过滤器，则只有在这些字段实际发生更改时，而不是任何其他值发生更改时，您才会收到<code>UPDATE</code>事件。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>topReferenceObjCode</code></li>
     <li><code>referenceObjectName</code></li>
    </ul> 
   </td> 
   <td>删除费用对象时，在发送<code>DELETE</code>事件之前发送了<code>UPDATE</code>事件，并将受影响的字段更改为null。    </td> 
   <td>未发送额外的<code>UPDATE</code>事件。 <code>DELETE</code>事件具有处于“之前”状态的受影响字段的正确值。 </td> 
   <td>如果您对<code>UPDATE</code>事件中受影响的字段具有过滤器，并且希望在删除对象时收到该过滤器，则您将不再收到该<code>UPDATE</code>事件。 如果您希望在删除对象时看到这些字段，则必须创建其他<code>DELETE</code>订阅。
</td> 
  </tr> 
  <tr> 
   <th rowspan="1">HOUR</th> 
  <td>
    <ul>
     <li><code>projectID </code></li>
     <li><code>taskID </code></li>
     <li><code>roleID</code></li>
     <li><code>timesheetID</code></li>
     <li><code>hourTypeID </code></li>
     <li><code>projectOverheadID</code></li>
     <li><code>referenceObjID</code></li>
     <li><code>referenceObjCode</code></li>
     <li><code>securityRootID</code></li>
    </ul> 
   </td> 
   <td>删除此对象时，<code>DELETE</code>事件将受影响的字段错误地显示为<code>null</code>，其状态为“之前”。 </td> 
   <td><code>DELETE</code>事件正确显示了处于“之前”状态的受影响字段。</td> 
   <td>无。 <code>DELETE</code>事件仍会发送，但现在会显示受影响字段的正确数据。 </td> 
  </tr> 
  <tr> 
   <th rowspan="2">OPTASK</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>在此对象上更新任何参数值时，<code>UPDATE</code>事件错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。 </td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果受影响的字段上有筛选器，则仅当该字段实际发生更改时，而不是当任何其他参数值发生更改时，您才会收到<code>UPDATE</code>事件。
</td> 
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>resolveProjectID</code></li>
     <li><code>resolveTaskID</code></li>
     <li><code>resolvingObjID</code></li>
    </ul> 
   </td> 
   <td>更新此对象时，<code>UPDATE</code>事件有时错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件将显示受影响字段的正确值。    </td> 
   <td></td> 
  </tr> 
  <tr> 
   <th rowspan="2">项目</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   <td>在此对象上更新任何参数值时，<code>UPDATE</code>事件错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。 </td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果受影响的字段上有筛选器，则仅当该字段实际发生更改时，而不是当任何其他参数值发生更改时，您才会收到<code>UPDATE</code>事件。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>更新此对象时，<code>UPDATE</code>事件有时错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果受影响的字段上有筛选器，则仅当该字段实际发生更改时，而不是当任何其他参数值发生更改时，您才会收到<code>UPDATE</code>事件。
  </tr> 
  <tr> 
   <th rowspan="2">任务</th> 
  <td>
    <ul>
     <li><code>rootGroupID</code></li>
    </ul> 
   </td> 
   <td>在此对象上更新任何参数值时，<code>UPDATE</code>事件错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。 </td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果受影响的字段上有筛选器，则仅当该字段实际发生更改时，而不是当任何其他参数值发生更改时，您才会收到<code>UPDATE</code>事件。
  </tr> 
  <tr> 
  <td>
    <ul>
     <li><code>convertedOpTaskID</code></li>
    </ul> 
   </td> 
   <td>更新此对象时，<code>UPDATE</code>事件有时错误地显示受影响的字段从<code>null</code>更改为<code>ID value</code>。</td> 
   <td>所有<code>UPDATE</code>事件都显示受影响字段的正确值。</td> 
   <td>无。 如果受影响的字段上有筛选器，则仅当该字段实际发生更改时，而不是当任何其他参数值发生更改时，您才会收到<code>UPDATE</code>事件。
 </tbody> 
</table>


## 在Workfront Fusion场景中更新事件订阅版本

Workfront Fusion使用事件订阅来监视Workfront中的更改以触发场景。 您可以使用Workfront >更新事件有效负载版本模块，更新Fusion直接在场景中使用的事件订阅版本。

有关使用此模块的说明，请参阅Workfront Fusion文档中的[Workfront模块](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules)。
