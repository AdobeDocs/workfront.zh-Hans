---
content-type: api
navigation-topic: api-navigation-topic
title: API版本18中的新增功能
description: Adobe Workfront于2022年4月6日发布了API版本18。 API版本18具有对版本15的以下更改。
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# API版本18中的新增功能

Adobe Workfront于2024年4月8日发布了API版本18。 API版本18具有对版本15的以下更改。

## 已添加资源

没有为API版本18添加资源。

## 已删除资源

没有为API版本18删除资源

## 已修改的资源

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
            <p><b>coreAction</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
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
            <p><b>操作</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
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
            <p><b>coreAction</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
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
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 等待批准(AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">运营</td>
      <td>
        <ul>
          <li>
            <p>添加了以下操作：
            </p>
            <ul>
              <li>
                <p><b>添加</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 基线(BLIN)

基线是给定时刻项目性能的快照。 它们存储有关项目的关键信息，如关键日期、进度、成本和收入值。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 基线任务(BSTSK)

基线是给定时刻项目性能的快照。 它们存储有关项目的关键信息，如关键日期、进度、成本和收入值。 创建基线时，也会在该基线的基线任务中捕获任务信息。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
            <p><b>catObjCode</b>：
            </p>
            <p>添加了以下可能值：
            <ul>
              <li>
                <p><code>NLBRCY</code> （非人工资源类别）
                </p>
              </li>
              <li>
                <p><code>HOUR</code> （小时）
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> （费率卡）
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>：
            </p>
            <p>添加了以下可能值：
            <ul>
              <li>
                <p><code>NLBRCY</code> （非人工资源类别）
                </p>
              </li>
              <li>
                <p><code>HOUR</code> （小时）
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> （费率卡）
                </p>
              </li>
             </ul>
             </p>
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
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>：
            </p>
            <p>添加了以下参数：
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>：
            </p>
            <p>已添加。 此新操作会采用以下参数：
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 财务数据(FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">默认字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
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
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.open)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decisions.maked)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
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
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>：
            </p>
            <p>添加了以下字段：
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>：
            </p>
            <p>添加了以下字段：
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
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
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>已添加。
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

QueueDef对象表示队列，这是一个已发布到技术支持区域以允许用户向其提交问题的项目。

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
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> （查看成本率）</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> （查看记帐费率）</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> （查看一般财务）</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> （编辑成本率）</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> （编辑记帐费率）</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> （编辑一般财务）</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 比率（比率）

Rate对象表示Workfront中的记帐费率。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>添加了以下标志：
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>动态
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>显示名称</b></p><p>已添加。</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>显示名称</b>
            </p><p>已添加。</p>
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
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>添加了以下字段：
             <ul><li><code>copyCategories</code></li></ul>
            </p>
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
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

TemplateTask对象表示属于Template一部分的Task。 模板任务将成为使用模板的项目中的任务。<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole（团队）

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 时间表(TSHET)

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

<table>
  <tbody>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p>删除了以下字段：
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
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
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>已添加。</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

UserPrefValue对象表示用户首选项。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>值</b>
            </p>
            <p>已添加验证器 <code>MAX_LENGTH</code></p>
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
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>添加了以下字段：
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

