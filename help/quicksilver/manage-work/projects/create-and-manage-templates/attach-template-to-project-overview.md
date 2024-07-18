---
content-type: overview
product-area: templates
keywords: 覆盖，字段，已覆盖
navigation-topic: templates-navigation-topic
title: 将模板附加到项目的概述
description: 将模板附加到现有项目时，您正在根据该模板修改项目上的某些信息。 该项目的某些信息保持不变。
author: Alina
feature: Work Management
exl-id: 7f0137b6-ce8e-4b66-ad55-e6dc2aae09d9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 5%

---

# 将模板附加到项目的概述

将模板附加到现有项目时，您正在根据该模板修改项目上的某些信息。 该项目的某些信息保持不变。

有关如何将模板附加到项目的信息，请参阅[将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

## 将模板添加到项目时的注意事项

将模板添加到项目时，请考虑以下事项：

* 您只能将活动模板附加到项目。
* 仅当您的Adobe Workfront管理员或组管理员在项目偏好设置区域中启用了此功能时，您才可以在项目处于“完成”、“终止”或“未决批准”状态时向项目附加模板。 有关设置项目首选项的信息，请参阅[配置系统范围项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。
* 除非排除特定模板任务不添加到附件流程中，否则所有模板任务都将添加到现有项目中。
* 大多数模板设置已添加到项目中。 某些项目设置将被保留。 有关信息，请参阅本文中的[了解附加模板](#understand-changes-to-project-fields-when-attaching-a-template)时项目字段的更改。

## 了解附加模板时项目字段的更改 {#understand-changes-to-project-fields-when-attaching-a-template}

>[!IMPORTANT]
>
>将模板附加到项目与从模板创建项目不同。 从模板创建项目时，所有模板字段都会转移到新项目。 附加模板时，某些现有项目字段会保持不变。

某些模板设置会自动传输到项目，除非您在模板附加过程中明确将其标记为排除。 当您将其标记为排除时，项目字段值将保留。

但是，在将模板附加到项目的过程中，并非所有项目字段都可供管理。 有关信息，请参阅[将模板附加到项目](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md)。

下表描述了附加模板时项目字段的默认值，以及在附加过程中可以管理哪些字段以覆盖默认行为：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>字段</td> 
   <td>默认情况下，在附加模板的过程中会发生什么情况</td> 
   <td>能够在附件流程中管理字段更新 </td> 
  </tr> 
  <tr> 
   <td>描述</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>状态</p> </td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>URL</td> 
   <td>从模板转移（如果项目上的字段为空）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>优先级</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>完成情况类型</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>排程模式</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>计划日期</td> 
   <td>可能会根据添加的任务而更改</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>实际日期</td> 
   <td>可能会根据添加的任务而更改</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目组合</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目群</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>组</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>公司</td> 
   <td>从模板转移（如果项目上的字段为空）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>规划小时数</td> 
   <td>可能会根据添加的任务而更改</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目所有者</td> 
   <td>从模板转移（如果项目上的字段为空）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>项目赞助者</td> 
   <td>从模板转移（如果项目上的字段为空）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>资源管理器</td> 
   <td>已添加到项目中现有资源经理的列表</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>自定义Forms</td> 
   <td>除了项目中已存在的表单之外，还添加到项目中</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>预算</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>货币</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>绩效指数方法</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>EAC</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>规划收益</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>实际收益</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>里程碑路径</td> 
   <td>从模板转移（如果项目上的字段为空）</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>完成模式</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>摘要完成模式</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>更新类型</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>计划</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>用户空闲时间</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>资源均衡模式</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>风险（项目字段）</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>资源池</td> 
   <td>已添加到项目上现有资源池的列表</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>小时类型</td> 
   <td> <p>如果在附加过程中取消选择小时类型，则项目上的小时类型设置将保持不变。 </p> <p>如果选择，模板设置将转移到项目。 如果项目和模板上的小时类型筛选都设置为“是”，则模板中的小时类型将添加到项目中的小时类型。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p>✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td>提醒通知</td> 
   <td> <p>已添加到项目中的现有提醒列表。 </p> <p>如果在附件流程中取消选择，项目提醒通知将保持不变。 </p> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>任务默认审批流程</td> 
   <td>项目信息被保留</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>任务默认自定义Forms</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>工作投入</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>允许用户添加内联问题</span> </td> 
   <td><span>项目信息已保留</span> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>所有设置</td> 
   <td>模板设置会覆盖项目的模板设置</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>任务</td> 
   <td>在现有项目任务之外，添加到任务列表底部</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>文档</td> 
   <td>在现有项目文档之外，还添加到项目</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>风险（项目的“风险”区域中的对象）</td> 
   <td>在现有项目风险之外，还添加到项目 </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>审批流程</td> 
   <td>已从模板转移</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>记帐费率</td> 
   <td> <p>除了项目上的现有记帐费率之外，还从模板转移。 </p> <p>如果项目和模板中的同一工作角色具有不同的费率，则项目的费率保持不变。 </p> </td> 
   <td> <p> </p> <p>✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td>开票记录</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>费用</td> 
   <td>除了项目上的现有费用外，还从模板转移</td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>财务信息</td> 
   <td> <p>在附件流程中选择此选项后，以下字段将被传输或添加到项目中： </p> 
    <ul> 
     <li> <p>固定成本</p> <p>选择该选项后，将使用以下公式计算项目的已更新固定成本：</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li> 
     <li> <p>固定收入</p> <p>在选择该选项后，将使用以下公式计算项目的已更新固定收入：</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li> 
     <li> <p>任务的成本类型</p> <p>已从模板转移</p> </li> 
     <li> <p>任务的收入类型</p> <p>已从模板转移</p> </li> 
    </ul> <p>如果在附加过程中取消选择此字段，则会出现以下情况：</p> 
    <ul> 
     <li> <p>项目的固定成本和固定收入将保留。</p> </li> 
     <li> <p>从模板添加的任务的“成本”和“收入类型”设置为“无成本”和“不可记帐”</p> </li> 
    </ul> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td>小时</td> 
   <td>项目信息被保留</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>队列详细信息、主题组、队列主题、路由规则</td> 
   <td> <p>已从模板转移</p> <p>如果在附加过程中选择<strong>队列属性和问题设置</strong>选项，则模板的队列详细信息将覆盖项目的队列详细信息。 在这种情况下，模板的“路由规则”、“队列主题”和“主题组”将添加到项目的路由规则、队列主题和主题组。 <br>如果项目设置为请求队列，而您附加到项目的模板未设置为请求队列，则如果您选中<strong>队列属性和问题设置</strong>框，项目的队列信息将被删除。 <br>如果取消选中<strong>队列属性和问题设置</strong>框，则会保留项目的所有队列设置设置，并且不会附加模板中的队列设置设置。</p> </td> 
   <td> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p> </p> <p>✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td>任务限制</td> 
   <td> <p>已从模板转移 </p> <p>如果在附件流程期间取消选择任务约束，则任务约束将设置为“尽可能早”或“尽可能晚”，具体取决于项目“计划自”设置。 </p> </td> 
   <td> <p> </p> <p> </p> <p style="text-align: center;">✓ {\f13 }</p> </td> 
  </tr> 
  <tr> 
   <td>前置任务</td> 
   <td> <p>已从模板转移</p> <p>如果在连接过程中取消选择，则模板任务之间的所有前置任务连接都将被删除。</p> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
  <tr> 
   <td>共享选项</td> 
   <td> <p>如果在附件流程中取消选择此项，则项目权限将保持不变。</p> <p>如果在附件流程中选择了模板权限，则模板权限会添加到或覆盖项目的权限。 </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>示例： </b></span></span>如果用户A具有项目的“查看”权限，但他们具有模板的“管理”权限，则在附加模板后，用户A将获得项目的“管理”访问权限。</p> </td> 
   <td>✓ {\f13 }</td> 
  </tr> 
 </tbody> 
</table>

 

<!--WRITER
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<div>
<h2> </h2>
<h2>Understand changes to project fields when attaching a template</h2> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and replaced with the table above, per Anna)</p>
-->
<!--
<p>Some template settings automatically transfer to the project, unless you specifically mark them to be excluded during the template attachment process. When you mark them to be excluded, the project field values are preserved. </p> <note type="important">
Not all project fields are available to manage in the process of attaching a template to a project. For information, see
<a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md" class="MCXref xref">Attach a template to a project</a>.
</note>
<p>The following scenarios exist when attaching a template to an existing project: </p>
<ul>
<li> <p><a href="#project-fields-that-are-empty-and-the-template-information-updates-them" class="MCXref xref">Project fields that are empty and the template information updates them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-the-template-information-overwrites-them" class="MCXref xref">Project fields that are populated and the template information overwrites them</a> </p> </li>
<li> <p><a href="#project-fields-that-are-populated-and-they-remain-unchanged-after-attaching-the-template" class="MCXref xref">Project fields that are populated and they remain unchanged after attaching the template</a> </p> </li>
</ul> <note type="important">
Attaching a template to a project is not the same as creating a project from a template. When you create a project from a template all template fields transfer to the new project. Attaching a template leaves some of the existing project's fields unchanged.
</note>
<p><strong>Project fields that are empty and the template information updates them</strong></p>
<p>Most project fields that are empty are populated with template information when attaching the template to an existing project. </p>
<p><strong>Project fields that are populated and the template information overwrites them</strong></p>
<p>The following fields always overwrite or update existing project information with template information when you attach a template to the project and they cannot be managed during attaching the template: </p>
<ul>
<li> <p><b>Resource manager</b>: The template Resource Managers are added to the list of existing resource managers on the project.</p> </li>
</ul>
<ul>
<li> <p><b>Financial Information</b>: You can indicate whether you want financial information to transfer from the template or to keep the existing financial information on the project in the process of attaching a template. However, when the Financial Information option is selected to indicate that you intend to keep the information from the template, the following fields are updated on the project: </p>
<ul>
<li> <p> The updated Fixed Cost of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Cost = Original Project Fixed Cost + Template Fixed Cost</code> </p> </li>
<li> <p>The updated Fixed Revenue of the project is calculated using the following formula:</p> <p><code>Updated Project Fixed Revenue = Original Project Fixed Revenue + Template Fixed Revenue </code> </p> </li>
</ul> </li>
</ul>
<ul>
<li> <p><b>Filter Hour Types</b> </p> </li>
</ul>
<ul>
<li> <p><b>Access settings</b> </p> </li>
</ul>
<ul>
<li> <p><b>Custom&nbsp;Forms</b>:&nbsp;Template custom forms are added to the project, in addition to existing project custom forms. If the fields from the template custom forms already exist on the project and contain information, they preserve the information already on the project. You cannot edit them during attaching the template. </p> </li>
</ul>
<ul>
<li> <p><b>Start&nbsp;From</b> </p> </li>
</ul>
<p><strong>Project fields that are populated and they remain unchanged after attaching the template</strong></p>
<p>The following fields remain unchanged on the project, even if they are also populated on the template, and they cannot be managed during attaching the template: </p>
<ul>
<li> <p style="font-weight: bold;">URL</p> </li>
<li> <p style="font-weight: bold;">Project Owner</p> </li>
<li> <p style="font-weight: bold;">Project&nbsp;Sponsor</p> </li>
<li> <p style="font-weight: bold;">Group</p> </li>
<li> <p style="font-weight: bold;">Company</p> </li>
<li> <p style="font-weight: bold;">Currency</p> </li>
<li> <p style="font-weight: bold;">Milestone Path</p> </li>
<li> <p><b>Completion Mode</b> </p> </li>
<li> <p style="font-weight: bold;">Resource Pool</p> </li>
<li> <p style="font-weight: bold;">Tasks Settings fields</p> </li>
<li class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p style="font-weight: bold;">Issue Settings fields</p> </li>
</ul>
</div>
<p>&nbsp;</p>
</div>
-->

 
