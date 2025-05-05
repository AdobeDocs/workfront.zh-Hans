---
content-type: api
navigation-topic: api-navigation-topic
title: API版本15中的新增功能
description: Adobe Workfront于2022年6月14日发布了API版本14。 API版本15具有对版本14的以下更改。
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 0%

---

# API版本15中的新增功能

Adobe Workfront于2022年6月14日发布了API版本15。 API版本15具有对版本14的以下更改。

## 已添加资源

* [计划(INITIV)](#Initiati)

* [Issdef (ISSDEF)](#IssueDef)

* [对象集成(OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [用户审批(USRAPV)](#UserAppr)

### 计划(INITIV)

计划对象在Workfront Scenario Planner中为工作角色的类型和数量、固定成本和计划福利创建估计值。

有关计划的详细信息，请参阅Scenario Planner[&#128279;](../../scenario-planner/initiatives-overview.md)中的计划概述。

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
            <p>这是一个内部对象。</p>
          </li>
          <li>
            <p><b>持续时间</b>
            </p>
            <p>endDate和startDate之间的时间量。</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>计划的计划完成日期。</p>
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
            <p><b>计划ID</b>
            </p>
            <p>与计划关联的ID。</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>上次在Workfront Scenario Planner中发布计划的日期。</p>
          </li>
          <li>
            <p><b>名称</b>
            </p>
            <p>计划的名称</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>与计划关联的计划的ID。</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>与计划关联的计划的名称。</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>与计划关联的项目的ID。</p>
          </li>
          <li>
            <p><b>方案ID</b>
            </p>
            <p>Workfront Scenario Planner中与计划关联的方案的ID。</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>计划的计划开始日期。</p>
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
            <p><b>输入者</b>
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
            <p><b>名称</b>
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
      <td role="rowheader">运营</td>
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
            <p><b>报告</b>
            </p>
          </li>
          <li>
            <p><b>搜索</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Issdef (ISSDEF)

IssueDef对象表示关于问题格式的一组数据。 此对象可以附加到项目或模板，并影响添加到该项目或模板的问题。

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

### 对象集成(OBJINT)

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
            <p>这是一个内部对象。</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>将ObjectIntegration输入到Workfront系统中的日期和时间。</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>特定ObjectIntegration对象的唯一Workfront ID。</p>
          </li>
          <li>
            <p><b>集成类型</b>
            </p>
            <p>ObjectIntegration对象用于创建链接的外部软件。 可能的值包括：</p>
            <ul>
              <li>
                <p>JIRA</p>
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
            <p>Workfront中与ObjectIntegration关联的对象。</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>与ObjectIntegration关联的Workfront中对象的对象代码。</p>
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

### TaskDef (TSKDEF)

TaskDef对象表示关于任务格式的一组数据。 此对象可以附加到项目或模板，并影响添加到该项目或模板的任务。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
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
            <p><b>对象类别
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

### 用户审批(USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段 </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
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
            <p><b>请求者ID</b>
            </p>
          </li>
          <li>
            <p><b>状态</b>
            </p>
          </li>
          <li>
            <p><b>用户ID</b>
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
            <p><b>审批者</b>
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
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>请求者ID</b>
            </p>
          </li>
          <li>
            <p><b>状态</b>
            </p>
          </li>
          <li>
            <p><b>用户ID</b>
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
      <td role="rowheader">运营</td>
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
            <p><b>报告</b>
            </p>
          </li>
          <li>
            <p><b>搜索</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## 已删除资源

未删除API版本15的资源。

## 已修改的资源

* [访问级别(ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSURL)](#AccessRu)

* [批准(APPROVAL)](#Approval)

* [类别(CTGY)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [客户首选项(CUSTPR)](#Customer)

* [文档文件夹(DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [组（组）](#Group)

* [日志条目(JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [Op任务/问题(OPTASK)](#OpTask)

* [参数（参数）](#Paramete)

* [Portfolio（端口）](#Portfoli)

* [计划(PRGM)](#Program)

* [项目（项目）](#Project)

* [QueueDef (QUED)](#QueueDef)

* [记分卡问题(SCOREQ)](#ScoreCar)

* [任务（任务）](#Task)

* [模板（模板）](#Template)

* [时间表(TSHET)](#Timeshee)

* [视图(UIVIEW)](#View)

* [更新（更新）](#Update)

* [用户（用户）](#User)

* [用户注释(USRNOT)](#UserNote)

* [工作（工作）](#Work)

### 访问级别(ACSLVL)

AccessLevel对象与用户相关联，并描述确定用户可以访问的AccessLevelPermissions集。

有关访问级别的详细信息，请参阅[访问级别](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md)。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> （字符串[]）</p>
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

### AccessLevelPermissions (ALVPER)

AccessLevelPermissions对象表示访问、创建或修改Workfront对象的特定权限。 然后，可将这些权限与访问级别关联。

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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

如果用户无权访问Workfront中他们需要的对象，则可以请求对该对象的访问权限。 AccessRequest对象表示此请求。

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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b>（字符串）</p>
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

### AccessRule (ACSURL)

AccessRule对象表示自定义访问级别中的规则集，该规则集确定用户如何共享他们创建的项目。

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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 批准(APPROVAL)

给定工作项，如任务、文档或时间表，可能要求主管或其他用户签发该工作项。 审批对象表示在工作项上注销的操作。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours </b>
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
            <p><b>计划</b>
            </p>
            <p>已添加。</p>
            <p>计划对象在Workfront Scenario Planner中为工作角色的类型和数量、固定成本和计划福利创建估计值。 </p>
          </li>
          <li>
            <p><b>问题定义</b>
            </p>
            <p>已添加。</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>已添加。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>对象集成
</b>
            </p>
            <p style="font-weight: normal;">已添加。</p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 类别(CTGY)

Category对象是自定义表单。

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
                <p>组（组）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>已添加。</p>
            <p style="font-weight: normal;">此参数是可附加自定义表单的可能对象的数组。 添加了它以支持将自定义表单附加到多种对象类型的功能。</p>
            <p>可能的值： </p>
            <p>CMPY、端口、PRGM、项目、任务、OPTASK、用户、DOCU、EXPN、ITRN、帐单、组</p>
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
            <p>已添加。</p>
            <p style="font-weight: normal;">此参数是可附加自定义表单的可能对象的数组。 添加了它以支持将自定义表单附加到多种对象类型的功能。</p>
            <p>可能的值： </p>
            <p>CMPY、端口、PRGM、项目、任务、OPTASK、用户、DOCU、EXPN、ITRN、帐单、组</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

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
            <p>已添加。</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>已添加。</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>已添加。</p>
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
            <p><b>名称</b>
            </p>
            <p>添加了以下值：</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint (Graph API)集成已启用)</p>
                <p>此值支持更新的Sharepoint集成。</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> （允许用户在不使用模板的情况下创建项目）</p>
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

### 文档文件夹(DOCFDR)

可以将文档组织到文件夹中。 您可以在个人文档区域中创建个人文件夹。 DocumentFolder对象表示这些文件夹之一。

DocumentFolder对象添加了标志`SHARABLE`。

### DocumentVersion (DOCV)

DocumentVersion对象表示文件的特定版本（如书面材料、图像或其他形式的信息）。

有关文档版本的详细信息，请参阅[上载文档的新版本](../../documents/managing-documents/upload-new-document-version.md)。

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
                <p><code>SHAREPOINT_V2</code> (SharePoint （图形API）)</p>
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

组对象表示一组用户和团队。 组通常代表部门结构。

有关组的更多信息，请参阅组与团队。

组对象添加了标志`DATA_EXTENDIBLE`

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
            <p><b>类别ID</b>
            </p>
            <p>类别是自定义表单。 添加此参数是为了支持向组对象添加自定义Forms的功能。 </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>这是一个布尔参数，如果对象处于Active状态，则该参数的值为true ；否则为false。 设置为“活动”的对象会显示在下拉菜单和预输入字段中，并可附加到其他对象。</p>
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
            <p><b>审批者</b>
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
            <p><b>对象类别</b>
            </p>
          </li>
          <li>
            <p><b>对象集成</b>
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
            <p>这是一个布尔参数，如果对象处于Active状态，则该参数的值为true ；否则为false。 设置为“活动”的对象会显示在下拉菜单和预输入字段中，并可附加到其他对象。</p>
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
            <p>此操作重新计算自定义表单字段中的表达式。</p>
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

### 日志条目(JRNLE)

JournalEntry对象可以设置为在修改特定对象字段时记录这些字段的相关信息。 将某个字段设置为记录为日志条目对象的一部分时，每次修改该字段时将创建相应的日志条目。

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

### LinkedFolder (LNKFDR)

LinkedFolder对象表示从外部文档提供商(如Google驱动器或Dropbox)链接的文件夹。

有关链接的文件夹的详细信息，请参阅从外部应用程序链接文档。

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
                <p><code>SHAREPOINT_V2</code> (SharePoint （图形API）)</p>
                <p>此值支持更新的Sharepoint集成。</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Op任务/问题(OPTASK)

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

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
        <p>已修改以下操作：</p>
        <ul>
          <li>
            <p><b>复制问题</b>
            </p>
            <p>已添加字段 <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 参数（参数）

Parameter对象是一个自定义字段。

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
        <p>以下字段已修改：</p>
        <ul>
          <li>
            <p><b>数据类型</b>
            </p>
            <p>已添加可能的值<code>WIDGET </code>（小组件） </p>
            <p>此值支持在自定义表单中使用图像。</p>
          </li>
          <li>
            <p><b>显示类型</b>
            </p>
            <p>已添加可能的值<code>WIDGET </code>（小组件）</p>
            <p>此值支持在自定义表单中使用图像。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio（端口）

Portfolio对象是争夺相同资源（通常是资金或人员来完成这些资源）的项目集合。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象集成</b>
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

### 计划(PRGM)

项目群对象是项目组合中项目的子集，其中类似的项目可以分组在一起。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象集成</b>
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

### 项目（项目）

项目是Workfront中的工作项，是Workfront帮助人们完成工作方式中的主要构建基块。 Project对象表示一组具有通用、特定目标的任务。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>resourcePlannerBudgetedHours</b>
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
            <p><b>计划</b>
            </p>
            <p>计划对象在Workfront Scenario Planner中为工作角色的类型和数量、固定成本和计划福利创建估计值。 </p>
          </li>
          <li>
            <p><b>问题定义</b>
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
            <p><b>对象集成</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

QueueDef对象表示队列，这是一个已发布到技术支持区域以允许用户向其提交问题的项目。

有关请求队列的详细信息，请参阅[创建请求队列](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
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
                <p>EDIT_TEAMS_I_GROUP_ADMIN(编辑我管理的组中的团队（仅限组管理员）)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 记分卡问题(SCOREQ)

ScoreCardQuestion对象表示已添加到记分卡的问题。 这些问题通常由Portfolio经理决定，这些问题的答案让经理能够了解项目与项目组合目标的符合程度。

有关记分卡问题的详细信息，请参阅[创建记分卡](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>显示类型</b>
            </p>
            <p>已添加可能的值<code>WIDGET </code>（小组件）</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 任务（任务）

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象集成</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 模板（模板）

Template对象表示项目的模式。 可使用模板创建项目以节省时间。 模板包含团队和任务，这些团队和任务将被复制到从该模板创建的任何项目中。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li>
            <p><b>问题定义</b>
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

### 时间表(TSHET)

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <p>已删除以下字段：</p>
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

### 视图(UIVIEW)

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
            <p>已删除以下可能值：</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> （四列式布局）</p>
              </li>
              <li>
                <p><code>UPDATES</code> （更新）</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> （更新）</p>
              </li>
              <li>
                <p><code>WORKINGON</code> （正在处理）</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> （自定义数据）</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> （更新自定义数据）</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> （状态更新）</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> （状态更新）</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> （状态更新）</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> （状态更新）</p>
              </li>
              <li>
                <p><code>DLIST</code> （详细信息列表）</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> （详细信息列表部分）</p>
              </li>
            </ul>
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
            <p><b>updateType</b>
            </p>
            <p>添加了可能的值<code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 用户（用户）

User对象表示在Workfront中拥有帐户的人员，该帐户可以登录并与系统交互。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li>
            <p><b>用户审批</b>
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
            <p><b>eventType</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>DUP </code>（要求您证明文档）</p>
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

Work对象是Task和OpTask都继承的公用接口，它们共享公用代码。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象集成</b>
            </p>
            <p>在某些情况下，可以将Workfront工作项直接链接到外部软件产品中的对象。 ObjectIntegration对象表示此链接。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
