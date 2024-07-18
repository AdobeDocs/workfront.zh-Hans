---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：审批信息问题'
description: 以下问题视图显示了批准流程、步骤、批准者的名称和批准前的问题状态。 其中某些字段无法通过标准界面生成器访问。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# 查看：审批信息存在问题

以下问题视图显示了批准流程、步骤、批准者的名称和批准前的问题状态。 其中某些字段无法通过标准界面生成器访问。

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>请求修改视图 </p>
   <p>计划修改报告</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> <p><b>注释</b>

如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 查看有关批准信息的问题

1. 转到问题列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：
   <pre style="font-style: normal;">column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listort=string(name)<br>column(name){name){name.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=40<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=220<br>column.1.descriptionkey=assignedto<br>column.1.listort=nestalled(assignedTo){stringTo)。string(name)。string(name) 18}column.1.namekey=assignedto<br>column.1.querysort=assignedTo：name<br>column.1.shortview=true<br>column.1.stretch=0<br>column.1.valuefield=assignedTo：name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=role<br>column.2.linkedname=role{role<br>column.2.2.linkedname=role{role{role{role<br>column.2.2.2.listsort role)。string(name)<br>column.2.namekey=role<br>column.2.querysort=role：name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.description=批准流程名称<br>column.3.linkedname=direct<br>column.3.listsort=string （名称）<br>column.3.name=批准流程名称<br>column.3.querysort=name<br>column.3.shortview=false<br>column.3.stretch=35<br>column.3.valuefield=approvalProcess：name<br>column.3.valueformat=HTML<br>column.3.width=220<br>column.4.description=批准步骤名称<br>column.linkedname=direct<br>column.listort.string=direct{direct{direct<br>column.listort （名称）<br>column.4.name=批准步骤名称<br>column.4.querysort=name<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valuefield=currentApprovalStep：name<br>column.4.valueformat=HTML<br>column.4.width=220<br>column.5.description=Previous<br>column.5.linkedname=direct<br>column.5.listort(direct（字符串） name)<br>column.5.name=Previous Status<br>column.5.querysort=name<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=previousStatus<br>column.5.valueformat=HTML<br>column.5.width=220<br>column.6.linkedname=direct<br>column.6.listort=HTML(approvers){approvers7}column.6.namekey=approkey ver.plural.abbr<br>column.6.querysort=approversString<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=approversString<br>column.6.valueformat=HTML<br>column.6.viewalias=approver.plural<br>column.6.width=200<br><br></pre>

1. 单击&#x200B;**保存视图**。
