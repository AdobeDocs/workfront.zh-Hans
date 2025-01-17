---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect数据字典
description: 本页包含有关Workfront Data Connect中数据的结构和内容的信息。
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '4609'
ht-degree: 4%

---

# Workfront Data Connect数据字典

本页包含有关Workfront Data Connect中数据的结构和内容的信息。

>[!NOTE]
>
>Data Connect中的数据每四小时刷新一次，因此最近的更改可能不会立即反映出来。

## 表类型

您可以在Data Connect中使用多种表类型，以最深入地了解的方式查看Workfront数据。

* **当前表**

  当前表反映的数据与Workfront中的数据、每个对象及其当前状态类似。 但是，与Workfront相比，它可以以低得多的延迟进行导航。

* **事件表**

  “事件”表格将跟踪Workfront中的每个更改记录：即，每次对象更改状态时，都将创建一个记录以显示更改的时间、进行更改的人员以及更改的内容。 因此，此表对于时间点比较很有用。 此表仅包括过去三年的记录。

* **每日历史记录表**

  “每日历史记录”表提供了“事件”表的缩写版本，它以每日为基础显示每个对象的状态，而不是显示每个单独事件发生时的状态。 因此，此表可用于趋势分析。

<!-- Custom table -->

## 实体关系图

Workfront中的对象（因此也就是Data Connect数据湖中的对象）不仅由其各个值定义，而且由其与其他对象的关系定义。 下面的实体关系图提供了数据连接中对象关系的高级映射。 可以使用以下链接查看和下载图表：

[Data Connect实体关系图](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>实体关系图是正在进行的工作 — 因此，它仅供参考，并且可能会发生更改。

## 日期类型

有许多日期对象提供有关特定事件发生时间的信息。

* `DL_LOAD_TIMESTAMP`：此日期用于内部引用，并反映数据加载到Current、Event或Daily History表中的时间。 此日期不应用于数据分析，计划在Workfront数据湖的测试阶段删除。
* `CALENDAR_DATE`：此日期仅存在于“每日历史记录”表中。 此表记录了`CALENDAR_DATE`中指定的每个日期在11:59 UTC时的数据外观。
* `BEGIN_EFFECTIVE_TIMESTAMP`：此日期同时存在于“事件”和“每日历史记录”表中，并且记录记录记录何时将&#x200B;_更改为_&#x200B;其在当前行中的值。
* `END_EFFECTIVE_TIMESTAMP`：此日期同时存在于“事件”和“每日历史记录”表中，记录某记录何时将&#x200B;_从_&#x200B;当前行中的值更改为其他行中的值。 为了在`BEGIN_EFFECTIVE_TIMESTAMP`和`END_EFFECTIVE_TIMESTAMP`上的查询之间允许，此值从不为null，即使没有新值也是如此。 如果记录仍然有效（即值未更改），`END_EFFECTIVE_TIMESTAMP`的值将为2300-01-01。

## 术语表

下表将Workfront中的对象名称（以及它们在接口和API中的名称）与它们在Data Connect中的等效名称相关联。

<table>
  <thead>
    <tr>
        <th>Workfront实体名称</th>
        <th>界面引用</th>
        <th>API参考 | 标签</th>
        <th>数据湖表</th>
        <th>关系字段</th>
        <th>关系表和字段</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>访问级别</td>
        <td>访问级别</td>
        <td>ACSLVL | 访问级别</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>不是关系；用于内部申请<br>USER_CURRENT | USERID<br>不是关系；用于内部应用目的<br>在OBJCODE字段中标识的对象的ID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>访问规则</td>
        <td>共享</td>
        <td>ACSRUL | 共享</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (self) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>ACCESSOROBJCODE字段<br>Self<br>在ANCESTOROBJCODE字段中标识的对象的ID<br>USERS_CURRENT | USERID<br>在SECURITYOBJCODE字段中标识的对象的ID<br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>批准路径</td>
        <td>批准路径</td>
        <td>ARVPTH | 批准</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID （自身） <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>Self<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>审批流程</td>
        <td>审批流程</td>
        <td>ARVPRC | 批准流程</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY<br>APPROVALPROCESSES_EVENT</td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>自助<br>用户_当前 | USERID<br>用户_当前 | USERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>审批步骤</td>
        <td>审批步骤</td>
        <td>ARVSTP | 审批阶段</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID （自身） <br>SYSID</td>
        <td>APPROVALPATH_CURRENT | APPROVALPATHID<br>Self<br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>ApproverStatus</td>
        <td>审批者状态</td>
        <td>ARVSTS | ApproverStatus</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY<br>APPROVERSTATUSES_EVENT</td>
        <td>APPROVERSTATUSID （自身）<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>在APPROVABLEOBJCODE字段中标识的对象的ID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USERS_CURRENT | 用户ID <br>用户_当前 | 用户ID<br>用户_当前 | 用户ID <br>OPTASKS_CURRENT | OPTASKID<br>用户_当前 | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用程序目的<br>TASKS_CURRENT | TASKID<br>用户_当前 | 用户ID</td>
    </tr>
    <tr>
        <td>任务分配</td>
        <td>任务分配</td>
        <td>分配 | 指定任务</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID （自身）<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | 用户ID<br>自身<br>类别_当前 | CATEGORYID<br>当前不支持分类器表<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | 角色ID<br>任务_当前 | TASKID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>等待审批</td>
        <td>等待审批</td>
        <td>AWAPVL | 等待审批</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID （自身） <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>当前不支持访问请求表<br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | USERID<br>Self<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>项目_当前 | PROJECTID<br>ROLES_CURRENT | 角色ID<br>用户_当前 | USERID<br>不是关系；用于内部应用程序目的<br>TASKS_CURRENT | TASKID<br>团队_当前 | TEAMID<br>时间表_当前 | 时间表ID<br>用户_当前 | 用户ID</td>
    </tr>
    <tr>
        <td>基线</td>
        <td>基线</td>
        <td>BLIN | 基线</td>
        <td>BASELINES_CURRENT<br>BASELINES_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>基线任务</td>
        <td>基线任务</td>
        <td>BSTSK | 基线任务</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>基线_当前 | BASELINEID<br>Self<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>不是关系；用于内部应用目的<br>TASKS_CURRENT | TASKID</td>
    </tr>
    <tr>
        <td>记帐费率</td>
        <td>费率或覆盖率</td>
        <td>费率 | 记帐费率</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (SELF)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNATIONS_CURRENT | ASSIGNMENTID<br>当前不支持分类器表<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>当前不支持非人工资源类别表<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>OBJCODE字段<br>PROJECTS_CURRENT中标识的对象的ID | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>自助<br>角色_当前 | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>不是关系；用于内部应用程序目的<br>TEMPLATES_CURRNT | TEMPLATEID<br>USERS_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>账单记录</td>
        <td>账单记录</td>
        <td>帐单 | 开票记录</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>自助<br>类别_当前 | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>当前不支持发票表<br>USERS_CURRENT | 用户ID <br>PROJECTS_CURRENT | PROJECTID   <br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>预订</td>
        <td>预订</td>
        <td>预订 | 预订</td>
        <td>BOOKINGS_CURRENT<br>BOOKINGS_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (SELF)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>自助<br>用户_当前 | USERID<br>用户_当前 | USERID<br>当前不支持非人工资源类别表<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>在OBJOBJCODE字段中标识的对象的ID<br>PROJECTS_CURRENT | PROJECTID <br>不是关系；用于内部应用程序目的<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE字段中标识的对象的ID</td>
    </tr>
    <tr>
        <td>企业轮廓</td>
        <td>企业轮廓</td>
        <td>BSNPRF | 业务配置文件</td>
        <td>BUSINESSPROFILE_CURRENT<br>BUSINESSPROFILE_DAILY_HISTORY<br>BUSINESSPROFILE_EVENT</td>
        <td>ACCESSLEVELID<br>BUSINESSPROFILEID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>ACCESSLEVELS_CURRENT | ACCESSLEVELID<br>自身<br>用户_当前 | USERID<br>组_当前 | GROUPID<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>业务规则</td>
        <td>业务规则</td>
        <td>BSNRUL | 业务规则</td>
        <td>BUSINESSRULE_CURRENT<br>BUSINESSRULE_DAILY_HISTORY<br>BUSINESSRULE_EVENT</td>
        <td>BUSINESSRULEID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>自助<br>用户_当前 | USERID<br>用户_当前 | USERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>类别</td>
        <td>自定义表单</td>
        <td>CTGY | 类别</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>SYSID</td>
        <td>自助<br>用户_当前 | USERID<br>组_当前 | GROUPID<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>类别参数</td>
        <td>自定义表单字段</td>
        <td>CTGYPA | 类别参数</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID<br>SYSID</td>
        <td>自助<br>类别_当前 | 当前不支持CATEGORYID<br>参数组表<br>PARAMETERS_CURRENT | 参数    <br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>分类器</td>
        <td>位置</td>
        <td>CLSF | 位置</td>
        <td>CLASSIFIER_CURRENT<br>CLASSIFIER_DAILY_HISTORY<br>CLASSIFIER_EVENT</td>
        <td>CLASSIFIERID (self)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>PARENTID<br>SYSID</td>
        <td>自助<br>用户_当前 | USERID<br>用户_当前 | USERID<br>CLASSIFIER_CURRENT | CLASSIFIERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>公司</td>
        <td>公司</td>
        <td>CMPY | 公司</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (self)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>自身<br>用户_当前 | 用户ID <br>组_当前 | GROUPID<br>USERS_CURRENT | 用户ID <br>RATECARD_CURRENT | RATECARDID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>自定义季度</td>
        <td>自定义季度</td>
        <td>CSTQRT | 自定义季度</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>CustomEnum</td>
        <td>条件、优先级、严重性、状态</td>
        <td>系统 | 自定义枚举</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>*记录类型通过“enumClass”属性进行标识。 以下是预期的类型：<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>STATUS_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>组当前 | GROUPID</td>
    </tr>
    <tr>
        <td>文档</td>
        <td>文档</td>
        <td>DOCU | 文档</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>ID releaseversionid<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>用户当前 | 当前不支持USERID<br>Self<br>文档请求表<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>变量取决于DOCOBJCODE值<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_当前 | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>当前不支持<br>TASK_CURRENT版本表 | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>变量取决于TOPOBJCODE值<br>USER_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>文档审批</td>
        <td>文档审批</td>
        <td>DOCAPL | 文档审批</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | 用户ID <br>自身<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>用户_当前 | USERID <br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>文档文件夹</td>
        <td>文档文件夹</td>
        <td>DOCFLD | 文档文件夹</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>用户ID</td>
        <td>自助<br>用户_当前 | USERID<br>OPTASKS_CURRENT | OPTASKID<br>迭代_当前 | ITERATIONID<br>LINKEDFOLDERS_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_当前 | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMID    <br>项目_当前 | PROJECTID <br>不是关系；用于内部应用目的<br>TASKS_CURRENT | TASKID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>用户_当前 | 用户ID</td>
    </tr>
    <tr>
        <td>DocumentProveMetadata</td>
        <td>文档提供元数据</td>
        <td>文档 | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID （自身） <br>SYSID</td>
        <td>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>Documentprovider</td>
        <td>文档提供者</td>
        <td>DOCPRO | 文档提供商</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID （自身）<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>Self<br>USERS_CURRENT | 用户ID    <br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>文档提供程序配置</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID （自身）<br>SYSID</td>
        <td>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>文档版本</td>
        <td>文档版本</td>
        <td>DOCV | 文档版本</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>Self<br>USER_CURRENT | 当前不支持USERID<br>外部ID<br>校对审批状态表<br>USER_CURRENT | 当前不支持USERID<br>校对表<br>USER_CURRENT | 当前不支持USERID<br>验证阶段表</td>
    </tr>
    <tr>
        <td>汇率</td>
        <td>汇率</td>
        <td>表达式 | 汇率</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID （自身）<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>自助<br>项目_当前 | PROJECTID <br>不是关系；用于内部应用目的<br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>费用</td>
        <td>费用</td>
        <td>展开 | 费用</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (self) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>类别_当前 | CATEGORYID<br>用户_当前 | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Self <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>对象代码字段<br>PROJECTS_CURRENT中标识的对象的ID | PROJECTID <br>不是关系；用于内部应用目的<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>TOPOBJCODE字段中标识的对象的ID</td>
    </tr>
    <tr>
        <td>费用类型</td>
        <td>费用类型</td>
        <td>EXPTYP | 费用类型</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>不是关系；用于内部应用程序目的<br>Self<br>在OBJCODE字段中标识的对象的ID <br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>组</td>
        <td>组</td>
        <td>组 | 组</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | 用户ID<br>类别_当前 | CATEGORYID<br>用户当前 | 不支持USERID<br>Self<br>布局模板表<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>小时</td>
        <td>小时</td>
        <td>HOUR | 小时</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>ID taskid<br>TIMESHEETID</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>类别_当前 | CATEGORYID<br>当前不支持分类器表<br>不是关系；用于内部应用程序目的<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>不是Workfront关系；用于与外部系统<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>不是关系；用于内部应用程序目的<br>ROLE_CURRENT | 角色ID<br>任务当前 | TASKID<br>工时表当前 | 时间表ID</td>
    </tr>
    <tr>
        <td>小时数类型</td>
        <td>小时数类型</td>
        <td>小时 | 小时类型</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>不是关系；用于内部申请<br>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>开发周期</td>
        <td>开发周期</td>
        <td>ITRN | 迭代</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (self)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>用户_当前 | 用户ID <br>自身<br>用户_当前 | 用户ID <br>用户_当前 | USERID <br>不是关系；用于内部应用程序目的<br>TEAMS_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>日志条目</td>
        <td>日志条目</td>
        <td>JRNLE | 日志条目</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (self)<br>OBJID<br>OPTASKID<br>ID portfolioid<br>PROGRAMID<br>PROJECTID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TIMESHEETID<br>TOPOBJID<br>USERID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>当前不支持<br>BASELINES_CURRENT的审核记录表 | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>公司_当前 | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>当前不支持文档共享表<br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>当前不支持Initiative表<br>Self<br>在OBJCODE字段中标识的对象的ID<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_当前 | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>在SUBOBJCODE字段中标识的对象的ID<br>当前不支持订阅表<br>不是关系；用于内部应用程序目的<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>TOPOBJCODE字段<br>USERS_CURRENT中标识的对象的ID | 用户ID</td>
    </tr>
    <tr>
        <td>链接文件夹</td>
        <td>链接文件夹</td>
        <td>LNKFDR | 链接文件夹</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY<br>LINKEDFOLDERS_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (self)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>外部ID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>里程碑</td>
        <td>里程碑</td>
        <td>英里 | 里程碑</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY<br>MILESTONES_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>Self<br>MILESTONEPATH_CURRENT | 里程碑ID</td>
    </tr>
    <tr>
        <td>里程碑路径</td>
        <td>里程碑路径</td>
        <td>MPATH | 里程碑路径</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>自身</td>
    </tr>
    <tr>
        <td>非人工资源</td>
        <td>非劳动力资源</td>
        <td>NLBR | 非人工资源</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (self)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID<br>SYSID  </td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>自身<br>用户_当前 | USERID<br>组_当前 | GROUPID<br>USERS_CURRENT | USERID<br>当前不支持非人工资源类别表<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>非劳动力资源类别</td>
        <td>非劳动力资源类别</td>
        <td>NLBRCY | 非人工资源类别</td>
        <td>NLBRCATEGORIES_CURRENT<br>NLBRCATEGORIES_DAILY_HISTORY<br>NLBRCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID （自身）<br>PRIVATERATECARDID<br>SCHEDULEID<br>SYSID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>用户_当前 | USERID<br>用户_当前 | USERID<br>Self<br>RATECARD_CURRENT | RATECARDID<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用目的</td>
    </tr>
    <tr>
        <td>非工作日</td>
        <td>计划例外</td>
        <td>非WKD | 非工作日</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>OBJCODE字段<br>SCHEDULES_CURRENT中标识的对象的ID | SCHEDULEID <br>不是关系；用于内部申请<br>USERS_CURRENT | 用户ID  </td>
    </tr>
    <tr>
        <td>注释</td>
        <td>注释</td>
        <td>注意 | 注意</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHHOPTASKID<br>ATTACHHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTANDORSEMENTID<br>IDID parentjournalentryid<br>PARENTNOTEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONID<br>PROOFID<br>RICHTEXTNOTEID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>THREADID<br>TIMESHEETID<br>TOPOBJID <br>用户ID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>变量，取决于ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | 当前不支持USERID<br>审核记录表<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>不是Workfront关系；用于与外部系统<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>变量，具体取决于NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | 当前不支持USERID<br>认可表<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_当前 | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>当前不支持校对操作表<br>当前不支持校对表<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>变量，取决于TOPOBJCODE<br>USER_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>对象集成</td>
        <td>对象集成</td>
        <td>对象 | 对象集成</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>在LINKEDOBJECTCODE字段<br>Self<br>中标识的对象的ID在OBJCODE字段<br>中标识的对象的ID不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>对象类别</td>
        <td>对象类别</td>
        <td>对象 | 对象类别</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>Self<br>在OBJCODE字段<br>中标识的对象的ID不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>Op 任务</td>
        <td>问题，请求</td>
        <td>OPTASK | 问题</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID RESOLVEOPTASKID<br>QUEUETOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br>SOURCETASKID<br>SUBMITTEDBYID<br>TEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | 用户ID<br>类别_当前 | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | 当前不支持ITERATIONID<br>Kanban展示板表<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>自身<br>用户当前 | USERID<br>PROJECT_CURRENT | PROJECTID<br>当前不支持队列定义表<br>当前不支持队列主题表<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>变量，取决于RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>变量，取决于SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>用户当前 | USERID<br>TEAM_CURRENT | TEAMID</td>
    </tr>
    <tr>
        <td>参数</td>
        <td>自定义字段</td>
        <td>参数 | 参数</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY<br>PARAMETERS_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID （自身）<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>参数筛选器表当前不支持<br>Self<br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>参数选项</td>
        <td>参数选项</td>
        <td>POPT | 参数选项</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID （自身） <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>自身<br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>门户部分</td>
        <td>报告</td>
        <td>PTLSEC | 报表</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID （自身）<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>不是关系；用于内部应用目的<br>USERS_CURRENT | USERID <br>UIFILTERS_CURRENT | 筛选<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | 用户ID <br>用户_当前 | USERID <br>在OBJOBCODE字段中标识的对象的ID<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | 用户ID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>当前不支持计划报告表<br>不是关系；用于内部应用程序目的<br>UIVIEWS_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>门户选项卡</td>
        <td>仪表板</td>
        <td>PTLTAB | 仪表板</td>
        <td>PORTALTABLES_CURRENT<br>PORTALTABLES_DAILY_HISTORY<br>PORTALTABLES_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID （自身）<br>SYSID<br>USERID</td>
        <td>不是关系；用于内部应用目的<br>USERS_CURRENT | 不支持USERID <br>门户配置文件表<br>Self<br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID  </td>
    </tr>
    <tr>
        <td>门户选项卡部分</td>
        <td>仪表板节</td>
        <td>PRTBSC | 门户选项卡部分</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (self)<br>SYSID</td>
        <td>当前不支持日历门户节<br>当前不支持外部节表<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>在PORTALSECTIONOBJCODE字段<br>PORTALTABLES_CURRENT中标识的对象的ID | PORTALTABID<br>Self<br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>报表上次查看者</td>
        <td>PLSLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID  </td>
    </tr>
    <tr>
        <td>项目组合</td>
        <td>项目组合</td>
        <td>端口 | Portfolio</td>
        <td>Portfolio_CURRENT<br>PORTFOLIO_每日_历史记录<br>PORTFOLIO_事件<br>PORTFOLIO_CUSTOM_VALUE_CURRENT<br>PORTFOLIO_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIO_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>当前不支持<br>CATEGORIES_CURRENT记分卡表 | CATEGORYID<br>用户当前 | 用户ID<br>组当前 | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | 用户ID<br>自身</td>
    </tr>
    <tr>
        <td>首选项</td>
        <td>查看、筛选、分组、报告定义</td>
        <td>PROSET | 首选项</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID （自身） <br>SYSID  </td>
        <td>不是关系；用于内部申请<br>自身<br>不是关系；用于内部申请  </td>
    </tr>
    <tr>
        <td>项目群</td>
        <td>项目群</td>
        <td>PRGM | 项目</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORY_CURRENT | CATEGORYID<br>用户当前 | USERID<br>组当前 | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_当前 | PORTFOLIOID<br>自身</td>
    </tr>
    <tr>
        <td>项目</td>
        <td>项目</td>
        <td>项目 | 项目</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFID<br>REJECTIONISSUEID<br>RESOURCEPOOLID<br>SCHEDEDID SPONSORID<br>SUBMITTEDBYID<br>TEAMID<br>TEMPLATEID<br><br></td>
        <td>不是Workfront关系；用于集成到外部系统<br>当前不支持<br>APPROVALPROCESSES_CURRENT的记分卡表 | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>类别_当前 | CATEGORYID<br>公司_当前 | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | 当前不支持APPROVALSTEPID<br>记分卡表<br>USER_CURRENT | USERID<br>组当前 | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>用户当前 | 当前不支持USERID<br>Pop帐户表<br>PORTFOLIO_当前 | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | 当前不支持PROGRAMID<br>Self<br>队列定义表<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | 用户ID<br>团队当前 | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>项目团队用户</td>
        <td>项目团队用户</td>
        <td>PRT | 项目用户</td>
        <td>PROJECTSUSERS_CURRENT<br>PROJECTSUSERS_DAILY_HISTORY<br>PROJECTSUSERS_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERID (self)<br>SYSID<br>TMPUSERID<br>USERID</td>
        <td>项目当前 | PROJECTID<br>Self<br>不是关系；用于内部应用程序目的<br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>项目团队用户角色</td>
        <td>项目团队用户角色</td>
        <td>团队 | ProjectUserRole</td>
        <td>PROJECTSUSERSROLES_CURRENT<br>PROJECTSUSERSROLES_DAILY_HISTORY<br>PROJECTSUSERSROLES_EVENT</td>
        <td>PROJECTID<br>PROJECTSUSERSROLEID (self)<br>ROLEID<br>SYSID<br>USERID</td>
        <td>项目当前 | PROJECTID<br>自身<br>角色_当前 | ROLEID<br>不是关系；用于内部应用目的<br>USERS_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>费率卡</td>
        <td>费率卡</td>
        <td>RTCRD |评级卡</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY<br>RATECARD_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (SELF) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>用户_当前 | 用户ID <br>用户_当前 | 用户ID    <br>Self<br>在SECURITYOBJCODE字段中标识的对象的ID <br>在SOURCEOBJCODE字段中标识的对象的ID<br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>报告文件夹</td>
        <td>报告文件夹</td>
        <td>RPTFDR | 报表文件夹</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY<br>REPORTFOLDERS_EVENT</td>
        <td>REPORTFOLDERID (self)<br>SYSID</td>
        <td>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>报表视图统计计数</td>
        <td>报表视图统计计数</td>
        <td>PLSVST | PortalSectionStatisticInfo</td>
        <td>REPORTVIEWSTATISTICCOUNTS_CURRENT<br>REPORTVIEWSTATISTICCOUNTS_DAILY_HISTORY<br>REPORTVIEWSTATISTICCOUNTS_EVENT</td>
        <td>REPORTID<br>REPORTVIEWSTATISTICCOUNTID (self)<br>SYSID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID<br>Self<br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>可报告预算小时数</td>
        <td>可报告预算小时数</td>
        <td>RPBGHR | 预算小时</td>
        <td>REPORTABLEBUDGETEDHOURS_CURRENT<br>REPORTABLEBUDGETEDHOURS_DAILY_HISTORY<br>REPORTABLEBUDGETEDHOURS_EVENT</td>
        <td>PROJECTID<br>REPORTABLEBUDGETEDHOURID (self)<br>ROLEID<br>SYSID<br>USERID</td>
        <td>项目当前 | PROJECTID<br>自身<br>角色_当前 | ROLEID<br>不是关系；用于内部应用目的<br>USERS_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>保留时间</td>
        <td>（个人）休假</td>
        <td>REVT | 空闲时间</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID （自身）<br>SYSID<br>TASKID<br>USERID</td>
        <td>自身<br>不是关系；用于内部申请<br>TASKS_CURRENT | TASKID<br>用户_当前 | 用户ID</td>
    </tr>
    <tr>
        <td>资源管理器</td>
        <td>资源管理器</td>
        <td>RESMGR | 资源管理器</td>
        <td>RESOURCEMANAGERS_CURRENT<br>RESOURCEMANAGERS_DAILY_HISTORY<br>RESOURCEMANAGERS_EVENT</td>
        <td>ID （自身）<br>PROJECTID<br>RESOURCEMANAGERID<br>SYSID<br>TEMPLATEID</td>
        <td>自助<br>项目_当前 | PROJECTID<br>USERS_CURRENT | USERID<br>不是关系；用于内部应用程序目的<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>资源池</td>
        <td>资源池</td>
        <td>RSPL | 资源池</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID （自身）<br>SYSID  </td>
        <td>USERS_CURRENT | 用户ID <br>用户_当前 | USERID <br>Self<br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>丰富文本备注</td>
        <td>丰富文本备注</td>
        <td>RHNOTE | 富文本注释</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID （自身）<br>SYSID</td>
        <td>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>富文本参数值</td>
        <td>富文本参数值</td>
        <td>RCHVAL | RtfParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID （自身） <br>SYSID  </td>
        <td>参数值表当前不支持<br>自身<br>不是关系；用于内部应用程序目的  </td>
    </tr>
    <tr>
        <td>风险</td>
        <td>风险</td>
        <td>风险 | 风险</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGEERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (self)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>用户_当前 | 用户ID <br>PROJECTS_CURRENT | PROJECTID   <br>自身<br>RISKTYPES_CURRENT | RISKTYPEID<br>不是关系；用于内部应用目的<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>风险类型</td>
        <td>风险类型</td>
        <td>RSKTYP | 风险类型</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>自身<br>不是关系；用于内部申请</td>
    </tr>
    <tr>
        <td>角色</td>
        <td>工作角色</td>
        <td>角色 | 工作角色</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | 不支持USERID<br>布局模板表<br>RATECARD_CURRENT | RATECARDID<br>自助<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>计划</td>
        <td>计划</td>
        <td>时间表 | 计划</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>组当前 | GROUPID<br>GROUP_CURRENT | GROUPID<br>自助</td>
    </tr>
    <tr>
        <td>步骤审批者</td>
        <td>步骤审批者</td>
        <td>SPAPVR | 阶段审批者</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>不是关系；用于内部应用程序目的<br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | 用户ID</td>
    </tr>
    <tr>
        <td>任务</td>
        <td>任务</td>
        <td>任务 | 任务</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTOTEID LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMEID<br>ROLEID<br>SUBMITTEDBYID<br>TASKID<br>TEAMID<br>TEMPLATETASKID<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>类别_当前 | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | 当前不支持ITERATIONID<br>Kanban展示板表<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | 当前不支持PROJECTID<br>周期性规则表<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | 用户ID<br>自身<br>团队当前 | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>前置任务</td>
        <td>前置任务</td>
        <td>前置任务 | 前置任务</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID （自身）<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>Self<br>TASKS_CURRENT | TASKID<br>任务_当前 | TASKID <br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>团队</td>
        <td>团队</td>
        <td>TEAMOB | 团队</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>组当前 | 不支持GROUPID<br>布局模板表<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>Self<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>团队成员</td>
        <td>其他团队、团队成员</td>
        <td>TEAMMB | 团队成员</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID （自身）<br>USERID</td>
        <td>不是关系；用于内部申请<br>TEAMS_CURRENT | TEAMID<br>自助<br>用户_当前 | 用户ID</td>
    </tr>
    <tr>
        <td>团队成员角色</td>
        <td>团队成员角色</td>
        <td>团队成员 | 团队成员角色</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID （自身）<br>USERID</td>
        <td>ROLES_CURRENT | 角色ID <br>团队_当前 | TEAMID<br>自助<br>用户_当前 | 用户ID</td>
    </tr>
    <tr>
        <td>模板</td>
        <td>模板</td>
        <td>模板 | 模板</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEAMID<br>TEMPLATEID （自助）</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>类别_当前 | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>组_当前 | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>用户_当前 | 用户ID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | 当前不支持PROGRAMID<br>队列定义表<br>SCHEDULES_CURRENT | SCHEDULEID <br>不是关系；用于内部申请<br>TEAMS_CURRENT | TEAMID<br>自助</td>
    </tr>
    <tr>
        <td>模板分派</td>
        <td>模板分派</td>
        <td>任务 | 模板分派</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (self)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | 用户ID<br>类别_当前 | CATEGORYID<br>用户_当前 | USERID<br>OBJCODE字段<br>ROLES_CURRENT中标识的对象的ID | ROLEID<br>不是关系；用于内部应用程序目的<br>TEAMS_CURRENT | TEAMID<br>当前不支持<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>模板任务</td>
        <td>模板任务</td>
        <td>TTSK | 模板任务</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br>RECURRENCERULEID<br>ROLEID<br>SYSID<br>TEAMAMTIMELINEABLEID<br>TEMPLATEID<br>ID templatetaskid (self)<br></td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>用户_当前 | 用户ID<br>类别_当前 | CATEGORYID<br>用户_当前 | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>注释_当前 | NOTEID<br>用户_当前 | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>当前不支持<br>ROLES_CURRENT | ROLEID<br>不是关系；用于内部应用程序目的<br>TEAMS_CURRENT | 当前不支持TEAMID<br>团队时间线表<br>TEMPLATES_CURRENT | TEMPLATEID<br>自身</td>
    </tr>
    <tr>
        <td>模板任务前置任务</td>
        <td>模板前置任务</td>
        <td>已触发 | 前置任务</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (self)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>自身<br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>时间表</td>
        <td>时间表</td>
        <td>TSHET | 工时表</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>Self<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>用户当前 | 用户ID</td>
    </tr>
    <tr>
        <td>时间表配置文件</td>
        <td>时间表配置文件</td>
        <td>TSPRO | 周期性工时表</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (self)</td>
        <td>USERS_CURRENT | USERID<br>用户_当前 | 用户ID <br>组_当前 | GROUPID<br>不是关系；用于内部应用程序目的<br>自身</td>
    </tr>
    <tr>
        <td>UI筛选器</td>
        <td>筛选条件</td>
        <td>UIFT | 筛选</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY<br>UIFILTERS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (self)</td>
        <td>不是关系；用于内部应用目的<br>USERS_CURRENT | 用户ID <br>用户_当前 | USERID <br>在OBJCODE字段中标识的对象的ID<br>PREFERENCES_CURRENT | PREFERENCEID<br>不是关系；用于内部应用目的<br>自身</td>
    </tr>
    <tr>
        <td>UI分组依据</td>
        <td>分组</td>
        <td>UIGB | 分组</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>组_当前 | GROUPID <br>USERS_CURRENT | USERID <br>不是关系；用于内部应用程序目的<br>自身</td>
    </tr>
    <tr>
        <td>UI模板</td>
        <td>布局模板</td>
        <td>UITMPL | 布局模板</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (self)</td>
        <td>不是关系；用于内部应用目的<br>USERS_CURRENT | 用户ID <br>用户_当前 | USERID <br>在OBJCODE字段中标识的对象的ID<br>PREFERENCES_CURRENT | PREFERENCEID<br>不是关系；用于内部应用目的<br>自身</td>
    </tr>
    <tr>
        <td>用户界面视图</td>
        <td>查看</td>
        <td>UIVIEW | 视图</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (self)</td>
        <td>不是关系；用于内部应用目的<br>USERS_CURRENT | 用户ID <br>用户_当前 | USERID <br>在OBJCODE字段中标识的对象的ID<br>PREFERENCES_CURRENT | PREFERENCEID<br>不是关系；用于内部应用目的<br>自身</td>
    </tr>
    <tr>
        <td>用户</td>
        <td>用户</td>
        <td>用户 | 用户</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>ID portalprofileid<br>PREFUIID<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UITEMPLATEID<br>USERID<br>UUMUSERID</td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>类别_当前 | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>不是关系；用于内部应用程序目的<br>USER_CURRENT | 用户ID<br>组当前 | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | 不支持NOTEID<br>布局模板表<br>USER_CURRENT | 不支持USERID<br>门户配置文件表<br>不是关系；用于内部应用程序目的<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>不是关系；用于内部应用程序目的</td>
    </tr>
    <tr>
        <td>用户委托</td>
        <td>用户委托</td>
        <td>超级 | 用户委托</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID（自身）</td>
        <td>USERS_CURRENT | USERID<br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID <br>自身</td>
    </tr>
    <tr>
        <td>用户组</td>
        <td>其他组</td>
        <td>USRGPS | 用户组</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (self)</td>
        <td>组_当前 | GROUPID <br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID <br>自身</td>
    </tr>
    <tr>
        <td>用户位置</td>
        <td>用户位置</td>
        <td>USRLOC | 用户位置</td>
        <td>USERLOCATIONS_CURRENT<br>USERLOCATIONS_DAILY_HISTORY<br>USERLOCATIONS_EVENT</td>
        <td>CLASSIFIERID<br>SYSID<br>USERID<br>USERLOCATIONID（自身）</td>
        <td>CLASSIFIER_CURRENT | CLASSIFIERID<br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID<br>自身</td>
    </tr>
    <tr>
        <td>用户角色</td>
        <td>其他角色</td>
        <td>USROL | 用户角色</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>角色ID <br>SYSID<br>用户ID    <br>USERROLESETID<br>USERSROLEID（自身）</td>
        <td>ROLES_CURRENT | ROLEID <br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID    <br>USERROLESET_CURRENT | USERROLESETID<br>自身</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | 用户首选项</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY<br>USERPREFVALUES_EVENT</td>
        <td>SYSID    <br>用户ID <br>用户PREFVALUEID （自身）</td>
        <td>不是关系；用于内部应用目的<br>USERS_CURRENT | 用户ID    <br>自助</td>
    </tr>
    <tr>
        <td>用户角色集</td>
        <td>用户角色集</td>
        <td>URSET | 用户角色集</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>用户ID    <br>USERROLESETID（自身）</td>
        <td>ROLES_CURRENT | ROLEID <br>不是关系；用于内部应用程序目的<br>USERS_CURRENT | 用户ID <br>自身</td>
    </tr>
    <tr>
        <td>用户决策</td>
        <td>用户决策</td>
        <td>USRDEC | 用户决策</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID （自身）<br>SYSID <br>用户ID  </td>
        <td>Self<br>不是关系；用于内部申请<br>USERS_CURRENT | 用户ID </td>
    </tr>
    <tr>
        <td>工作项</td>
        <td>工作项</td>
        <td>WRKIT | 工作项</td>
        <td>WORKITEMS_CURRENT<br>WORKITEMS_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>用户ID <br>工作项ID （自身）</td>
        <td>ASSIGNATIONS_CURRENT | ASSIGNMENTID <br>在OBJOBJCODE字段<br>OPTASK_CURRENT中标识的对象的ID | OPTASKID    <br>项目_当前 | PROJECTID <br>不是关系；用于内部应用程序目的<br>TASKS_CURRENT | TASKID    <br>用户_当前 | 用户ID    <br>自助 </td>
    </tr>
  </tbody>
</table>
