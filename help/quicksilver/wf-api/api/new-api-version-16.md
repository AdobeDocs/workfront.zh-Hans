---
content-type: api
navigation-topic: api-navigation-topic
title: API版本16的新增功能
description: Adobe Workfront于2022年4月6日发布了API版本16。 API版本16具有与版本15相比的以下更改。
author: Becky
feature: Workfront API
source-git-commit: 19978aaa2886008afc3c0faa9cfd18bd7c4b2555
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# API版本16的新增功能

Adobe Workfront于2022年4月6日发布了API版本16。 API版本16具有与版本15相比的以下更改。

## 添加了资源

未为API版本16添加任何资源。

## 删除的资源

未删除API版本16的资源

## 修改的资源

* <!--[AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [批准（批准）](#approval-approval)
* [客户首选项(CUSTPR)](#customerpreferences-custpr)
* [ExternalSection(EXTSEC)](#externalsection-extsec)
* [小时（小时）](#hour-hour)
* [布局模板(UITMPL)](#layouttemplate-uitmpl)
* [附注（附注）](#note-note)
* [OpTask /问题(OPTASK)](#note-note)
* [项目(PROJ)](#project-proj)
* [比率（比率）](#rate-rate)
* [富文本注释(RHNOTE)](#richtextnote-rhnote)
* [角色/作业角色（角色）](#role--job-role-role)
* [任务（任务）](#task-task)
* [工时单(TSHET)](#timesheet-tshet)
* [UIFilter /过滤器(UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping(UIGB)](#uigroupby--grouping-uigb)
* [UIView /视图(UIVW)](#uiview--view-uivw)
* [用户（用户）](#user-user)
* [UserNote(USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示您每天需要完成的工作分钟数。 它具有格式 <code>YYYY-MM-DD: (number of minutes)</code>、和会考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 分配(ASSGN)

分配对象表示工作项与被分配用于处理该工作项的用户、团队或组之间的连接。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示您每天需要完成的工作分钟数。 它具有格式 <code>YYYY-MM-DD: (number of minutes)</code>、和会考虑时区。</p>
          </li>
          <li>
            <p><b>具有轮廓</b>
            </p>
            <p>此字段已添加，且是一个布尔值，用于反映分配是否处于轮廓状态。 如果在负载平衡器中编辑了分配的每日分钟数，则分配已被处理。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum(CSTEM)

CustomEnum对象有助于将状态代码转换为人类可读的文本。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>此操作会返回一个布尔值，用于描述客户是否禁用了自动升级贡献者许可证持有者的选项。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection(EXTSEC)

ExternalSection对象是嵌入在Workfront报表中的外部网页。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>添加了该变量，并计算在报表中嵌入的iFrame的URL。</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>添加了该变量，并计算在报表中嵌入的iFrame的URL。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 小时（小时）

Hour对象表示用户在时间表上记录的一小时。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>timeskeHourIdentifier</b>
            </p>
            <p>已添加. 此参数用于标识使用 <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### 附注（附注）

Note对象是对Workfront对象进行的注释或更新。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>添加了此字段，表示附加到评论的文档列表。</p>
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
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示您每天需要完成的工作分钟数。 它具有格式 <code>YYYY-MM-DD: (number of minutes)</code>、和会考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>此操作会添加字段 <code>teamIDs</code> 支持为任务或问题分配多个团队的功能。</p>
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
            <p>添加了此字段，它表示项目上所有预算小时数的总和。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 比率（比率）

Rate对象表示Workfront中的计费费率。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>这些参数已从角色对象移到Rate对象，以便角色对象和用户对象可以具有多个值（对于不同的日期范围）。</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>这些参数表示Rate附加到的对象的ID和对象代码。
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>此操作已添加，并将Rate对象附加到给定对象。 此端点适用于所有可附加速率的对象。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 富文本注释(RHNOTE)

RichTextNote对象是对Workfront对象进行的注释或更新，该对象包含富文本，如粗体或斜体文本。

RichTextNote对象删除了标记 `REPORTABLE`.

### 角色/作业角色（角色）

角色对象（作业角色）表示用户可能填充的功能能力或技能集，如设计人员或产品经理。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
           <li>
            <p><b>费率</b>
            </p>
            <p>添加了，表示附加到此角色的Rate对象。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 任务（任务）

任务对象表示一个工作项，必须将该工作项作为实现最终目标（完成项目）的步骤来执行。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示您每天需要完成的工作分钟数。 它具有格式 <code>YYYY-MM-DD: (number of minutes)</code>、和会考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>此操作会添加字段 <code>teamIDs</code> 支持为任务或问题分配多个团队的功能。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 工时单(TSHET)

时间表对象表示一个虚拟工时记录卡，它允许用户输入为任务、项目和间接费用小时类型工作的实际小时数。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>此参数删除了标记 <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>此参数删除了标记 <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>此参数已添加，并以天为单位存储工时单持续时间，而不考虑对“完整Workday的等效小时数”的更改。  例如，如果“等效小时数”设置为6，并记录了一天，则“等效小时数”将更改为8小时， <code>totalDays</code> 仍具有值1。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter /过滤器(UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>添加了此操作，并获取过滤器查询映射并添加 <code>allowingnull</code> 可为null字段连接。</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>这些操作支持在全系统内共享过滤器、视图和分组的功能。</p><p>有关更多信息，请参阅 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">使过滤器、视图或分组对所有用户可用</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping(UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>这些操作支持在全系统内共享过滤器、视图和分组的功能。</p><p>有关更多信息，请参阅 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">使过滤器、视图或分组对所有用户可用</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView /视图(UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>这些操作支持在全系统内共享过滤器、视图和分组的功能。</p><p>有关更多信息，请参阅 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">使过滤器、视图或分组对所有用户可用</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 用户（用户）

User对象表示在Workfront中具有可登录并与系统交互的帐户的人员。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
           <li>
            <p><b>费率</b>
            </p>
            <p>添加了，表示附加到此用户的Rate对象。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote(USRNOT)

UserNote对象是通知。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">查询</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>添加了以下可能值：
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 工作（工作）

Work对象是Task和OpTask都可继承的通用接口，并在二者之间共享通用代码。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示您每天需要完成的工作分钟数。 它具有格式 <code>YYYY-MM-DD: (number of minutes)</code>、和会考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
