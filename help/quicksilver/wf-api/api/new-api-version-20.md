---
content-type: api
navigation-topic: api-navigation-topic
title: API版本20中的新增功能
description: Adobe Workfront于2022年4月6日发布了API版本20。 API版本20具有对版本19的以下更改。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# API版本20中的新增功能

Adobe Workfront于2025年5月4日发布了API版本20。 API版本20具有对版本19的以下更改。

## 已添加资源

没有为API版本20添加资源。

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## 已删除资源

没有为API版本20删除资源

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
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 公告附件(ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>文件扩展名</b>
            </p>
             <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>实际收益</li>
              <li>actualBillableExpenseCost</li>
              <li>实际成本</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>实际收入</li>
              <li>actualRiskCost</li>
              <li>实际值</li>
              <li>billedRevenue</li>
              <li>预算</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>预算劳力成本</li>
              <li>costAmou</li>
              <li>costType</li>
              <li>固定成本</li>
              <li>fixedrevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>计划成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>计划值</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingriscost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>风险绩效指数</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>实际成本</li>
          <li>实际收入</li>
          <li>计划成本</li>
          <li>plannedVenue</li>
          </ul>
          </li>
          <li><p><b>planneduration</b></p> <p>已添加标志<code>DYNAMIC</code>、<code>LAZY_READ</code>和 <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>添加了标志 <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>已添加可能的值<code>URH</code>（每小时用户和角色） </li>
          <li><p><b>revenualtype</b></p> <p>添加了可能的值<code>URH</code>（每小时用户和角色）、<code>URC</code>（每小时用户和角色包含上限）和<code>URF</code>（每小时用户和角色加固定）</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
          <p>添加了以下字段：</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### 分配(ASSGN)

Assignment对象表示工作项与分派处理该工作项的用户、团队或组之间的连接。

Assignment对象添加了标志`ATTRIBUTE_ATTACHABLE`和`DOMAIN_EXTENDABLE`。


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### 头像

头像对象是用户照片。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>已添加</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>已添加</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">运营</td>
      <td>
        <ul>
          <li>
            <p><b>副本</b>
            </p>
             <p>已添加</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>实际成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>预算</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>计划成本</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>实际成本</li>
          <li>计划成本</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>添加了标志 <code>CURRENCY</code></li>
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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>实际成本</li>
              <li>actualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>计划成本</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>实际成本</li>
          <li>计划成本</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>添加了标志 <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 记帐记录(BILL)

BillingRecord对象记录可记帐的收入、小时数或费用。 此信息可用于在外部会计系统中创建发票。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>数量</li>
              <li>其他金额</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>已添加</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b>配置</b>
            </p>
             <p>已添加</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 公司(CPY)

Company对象表示由人员集合组成的组织。

公司对象添加了标志`SHARABLE`。

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
             <p>添加了以下可能值：</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissuemove)</p></li>
            </ul>
          </li>
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
      <td>
           <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>费率</li>
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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLaborCost</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>固定成本</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedVenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

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
            <p><b>货币</b>
            </p>
             <p>已添加</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>实际成本</li>
              <li>resourceRe收入</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
              <li>实际成本</li>
              <li>resourceRe收入</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>已添加</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### Op任务(OPTASK)

OpTask对象通常称为“问题”。 问题是一个工作项，它通常表示存在阻止任务或项目完成的问题。 问题也可以是技术支持请求。 变更单、请求和错误也是问题。

OpTask对象添加了标志DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>实际成本</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
              <li>实际成本</li>
          </ul>
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
        <ul>
          <li>
            <p><b>显示类型</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>INTRNL</code> （内部查找）</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> （多选内部查找）</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio（端口）

Portfolio对象是争夺相同资源（通常是资金或人员来完成这些资源）的项目集合。

Portfolio对象添加了标志`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>已对齐</li>
              <li>预算</li>
              <li>货币</li>
              <li>净值</li>
              <li>预算</li>
              <li>onTime</li>
              <li>项目组合净值</li>
              <li>项目组合Roi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### 计划(PRGM)

项目群对象是项目组合中项目的子集，其中类似的项目可以分组在一起。

程序对象添加了标志`DOMAIN_EXTENDABLE`。

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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>实际收益</li>
              <li>actualBillableExpenseCost</li>
              <li>实际成本</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>实际收入</li>
              <li>actualRiskCost</li>
              <li>实际值</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billedRevenue</li>
              <li>预算</li>
              <li>budgetedCost</li>
              <li>budgetedHours</li>
              <li>预算劳力成本</li>
              <li>eac</li>
              <li>固定成本</li>
              <li>fixedrevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>计划成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedVenue</li>
              <li>plannedRiskCost</li>
              <li>计划值</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingriscost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>风险绩效指数</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>实际成本</li>
          <li>实际收入</li>
          <li>计划成本</li>
          <li>plannedVenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>添加了标志 <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> （从自定义数据中删除）</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> （添加子项目）</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 比率（比率）

Rate对象表示Workfront中的记帐费率。

Rate对象添加了标志`ATTRIBUTE_ATTACHABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rate值</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rate值</li>
          </ul>
          </li>
         <li>
          <p>添加了以下字段：
          <ul>
          <li>货币</li>
          <li>已锁定</li>
          <li>类型</li>
          <li>值</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 角色(ROLE)

角色对象（工作角色）表示用户可能填充的功能能力或技能集，如Designer或产品经理。

Role对象添加了标志`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
        <ul>
          <li>
          <p>添加了以下字段：
          <ul>
          <li>billingRates</li>
          <li>costRates</li>
          </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>格式</b>
            </p>
             <p>添加了以下可能值：</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 记分卡问题(SCOREQ)

ScoreCardQuestion对象表示已添加到记分卡的问题。 这些问题通常由Portfolio经理决定，这些问题的答案让经理能够了解项目与项目组合目标的对齐情况。

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
             <p>添加了以下可能值：</p>
             <ul>
              <li><p><code>INTRNL</code> （内部查找）</p></li>
              <li><p><code>MULTINTRNL</code> （多选内部查找）</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 任务（任务）

Task对象表示作为实现最终目标（完成项目）的步骤而必须执行的工作项。

Task对象添加了标志`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>实际成本</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>实际收入</li>
              <li>costAmou</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedVenue</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>实际成本</li>
          <li>实际收入</li>
          <li>计划成本</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>添加了以下可能值：<ul><li><code>URH</code> （用户和角色每小时）</li></ul></li>
          <li><p><b>revenualtype</b></p> <p>添加了以下可能值：<ul><li><code>URH</code> （用户和角色每小时）</li><li><code>URC</code> （受限的用户和角色小时）</li><li><code>URF</code> （用户和角色每小时加固定）</li></ul></li>
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
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>预算</li>
              <li>固定成本</li>
              <li>fixedrevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>计划成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedVenue</li>
              <li>plannedRiskCost</li>
              <li>所需工作</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>计划成本</li>
          <li>plannedVenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
          <p>添加了以下字段：</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask (TTSK)

TemplateTask对象表示属于Template一部分的Task。 模板任务将成为使用模板的项目中的任务。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>billingamount</li>
              <li>costAmou</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedVenue</li>
              <li>revenualtype</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>计划成本</li>
          <li>plannedVenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>添加了以下可能值：<ul><li><code>URH</code> （用户和角色每小时）</li></ul></li>
          <li><p><b>revenualtype</b></p> <p>添加了以下可能值：<ul><li><code>URH</code> （用户和角色每小时）</li><li><code>URC</code> （受限的用户和角色小时）</li><li><code>URF</code> （用户和角色每小时加固定）</li></ul></li>
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
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>已移除</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 用户（用户）

User对象表示在Workfront中拥有帐户的人员，该帐户可以登录并与系统交互。

用户对象添加了字段`ATTRIBUTE_ATTACHABLE`和`DOMAIN_EXTENDABLE`。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>
          <p>添加了以下字段：</p>
             <ul>
              <li><b>billingRates</b></li>
              <li><b>costRates</b></li>
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
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p>以下字段添加了标志<code>RESTRICTABLE</code>：
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>实际成本</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>实际收入</li>
              <li>costAmou</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>计划成本</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedVenue</li>
            </ul>
          </li>
          <li>
          <p>以下字段将其类型从<code>double</code>更改为<code>class java.math.BigDecimal</code>：
          <ul>
          <li>实际成本</li>
          <li>实际收入</li>
          <li>计划成本</li>
          <li>plannedVenue</li>
          </ul>
          </li>
          <li><p><b>planneduration</b></p> <p>已添加标志<code>DYNAMIC</code>、<code>LAZY_READ</code>和 <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>添加了标志 <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>已添加可能的值<code>URH</code>（每小时用户和角色） </li>
          <li><p><b>revenualtype</b></p> <p>添加了可能的值<code>URH</code>（每小时用户和角色）、<code>URC</code>（每小时用户和角色包含上限）和<code>URF</code>（每小时用户和角色加固定）</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



