---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: '查看：展开的用户详细信息'
description: 此“用户”视图显示有关用户的信息。 除了他们的姓名、访问级别和公司之外，它还会显示他们的组、团队和工作角色的列表。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a978b43-4718-43fb-80b8-844b35e09d06
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# 视图：展开的用户详细信息

此“用户”视图显示有关用户的信息。 除了他们的姓名、访问级别和公司之外，它还会显示他们的组、团队和工作角色的列表。

![expanded_user_view.png](assets/expanded-user-view-350x75.png)

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

## 查看展开的用户详细信息

要应用此视图，请执行以下操作：

1. 转到用户列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，选择&#x200B;**新建视图**。

1. 在&#x200B;**列预览**&#x200B;区域，除一个列外，请删除所有列。
1. 单击其余列的标题，然后单击&#x200B;**切换到文本模式**。
1. 将鼠标悬停在文本模式区域上，然后单击&#x200B;**单击以编辑文本**。
1. 删除在&#x200B;**文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: extra tag here that adds extra spaces in Preview)
   </MadCap:conditionalText>
   -->

   <pre>column.0.descriptionkey=name <br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.link.link=direct<br>column.0.listort=string(name){name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=accesslevel<br>column.link.link.property.0.name=ID<br>column.link.link.property.0.valuefield=accessLevel ：ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=accessLevel：objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=accessLevel<br>column.1.listsort=string(displayName)<br>column.1.namekey=accesslevel{25column<br>column 6}column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=accessLevel：displayName<br>column.1.valueformat=HTML<br>column.1.viewalias=accessLevel：displayName<br>column.1.width=100<br>column.2.link.property.0.name=ID<br>column.link.property .0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.value=val(objCode)<br>column.2.listdelimiter=<br>column.2.listmethod=nested(userGroups)。lists<br>column.2.namekey=group.plural<br>column.2.stretch=50<br>column.2.type=iterate<br>column.2.valuefield=group：name<br>column.2.valueformat =HTML<br>列。2.宽度=150<br>列。3.displayname=团队<br>列。3.listdelimiter=<br>列。3.listmethod=嵌套（团队）。lists<br>列。3.textmode=true<br>列。3.type=iterate<br>列。3.valueexpression={name}<br>列。3.valueformat=HTML<br>列。4.link.linkproperty.0.name=ID<br> column.4.link.linkproperty.0.valuefield=ID<br>column.4.link.linkproperty.0.valueformat=int<br>column.4.link.lookup=link.view<br>column.4.link.value=val(objCode)<br>column.4.listdelimiter=<br>column.4.listmethod=nested(userRoles)。lists<br>column.4.namekey=jobrole.plural<br>column.4.stretch=50<br>column.4.stretch=4.column .type=iterate<br>column.4.valuefield=role：name<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=company<br>column.5.link.linkproperty.0.name=ID<br>column.5.link.linkproperty.0.valuefield=company：ID<br>column.5.link.0.valueformat=int<br>column.link.lookup.lookup.link view<br>column.5.link.valuefield=company：objCode<br>column.5.link.valueformat=val<br>column.5.linkedname=company<br>column.5.listsort=nested(company)。string(name)<br>column.5.namekey=company<br>column.5.querysort=company：name<br>column.5.short=false<br>column.5.valuefield=company：name<br>column.column.5 valueformat=HTML<br>column.5.width=150<br><br><br></pre>

1. 单击&#x200B;**保存视图**。
