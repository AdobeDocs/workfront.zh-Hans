---
content-type: api
navigation-topic: api-navigation-topic
title: API版本15的新增功能
description: Adobe Workfront于2022年6月14日发布了API版本14。 API版本15具有与版本14相比的以下更改。
author: Becky
feature: Workfront API
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# API版本15的新增功能

Adobe Workfront于2022年6月14日发布了API版本15。 API版本15具有与版本14相比的以下更改。

## 添加了资源

* [倡议](#Initiati)

* [IssueDef(ISSDEF)](#IssueDef)

* [ObjectIntegration(OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue(GRCVAL)](#RichText)

* [TaskDef(TSKDEF)](#TaskDef)

* [用户批准(USRAPV)](#UserAppr)

### 倡议

“方案”对象在Workfront方案计划员中创建任务职责的种类和数量、固定成本和计划福利的估计。

有关计划的更多信息，请参阅 [方案规划器中的方案概述](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>这是内部对象。</p>
          </li>
          <li>
            <p><b>持续时间</b>
            </p>
            <p>endDate和startDate之间的间隔时间。</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>方案的计划完成日期。</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>与提交请求的用户关联的ID。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>与操作关联的ID</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>与方案关联的ID。</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>在Workfront方案规划器中上次发布方案的日期。</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>计划的名称</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>与计划关联的计划ID。</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>与方案关联的计划的名称。</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>与方案关联的项目的ID。</p>
          </li>
          <li>
            <p><b>方案ID</b>
            </p>
            <p>与方案关联的Workfront方案计划员中方案的ID。</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>计划的起始日期。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <ul>
          <li>
            <p><b>客户</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>项目</b>
            </p>
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
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>计数</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>报表 </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef(ISSDEF)

IssueDef对象表示一组与问题格式有关的数据。 此对象可以附加到项目或模板，并影响添加到该项目或模板的问题。

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
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration(OBJINT)

在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>这是内部对象。</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>将ObjectIntegration输入Workfront系统的日期和时间。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>特定ObjectIntegration对象的唯一Workfront ID。</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>ObjectIntegration对象创建链接的外部软件。 可能的值包括：</p>
            <ul>
              <li>
                <p>吉拉</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>ObjectIntegration与之关联的Workfront中的对象。</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>ObjectIntegration所关联的Workfront中对象的对象代码。</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <ul>
          <li>
            <p><b>客户</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef(TSKDEF)

TaskDef对象表示一组与任务格式有关的数据。 此对象可以附加到项目或模板，并影响添加到该项目或模板的任务。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlanedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 用户批准(USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段 </td>
      <td>
        <ul>
          <li>
            <p><b>审批者ID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>状态</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <ul>
          <li>
            <p><b>审批人</b>
            </p>
          </li>
          <li>
            <p><b>客户</b>
            </p>
          </li>
          <li>
            <p><b>请求者</b>
            </p>
          </li>
          <li>
            <p><b>用户</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">默认字段</td>
      <td >
        <ul>
          <li>
            <p><b>审批者ID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>状态</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>批准</b>
            </p>
          </li>
          <li>
            <p><b>拒绝</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>添加</b>
            </p>
          </li>
          <li>
            <p><b>计数</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>报表</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## 删除的资源

未删除API版本15的资源。

## 修改的资源

* [AccessLevel(ACSLVL)](#AccessLe)

* [AccessLevelPermissions(ALVPER)](#AccessLe2)

* [AccessRequest(ACSREQ)](#AccessRe)

* [AccessRule(ACSRUL)](#AccessRu)

* [批准（批准）](#Approval)

* [类别(CTGY)](#Category)

* [类别参数(CTGYPA)](#Category2)

* [客户首选项(CUSTPR)](#Customer)

* [DocumentFolder(DOCFDR)](#Document)

* [DocumentVersion(DOCV)](#Document2)

* [组（组）](#Group)

* [JournalEntry(JRNLE)](#JournalE)

* [LinkedFolder(LNKFDR)](#LinkedFo)

* [OpTask /问题(OPTASK)](#OpTask)

* [参数(PARAM)](#Paramete)

* [Portfolio（端口）](#Portfoli)

* [方案](#Program)

* [项目(PROJ)](#Project)

* [QueueDef(QUED)](#QueueDef)

* [ScoreCardQuestion(SCOREQ)](#ScoreCar)

* [任务（任务）](#Task)

* [模板(TMPL)](#Template)

* [工时单(TSHET)](#Timeshee)

* [查看(UIVIEW)](#View)

* [更新（更新）](#Update)

* [用户（用户）](#User)

* [UserNote(USRNOT)](#UserNote)

* [工作（工作）](#Work)

### AccessLevel(ACSLVL)

AccessLevel对象与用户相关联，并描述一组AccessLevelPermissions，这些AccessLevelPermissions决定用户可以访问哪些内容。

有关访问级别的更多信息，请参阅 [访问级别](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>VTMAWMG（查看与我的组关联的团队）</p>
              </li>
              <li>
                <p>VALLTM（查看所有团队）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions(ALVPER)

AccessLevelPermissions对象表示访问、创建或修改Workfront对象的特定权限。 然后，这些权限可以与访问级别关联。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest(ACSREQ)

如果用户无权访问其所需的Workfront中的对象，则他们可以请求访问该对象。 AccessRequest对象表示此请求。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>操作</b> （字符串）</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> （字符串）</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>WDL</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule(ACSRUL)

AccessRule对象表示自定义访问级别中的规则集，用于确定用户如何共享他们创建的项目。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 批准（批准）

给定工作项（如任务、文档或时间表）可能要求主管或其他用户在工作项上签名。 “批准”对象表示在工作项上注销的操作。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerDektedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <ul>
          <li>
            <p><b>主动性</b>
            </p>
            <p>已添加.</p>
            <p>“方案”对象在Workfront方案计划员中创建任务职责的种类和数量、固定成本和计划福利的估计。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>已添加.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">已添加.</p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 类别(CTGY)

类别对象是自定义表单。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b> （字符串）</p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>集团（集团）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>已添加.</p>
            <p style="font-weight: normal;">此参数是可附加自定义表单的可能对象数组。 添加了此插件，以支持将自定义表单附加到多种类型对象的功能。</p>
            <p>可能值： </p>
            <p>CMPY、PORT、PRGM、PROJ、TASK、OPTASK、USER、DOCU、EXPNS、ITRN、BILL、GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>已添加.</p>
            <p style="font-weight: normal;">此参数是可附加自定义表单的可能对象数组。 添加了此插件，以支持将自定义表单附加到多种类型对象的功能。</p>
            <p>可能值： </p>
            <p>CMPY、PORT、PRGM、PROJ、TASK、OPTASK、USER、DOCU、EXPNS、ITRN、BILL、GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 类别参数(CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>已添加.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>已添加.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>已添加.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 客户首选项(CUSTPR)

CustomerPreferences对象表示客户为其Workfront实例设置的一组首选项。

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
            <p>添加了以下值：</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (已启用 SharePoint (Graph API) 集成)</p>
                <p>此值支持更新的Sharepoint集成。</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (允许用户在不使用模板的情况下创建项目)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder(DOCFDR)

文档可以组织到文件夹中。 您可以在个人文档区域中创建个人文件夹。 DocumentFolder对象表示其中一个文件夹。

DocumentFolder对象添加了标记 `SHARABLE`.

### DocumentVersion(DOCV)

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

有关文档版本的更多信息，请参阅 [上传文档的新版本](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>添加了以下值： </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>此值支持更新的Sharepoint集成。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 组（组）

组对象表示一组用户和团队。 团体通常代表部门结构。

有关群组的更多信息，请参阅群组与团队。

Group对象添加了标记 `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <p>添加了以下字段：</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>类别是自定义表单。 添加此参数是为了支持将自定义Forms添加到组对象的功能。 </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>如果对象处于活动状态，则此参数是一个布尔参数，如果对象处于活动状态，则其值为true；如果对象处于非活动状态，则为false。 设置为“活动”(Active)的对象显示在下拉菜单和提前键入字段中，并可附加到其他对象。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <p>添加了以下字段：</p>
        <ul>
          <li>
            <p><b>审批人</b>
            </p>
          </li>
          <li>
            <p><b>客户</b>
            </p>
          </li>
          <li>
            <p><b>请求者</b>
            </p>
          </li>
          <li>
            <p><b>用户</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <p>添加了以下字段：</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">默认字段</td>
      <td >
        <p>添加了以下字段：</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>如果对象处于活动状态，则此参数是一个布尔参数，如果对象处于活动状态，则其值为true；如果对象处于非活动状态，则为false。 设置为“活动”(Active)的对象显示在下拉菜单和提前键入字段中，并可附加到其他对象。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <p>添加了以下字段：</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>此操作将重新计算自定义表单字段中的表达式。</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry(JRNLE)

JournalEntry对象可设置为在修改特定对象字段时记录有关这些字段的信息。 将字段设置为作为“日记帐分录”对象的一部分进行记录时，每次修改该字段时，都会创建相应的“日记帐分录”。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>添加了以下值： </p>
        <ul>
          <li>
            <p>DW（下载）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder(LNKFDR)

LinkedFolder对象表示从外部文档提供程序链接的文件夹，如Google驱动器或Dropbox。

有关链接文件夹的更多信息，请参阅从外部应用程序链接文档。

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
            <p>添加了以下值： </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>此值支持更新的Sharepoint集成。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask /问题(OPTASK)

OpTask对象通常称为问题。 问题是一个工作项，通常指示存在阻止完成任务或项目的问题。 问题也可以是帮助台请求。 更改订单、请求和错误也是问题。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <p>添加了以下操作：</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>修改了以下操作：</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>添加了字段 <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 参数(PARAM)

参数对象是自定义字段。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <p>添加了以下字段：</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>修改了以下字段：</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>添加了可能的值 <code>WIDGET </code>（小组件） </p>
            <p>此值支持在自定义表单中使用图像。</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>添加了可能的值 <code>WIDGET </code>（小组件）</p>
            <p>此值支持在自定义表单中使用图像。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（端口）

Portfolio对象是争夺相同资源（通常是资金或人员）的项目集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 方案

项目组合中的项目是项目对象的子集，可以将相似项目组合在一起。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 项目(PROJ)

项目是Workfront内的工作项，是Workfront帮助人们工作方式的主要构建基块。 项目对象表示一组具有相同特定目标的任务。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerDektedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td >
        <ul>
          <li>
            <p><b>主动性</b>
            </p>
            <p>“方案”对象在Workfront方案计划员中创建任务职责的种类和数量、固定成本和计划福利的估计。 </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef(QUED)

QueueDef对象表示Queue，该Queue是已发布到“帮助台”区域以允许用户向其提交问题的项目。

有关请求队列的更多信息，请参阅 [创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON（编辑我所在的团队）</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN(在我管理的组中编辑团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion(SCOREQ)

ScoreCardQuestion对象表示已添加到记分卡中的问题。 这些问题通常由Portfolio经理确定，他们的回答使经理能够了解项目与项目组合目标的一致程度。

有关记分卡问题的更多信息，请参阅 [创建记分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>添加了可能的值 <code>WIDGET </code>（小组件）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 任务（任务）

任务对象表示一个工作项，必须将该工作项作为实现最终目标（完成项目）的步骤来执行。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 模板(TMPL)

模板对象表示项目的模式。 可以从模板创建项目以节省时间。 模板包含团队和任务，这些团队和任务将复制到使用该模板创建的任何项目。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 工时单(TSHET)

时间表对象表示一个虚拟工时记录卡，它允许用户输入为任务、项目和间接费用小时类型工作的实际小时数。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <p>删除了以下字段：</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 查看(UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>删除了以下可能值：</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (四列式布局)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (更新)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (更新)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (正在处理)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (自定义数据)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (编辑自定义表单)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (状态更新)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (状态更新)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (状态更新)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (状态更新)</p>
              </li>
              <li>
                <p><code>DLIST</code> (详细信息列表)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (详细列表部分)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 更新（更新）

可以更新Workfront中的工作项，以便让用户了解当前状态。 更新对象表示这些更新之一。 更新可由用户输入或由Workfront系统创建。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
            <p>添加了可能的值 <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 用户（用户）

User对象表示在Workfront中具有可登录并与系统交互的帐户的人员。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserNote(USRNOT)

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
            <p><b>eventType</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>DUP </code>（请求您校样文档）</p>
              </li>
              <li>
                <p><code>DUV </code>（允许您查看文档）</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 工作（工作）

Work对象是Task和OpTask都可继承的通用接口，并在二者之间共享通用代码。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
