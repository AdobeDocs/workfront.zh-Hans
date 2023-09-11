---
content-type: api
navigation-topic: api-navigation-topic
title: API版本16中的新增功能
description: Adobe Workfront于2022年4月6日发布了API版本16。 API版本16具有对版本15的以下更改。
author: Becky
feature: Workfront API
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 8afbb1f45331d79bb849afb3acf3e9ff054cefc3
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# API版本16中的新增功能

Adobe Workfront于2023年4月6日发布了API版本16。 API版本16具有对版本15的以下更改。

## 已添加资源

没有为API版本16添加资源。

## 已删除资源

没有为API版本16删除资源

## 已修改的资源

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [批准(APPROVAL)](#approval-approval)
* [客户首选项(CUSTPR)](#customerpreferences-custpr)
* [外部节(EXTSEC)](#externalsection-extsec)
* [Hour (HOUR)](#hour-hour)
* [布局模板(UITMPL)](#layouttemplate-uitmpl)
* [附注（附注）](#note-note)
* [Op任务/问题(OPTASK)](#note-note)
* [项目（项目）](#project-proj)
* [比率（比率）](#rate-rate)
* [RichTextNote(RHNOTE)](#richtextnote-rhnote)
* [角色/工作角色(ROLE)](#role--job-role-role)
* [任务（任务）](#task-task)
* [时间表(TSHET)](#timesheet-tshet)
* [UIFilter/过滤器(UIFT)](#uifilter--filter-uift)
* [UIGB/分组(UIGB)](#uigroupby--grouping-uigb)
* [用户视图/视图(UIVW)](#uiview--view-uivw)
* [用户（用户）](#user-user)
* [用户注释(USRNOT)](#usernote-usrnot)

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
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示每天您需要完成的工作分钟数。 其格式为 <code>YYYY-MM-DD: (number of minutes)</code>，并考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 分配(ASSGN)

任务对象表示工作项与分配给该工作项的用户、团队或组之间的连接。

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
            <p>此字段已添加，并显示每天您需要完成的工作分钟数。 其格式为 <code>YYYY-MM-DD: (number of minutes)</code>，并考虑时区。</p>
          </li>
          <li>
            <p><b>isContured</b>
            </p>
            <p>此字段已添加，并且是一个布尔值，可反映是否对分配进行轮廓化。 如果在工作负载均衡器中编辑了分配的每日分钟数，则已配置分配。</p>
          </li>
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
            <p>此操作返回一个布尔值，描述客户是否已禁用自动升级参与者许可证持有者的选项。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 外部节(EXTSEC)

ExternalSection对象是嵌入到Workfront报表中的外部网页。

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
            <p>添加此参数，并计算报表中嵌入的iFrame的URL。</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>添加了此URL，并计算报表中嵌入的iFrame的URL。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Hour (HOUR)

Hour对象表示用户在时间表上记录的小时。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>timesheethouridentifier</b>
            </p>
            <p>已添加. 此参数用于标识创建的小时数 <code>batchSave</code>. </p>
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

Note对象是对Workfront对象所做的注释或更新。

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
            <p>此字段已添加，表示附加到评论的文档列表。</p>
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
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>此字段已添加，并显示每天您需要完成的工作分钟数。 其格式为 <code>YYYY-MM-DD: (number of minutes)</code>，并考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
           <li>
            <p><b>assignmultiple</b>
            </p>
            <p>此操作已添加字段 <code>teamIDs</code> 支持将多个团队分配给一个任务或问题的功能。</p>
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
            <p>已添加此字段，它表示项目中所有预算小时数的总和。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### 比率（比率）

Rate对象表示Workfront中的记帐费率。

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
           <p>这些参数已从Role对象移至Rate对象，以便Role和User对象可以有多个值（对于单独的日期范围）。</p>
          </li>
          <li><p><b>对象ID</b></p><p><b>对象代码</b></p>
          <p>这些参数表示与费率关联的对象的ID和目标代码。
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
           <p>已添加此操作，并将Rate对象附加到给定Object。 此端点适用于所有速率可附加对象。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote(RHNOTE)

RichTextNote对象是对Workfront对象所做的注释或更新，包括富文本，例如粗体或斜体文本。

RichTextNote对象删除了标志 `REPORTABLE`.

### 角色/工作角色(ROLE)

角色对象（工作角色）表示用户可能填充的功能能力或技能集，如设计人员或产品经理。

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
            <p>该角色已添加，表示附加到此角色的Rate对象。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 任务（任务）

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

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
            <p>此字段已添加，并显示每天您需要完成的工作分钟数。 其格式为 <code>YYYY-MM-DD: (number of minutes)</code>，并考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
           <li>
            <p><b>assignmultiple</b>
            </p>
            <p>此操作已添加字段 <code>teamIDs</code> 支持将多个团队分配给一个任务或问题的功能。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>availableactions</b>
            </p>
            <p>此参数删除了标记 <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>可编辑</b>
            </p>
            <p>此参数删除了标记 <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>添加了此参数，并且不论对“完整Workday的等效小时数”有何更改，都以天为单位存储时间表持续时间。  例如，如果等效小时数设置为6，并记录一天，则等效小时数将更改为8小时， <code>totalDays</code> 仍具有值1。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter/过滤器(UIFT)



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
            <p>此操作已添加，它采用过滤器查询映射并添加 <code>allowingnull</code> 为空字段加入。</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>这些操作支持在系统范围内共享筛选器、视图和分组的功能。</p><p>有关更多信息，请参阅 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">使过滤器、视图或分组对所有用户可用</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGB/分组(UIGB)


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
            <p>这些操作支持在系统范围内共享筛选器、视图和分组的功能。</p><p>有关更多信息，请参阅 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">使过滤器、视图或分组对所有用户可用</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### 用户视图/视图(UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>布局类型</b>
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
            <p>这些操作支持在系统范围内共享筛选器、视图和分组的功能。</p><p>有关更多信息，请参阅 <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">使过滤器、视图或分组对所有用户可用</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 用户（用户）

User对象表示在Workfront中拥有帐户的人员，该帐户可以登录并与系统交互。

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
            <p>此内容已添加，它表示附加到此用户的Rate对象。</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### 用户注释(USRNOT)

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

Work对象是Task和OpTask都继承的公用接口，它们共享公用代码。

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
            <p>此字段已添加，并显示每天您需要完成的工作分钟数。 其格式为 <code>YYYY-MM-DD: (number of minutes)</code>，并考虑时区。</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
