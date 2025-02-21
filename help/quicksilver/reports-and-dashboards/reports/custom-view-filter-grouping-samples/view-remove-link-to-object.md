---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 视图：删除列中对象的链接
description: 默认情况下，显示在视图链接中的某些对象将指向对象的“详细信息”页面。 例如，显示项目名称的列是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# 视图：删除列中对象的链接

<!--Audited: 11/2024-->

默认情况下，显示在视图链接中的某些对象将指向对象的“详细信息”页面。 例如，显示项目名称的列是指向项目的链接；显示用户名称的列是指向用户配置文件页面的链接。

您可以使用在所有视图中显示的列中的文本模式删除此链接。

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
   <td> <p> 当前： 
   <ul>
   <li>请求修改视图</li> 
   <li>计划修改报告</li>
   </ul>
     </p>
     <p> 新增： 
   <ul>
   <li>修改视图的参与者</li> 
   <li>用于修改报告的标准</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
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


## 示例：从任务视图的“任务名称”列中移除指向任务的链接：

1. 转到任务列表。
1. 从&#x200B;**视图**&#x200B;下拉菜单中，单击&#x200B;**新建视图**&#x200B;以创建新视图。

   或

   单击&#x200B;**编辑图标** ![编辑图标](assets/edit-icon.png)

   要编辑现有视图，请选择该视图。

1. 单击&#x200B;**添加列**&#x200B;以添加新列。

   或

   单击现有列，该列带有指向对象的链接。

1. 单击&#x200B;**切换到文本模式** > **编辑文本模式**。
1. 删除在&#x200B;**编辑文本模式**&#x200B;框中找到的文本，然后将其替换为以下代码：

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >您可以通过调整以下内容，对其他对象使用类似的代码：
   >
   >* 将代码的`valuefield`行替换为`valueexpression`，并在等号后面保留大括号中包含的相同名称。
   >* 从列的原始文本中删除所有以`link.`开头的行。 例如，消除以下所有行：
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. 单击&#x200B;**完成**，然后单击&#x200B;**保存视图**。

