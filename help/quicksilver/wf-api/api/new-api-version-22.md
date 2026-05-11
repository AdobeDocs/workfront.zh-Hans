---
content-type: api
navigation-topic: api-navigation-topic
title: API版本22中的新增功能
description: Adobe Workfront于2026年5月11日发布了API版本22。 API版本22具有对版本21的以下更改。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 2%

---

# API版本22中的新增功能

Adobe Workfront于2026年5月8日发布了API版本22。 API版本22具有对版本21的以下更改。

## 已添加资源

为API版本22添加了以下资源。

### ReportShareableFolder (RPSHFD)

您可以使用可共享报告文件夹来组织报告并与其他用户共享这些文件夹。 此功能专为管理大量报告并需要可扩展、一致的访问控制的团队而设计。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>对象代码</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">默认字段</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">运营</td>
      <td>
        <ul>
          <li>添加</li>
          <li>计数</li>
          <li>删除</li>
          <li>编辑</li>
          <li>GET</li>
          <li>报告</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## 已删除资源

以下资源已从API版本22中删除。

### UserLocation (USRLOC)

此对象已被删除。

## 已修改的资源

已为API版本22修改以下资源。

### 访问级别(ACSLVL)

AccessLevel对象与用户相关联，并描述确定用户可以访问的AccessLevelPermissions集。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>以下字段已修改，并更改了可能的值。 有关详细信息，请参阅开发人员文档。
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
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
      <td>以下字段已修改，并更改了可能的值。 有关详细信息，请参阅开发人员文档。
        <ul>
          <li><b>coreAction</b></li>
          <li><b>禁止操作</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>以下字段已修改，并更改了可能的值。 有关详细信息，请参阅开发人员文档。
        <ul>
          <li><b>操作</b></li>
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
      <td>以下字段已修改，并更改了可能的值。 有关详细信息，请参阅开发人员文档。
        <ul>
          <li><b>coreAction</b></li>
          <li><b>禁止操作</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>添加了以下字段。
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 公司(CPY)

Company对象表示由人员集合组成的组织。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmProjectID</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

CustomEnum对象有助于将状态代码转换为人类可读的文本。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>已添加
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">查询</td>
      <td>已添加
        <ul>
          <li><p><b>assignmentStatures</b></p></li>
          <li><p><b>bookingStatures</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### 客户（客户）

Customer对象表示一个使用Workfront实例的组织。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>以下字段已修改。
        <ul>
          <li>
            <p><b>customEnumType</b>
            </p>
            <p>添加了以下可能值。</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> （预订状态）</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> （分配状态）</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>添加了以下字段以支持企业存储管理。
         <ul>
         <li><b>islegacyCustomerEsmStorageEnabled</b></li>
         <li><b>islegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>以下字段已修改。
        <ul>
          <li>
            <p><b>customEnumType</b>
            </p>
            <p>添加了以下可能值以支持企业存储管理：</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### 文档(DOCU)

Document对象表示文件（如书面材料、图像或其他形式的信息）。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>已修改以下操作。
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>添加了以下字段以支持企业存储管理。
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>对象ID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### 文档文件夹(DOCFDR)

可以将文档组织到文件夹中。 您可以在个人文档区域中创建个人文件夹。 DocumentFolder对象表示这些文件夹之一。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      以下字段已修改。
        <ul>
          <li><b>version</b><p>删除了验证器“必需”。</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>添加了以下操作。
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">运营</td>
      <td>已添加以下操作。
        <ul>
          <li><p><b>编辑</b></p>
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
      <td>添加了以下字段。
        <ul>
          <li><b>项目组合ID</b></li>
          <li><b>programID
          </b></li>
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
      <td>以下字段已修改。
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>添加了以下可能值。</p>
             <ul>
              <li>
                <p><code>PFM</code>（移动文件夹）</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>标志</b>
            </p>
            <p>添加了以下可能值。</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### 日志字段(JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>以下字段已修改。
        <ul>
          <li>
            <p><b>操作</b>
            </p>
            <p>添加了以下可能值。</p>
             <ul>
              <li>
                <p><code>PFM</code>（移动文件夹）</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### Op任务(OPTASK)

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li><b>实际所需工作</b><p>添加了以下标志：
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">搜索字段</td>
      <td>
        <ul>
          <li><b>实际工作</b><p>类型从<code>null</code>更改为<code>double</code>。</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">运营</td>
      <td>添加了以下操作。
        <ul>
          <li><p><b>计数</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>报告</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>添加了以下字段。
        <ul>
          <li><b>enteredById</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### 参数组(PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段。
        <ul>
          <li><b>enteredById</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

PortalSection对象是报表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段。
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>添加了以下字段。
        <ul>
          <li><b>reportShareableFolder</b></li>
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
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnable</b></li>
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
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnable</b></li>
        </ul>
      以下字段已修改。
        <ul>
          <li><b>项目组合ID</b><p>添加了验证器“REQUIRED”。</li>
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
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnable</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

QueueDef对象表示Workfront中的请求队列定义。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>以下字段已修改，并更改了可能的值。 有关详细信息，请参阅开发人员文档。
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 计划报告(SCHREP)

ScheduledReport对象表示已配置为计划提交的报表。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>以下字段已修改，并对可能值进行了大量更改。 有关详细信息，请参阅开发人员文档。
        <ul>
          <li><b>格式</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 任务（任务）

Task对象表示作为实现最终目标（完成项目）的一部分而必须完成的工作项。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>已添加</p></li>
          <li><p><b>实际所需工作</b></p><p>已添加标志<code>AUTO_LOAD</code>和<code>DYNAMIC</code>。</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>已添加</p>
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
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持企业存储管理。
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>以下字段已修改。
        <ul>
          <li>
            <p><b>操作</b>
            </p>
            <p>添加了以下可能值。</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段。
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>已删除以下字段。
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





