---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：审批信息问题'
description: 以下问题视图显示了批准流程、步骤、批准者的名称和批准前的问题状态。 其中某些字段无法通过标准界面生成器访问。
author: Nolan
feature: Reports and Dashboards
exl-id: 4e123844-a0d6-474b-87fb-d30ed391ad07
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# 查看：审批信息存在问题

<!--Audited: 11/2024-->

以下问题视图显示了批准流程、步骤、批准者的名称和批准前的问题状态。 其中某些字段无法通过标准界面生成器访问。

![custom_issue_view_with_approval_info.png](assets/custom-issue-view-with-approval-info-350x46.png)

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：<ul><li>修改视图的参与者</li><li>用于修改报告的标准</li></ul></p><p>或</p>当前：<ul><li>请求修改视图</li><li>计划修改报告</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对报告、功能板和日历的访问权限以修改报告</p> <p>编辑对筛选器、视图和分组的访问权限以修改视图</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理报表的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 查看有关批准信息的问题

1. 转到问题列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请消除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**，然后单击&#x200B;**编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=40
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=220
   column.1.descriptionkey=assignedto
   column.1.linkedname=assignedTo
   column.1.listsort=nested(assignedTo).string(name)
   column.1.namekey=assignedto
   column.1.querysort=assignedTo:name
   column.1.shortview=true
   column.1.stretch=0
   column.1.valuefield=assignedTo:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=role
   column.2.linkedname=role
   column.2.listsort=nested(role).string(name)
   column.2.namekey=role
   column.2.querysort=role:name
   column.2.shortview=false
   column.2.stretch=25
   column.2.valuefield=role:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Approval Process Name
   column.3.linkedname=direct
   column.3.listsort=string(name)
   column.3.name=Approval Process Name
   column.3.querysort=name
   column.3.shortview=false
   column.3.stretch=35
   column.3.valuefield=approvalProcess:name
   column.3.valueformat=HTML
   column.3.width=220
   column.4.description=Approval Step Name
   column.4.linkedname=direct
   column.4.listsort=string(name)
   column.4.name=Approval Step Name
   column.4.querysort=name
   column.4.shortview=false
   column.4.stretch=0
   column.4.valuefield=currentApprovalStep:name
   column.4.valueformat=HTML
   column.4.width=220
   column.5.description=Previous Status
   column.5.linkedname=direct
   column.5.listsort=string(name)
   column.5.name=Previous Status
   column.5.querysort=name
   column.5.shortview=false
   column.5.stretch=0
   column.5.valuefield=previousStatus
   column.5.valueformat=HTML
   column.5.width=220
   column.6.linkedname=direct
   column.6.listsort=HTML(approversString)
   column.6.namekey=approver.plural.abbr
   column.6.querysort=approversString
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=approversString
   column.6.valueformat=HTML
   column.6.viewalias=approver.plural
   column.6.width=200
   ```

1. 单击&#x200B;**完成** > **保存视图**。
1. （可选）更新视图名称，然后单击&#x200B;**保存视图**。
