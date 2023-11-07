---
content-type: api
navigation-topic: api-navigation-topic
title: API版本17中的新增功能
description: Adobe Workfront于2022年4月6日发布了API版本17。 API版本17具有来自版本15的以下更改。
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 4%

---

# API版本17中的新增功能

Adobe Workfront于2023年10月12日发布了API版本17。 API版本17具有来自版本16的以下更改。

## 已添加资源

<!--

### Booking (BOOKNG)

-->

### 外部文档(EXTDOC)

ExternalDocument对象是位于Workfront外部的文档存储提供商中的文档或其他数字资源。 这些资源可以链接到Workfront，也可以从进行链接。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>描述</b></p></li>
          <li><p><b>documentProviderId</b></p></li>
          <li><p><b>分机</b></p></li>
          <li><p><b>文件类型</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>路径</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>只读</b></p></li>
          <li><p><b>大小</b></p></li>
          <li><p><b>缩略图URL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>描述</b></p></li>
          <li><p><b>documentProviderId</b></p></li>
          <li><p><b>分机</b></p></li>
          <li><p><b>文件类型</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>对象代码</b></p></li>
          <li><p><b>路径</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>只读</b></p></li>
          <li><p><b>大小</b></p></li>
          <li><p><b>缩略图URL</b></p></li>
          <li><p><b>值</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">默认字段</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>对象代码</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObject</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">查询</td>
      <td>
        <ul>
          <li><p><b>browslist</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>客户ID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li><p><b>客户</b></p></li>
          <li><p><b>用户</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>对象代码</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## 已删除资源

没有为API版本17删除资源

## 已修改的资源

已为API版本17修改以下资源。

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### 基线(BLIN)

基线是给定时刻项目性能的快照。 它们存储有关项目的关键信息，如关键日期、进度、成本和收入值。

Baseline对象删除了标记 **INLINE_EDITABLE**.

### 记帐记录(BILL)

BillingRecord对象记录可记帐的收入、小时数或费用。 此信息可用于在外部会计系统中创建发票。

BillingRecord对象删除了标志 **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### 公司(CPY)

Company对象表示由人员集合组成的组织。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>defaultinterface</b>
            </p>
            <p>已删除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 客户首选项(CUSTPR)

CustomerPreferences对象表示客户为其Workfront实例设置的首选项集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>添加了可能的值“config.defaultToNewHomeDescription”(customer：config.defaultToNewHome)&gt;/p？<p>这允许组织将新的主页体验设置为用户的默认体验。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>添加了可能的值“Frame.io”(FRAMEIO)</p>
          </li>
          <li>
            <p><b>文件类型</b>
            </p>
            <p>添加了可能的值“enum.filetype.site”（站点）</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 汇率（汇率）

ExchangeRate对象表示在Workfront中设置的货币汇率。 ExchangeRate对象不是动态的。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段：
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>已添加.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### 费用(EXPN)

费用代表在项目期限内可能产生的非人工成本。

Expense对象删除了标记 **INLINE_EDITABLE**.

### 组（组）

组对象表示一组用户和团队。 组通常代表部门结构。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>defaultinterface</b>
            </p>
            <p>已删除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hour (HOUR)

Hour对象表示用户在时间表上记录的小时。

Hour对象删除了标志 **INLINE_EDITABLE**.

### 迭代(ITRN)

小版本对象表示单个敏捷小版本。 迭代是离散的时间段，用于规划和完成Agile故事。

Iteration对象删除了标志 **INLINE_EDITABLE**.


### 日志条目(JRNLE)

JournalEntry对象可以设置为在修改特定对象字段时记录这些字段的相关信息。 将某个字段设置为记录为日志条目对象的一部分时，每次修改该字段时将创建相应的日志条目。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>已添加审批者(AAA)</li>
              <li>已添加审阅者(AAR)</li>
              <li>已移除审阅人(ARR)</li>
              <li>已移除审批者(ARA)</li>
              <li>批准的决定(ADA)</li>
              <li>已批准有更改的决策(ADC)</li>
              <li>决策需求工作(ADN)</li>
              <li>撤销的决策(ADR)</li>
              <li>审批者已更改(AAC)</li>
              <li>审阅者已更改(ARC)</li>
              <li>审阅完成(RDC)</li>
              <li>审阅已撤销(RDR)</li>
              <li>发布(PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban板(KNBNBD)

Kanban展示板用于在Agile环境中跟踪任务。

Kanban Board对象删除了标志 **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

LinkedFolder对象表示从外部文档提供商(如Google驱动器或Dropbox)链接的文件夹。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>添加了可能的值“Frame.io (FRAMEIO)”</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Op任务/问题(OPTASK)

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

Issue对象删除了标记 **INLINE_EDITABLE**.

### 项目（项目）

项目是Workfront中的工作项，是Workfront帮助人们完成工作方式中的主要构建基块。 Project对象表示一组具有通用、特定目标的任务。

Project对象删除了标志 **INLINE_EDITABLE**.

### 项目用户(PRTU)

ProjectUser对象表示与特定项目关联的用户。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### 比率（比率）

Rate对象表示Workfront中的记帐费率。

Rate对象删除了标志 **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>添加了以下操作以支持费率卡功能：
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>此 <b>setRatesForRole</b> 已修改操作以添加以下字段：
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 风险（风险）

风险对象表示可能会阻止项目按时完成或在预算内完成的可能事件。 在规划阶段的项目会增加风险，以在批准任何工作之前确定潜在的障碍。

Risk对象删除了标记 **INLINE_EDITABLE**.

### 角色/工作角色(ROLE)

角色对象（工作角色）表示用户可能填充的功能能力或技能集，如设计人员或产品经理。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>defaultinterface</b>
            </p>
            <p>已删除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 任务（任务）

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

Task对象删除了标志 **INLINE_EDITABLE**.

### 团队(TEAMOB)

团队对象是可分配给工作项的用户的集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>defaultinterface</b>
            </p>
            <p>已删除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 团队成员(TEAMMB)

TeamMember对象是与特定团队关联的用户。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 模板用户(TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 时间表(TSHET)

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象代码</b>
            </p>
            <p>已删除</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 更新（更新）

可以更新Workfront中的工作项以通知用户当前状态。 Update对象表示这些更新之一。 更新可由用户输入或由Workfront系统创建。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>添加了以下值：</p>
            <ul>
              <li>已添加审批者(assetapprovalAddApprover)</li>
              <li>已添加审阅人(assetapprovalAddReviewer)</li>
              <li>已移除审批者(assetapprovalRemoveApprover)</li>
              <li>已删除审阅人(assetapprovalRemoveReviewer)</li>
              <li>已批准决策(assetapprovalDecisionApproved)</li>
              <li>决策需求工作(assetapprovalDecisionNeedsWork)</li>
              <li>已批准有更改的决策(assetapprovalDecisionApprovedChanges)</li>
              <li>已撤消决策(assetapprovalDecisionRevoced)</li>
              <li>审批者已更改(assetapprovalApproverChanged)</li>
              <li>审阅人已更改(assetapprovalReviewerChanged)</li>
              <li>审阅完成(assetapprovalReviewerDecisionComplete)</li>
              <li>审阅已撤销(assetapprovalReviewerDecisionRevoced)</li>
              <li>外部文档发送错误(externalDocumentSendError)</li>
              <li>已发布的文档版本(documentVersionPublish)</li>
              <li>链接的文件夹工作流(linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### 用户（用户）

User对象表示在Workfront中拥有帐户的人员，该帐户可以登录并与系统交互。

User对象删除了标记 **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>工作时间</b>
            </p>
            <p>此字段已添加，并且是一个介于0和1之间的数字，表示用户每天可以在项目工作（非开销工作）上花费的时间百分比。 值为1意味着用户可以100%地花费在项目工作上。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 用户组(USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 用户注释(USRNOT)

UserNote对象是通知。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>添加了以下值：</p>
            <ul>
              <li>文档需要您的审批(AAA)</li>
              <li>文档需要您的审核(AAR)</li>
              <li>文档不再需要您的审批(ARA)</li>
              <li>文档不再需要您的审核(ARR)</li>
              <li>文档需要（用户）的批准(ATA)</li>
              <li>文档需求（用户）审核(ATR)</li>
              <li>文档不再需要（用户）批准(RTA)</li>
              <li>文档不再需要（用户）审核(RTR)</li>
              <li>已批准文档(ADA)</li>
              <li>已审批但有更改的文档(ADC)</li>
              <li>文档需求工作(ADN)</li>
              <li>（用户）已将（文档）标记为已批准。 不再需要您的审批. (AAN)</li>
              <li>（用户）已将（文档）标记为已批准，但有更改。 不再需要您的审批. (ACN)</li>
              <li>（用户）已将（文档）标记为需要工作。 不再需要您的审批. (AWN)</li>
              <li>文档需要您立即审核而不是批准(AAC)</li>
              <li>文档需要您立即批准而不是审阅(ADN)</li>
              <li>已审阅文档(RDC)</li>
              <li>已审阅文档(TRC)</li>
              <li>（用户）已审阅（文档）为完成。 不再需要您审阅. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 用户角色(USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
