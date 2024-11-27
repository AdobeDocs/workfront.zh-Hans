---
title: 从Adobe Workfront导入字段
description: 在Adobe Workfront Planning中，您可以为每种记录类型创建自定义字段。 然后，您可以将该字段与Workfront Planning记录关联。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 0da877936ba8f52341a5b151f76710c979ce9294
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 7%

---


<!--add to TOC-->

# 从Adobe Workfront导入字段

<span class="preview">此页面上的信息引用了尚未公开的功能。 它仅在“预览”环境中对所有客户可用。 在每月发布到生产环境后，生产环境中为启用快速发布的客户提供了相同的功能。</span>

<span class="preview">有关快速发布的信息，请参阅[为您的组织启用或禁用快速发布](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)。</span>


{{planning-important-intro}}

您可以导入现有Workfront字段的副本。 从Workfront导入字段会为Workfront Planning记录类型创建每个字段的副本。


## 访问要求

+++ 展开以查看Workfront Planning的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 产品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront规划<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront计划*</p></td> 
   <td> 
<p>以下任意Workfront计划：</p> 
<ul><li>选择</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning不适用于旧版Workfront计划</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront规划包*</p></td> 
   <td> 
<p>任何 </p> 
<p>有关每个Workfront计划中包括的内容的更多信息，请联系您的Workfront客户经理。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront平台</p></td> 
   <td> 
<p>贵组织的Workfront实例必须载入AdobeUnified Experience，才能访问Workfront Planning的所有功能。</p> 
<p>有关详细信息，请参阅<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">AdobeWorkfront的Unified Experience</a>。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront许可证*</p></td> 
   <td><p> 标准 </p>
   <p>Workfront计划不适用于旧版Workfront许可证</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>访问级别配置</p></td> 
   <td> <p>Adobe Workfront Planning没有访问级别控制</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>对象权限</p></td> 
   <td>   <p>管理工作区</a>的权限 </p>  
   <p>系统管理员有权访问所有工作区，包括他们未创建的工作区。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>布局模板</p></td> 
   <td> <p>必须为所有用户(包括Workfront管理员)分配一个布局模板，该模板应包括主菜单中的Planning区域。 </p> </td> 
  </tr> 
</tbody> 
</table>

*有关Workfront访问要求的详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 关于从Workfront导入字段的注意事项

* 您可以在Workfront Planning中将本机或自定义Workfront字段导入记录类型。
* 导入Workfront字段会创建相同字段的副本，并在Workfront Planning中保留字段名称。 在将字段复制到Workfront Planning后，这些字段与原始Workfront字段无关，并且不共享信息。
<!--check this: * You do not need permissions or access to Workfront objects to be able to add their fields to Workfront Planning. -->
* 您可以从以下Workfront对象添加本机或自定义字段：
   * 项目组合
   * 项目群
   * 项目
   * 任务
   * 问题
   * 文档
   * 公司
   * 组
   * 用户
   * 工作角色
   * 任务分配
   * 小时
   * 账单记录
     <!--Available only to Preview, but might not come to Prod:* Rate card-->
   * 费用
   * 迭代
     <!--* Non-labor resource-->
     <!--* Non-labour resource category-->
* 在Workfront Planning中导入Workfront字段后，这些字段可能不会保留其字段类型。

  下表显示了Workfront字段类型及其对应的Workfront规划字段类型。

  | Workfront字段类型 | Workfront Planning字段类型 |
  |------------------------------------------|-------------------------------|
  | 文本格式的单行文本 | 单行文本 |
  | 数字格式的单行文本 | 数字 |
  | 货币格式的单行文本 | 货币 |
  | 段落 | 段落 |
  | 带格式文本 | 段落 |
  | 单选下拉菜单 | 单选 |
  | 多选下拉框 | 多选 |
  | 不支持用户预输入筛选器 | 人员 |
  | 已计算* | 公式 |
  | 日期 | 日期 |
  | 复选框组 | 多选 |
  | 单选按钮 | 多选 |

  *计算字段将在以后可用。
Workfront Planning不支持所有其他Workfront字段类型。


## 从 Workfront 导入字段

<!--the first 3 steps are the same as in Create fields-->

{{step1-to-planning}}

1. 单击要为其创建字段的记录类型的工作区。

   此时会打开工作区，并显示记录类型。

1. 单击记录类型的卡。

   与记录类型关联的所有现有记录都会显示在表格视图的行中。

   >[!TIP]
   >
   >    某些字段可能已隐藏。 单击&#x200B;**字段**&#x200B;并为要作为表视图中的列查看的字段启用切换功能。

1. 单击表格视图右上角的&#x200B;**+**&#x200B;图标

   或

   将鼠标悬停在任何列的标题上，单击字段名称后面的向下箭头，然后单击&#x200B;**向左插入**&#x200B;或&#x200B;**向右插入**&#x200B;以添加新字段。
1. 单击&#x200B;**新建字段**&#x200B;选项卡右下角的&#x200B;**添加现有**。<!--check UI - did they change this??-->

   ![](assets/add-existing-fields-from-workfront-modal.png)

1. 在搜索区域中开始键入现有Workfront字段的名称，然后在列表中显示&#x200B;**+**&#x200B;时单击该名称。
1. （可选）键入其他字段，然后在列表中显示&#x200B;**+**&#x200B;时单击该字段。
1. （可选）单击&#x200B;**筛选器**&#x200B;图标![](assets/filters-in-import-fields-icon.png)，然后更新以下一个或两个字段：

   * 对象类型：选择要导入其字段的Workfront对象类型。
   * 自定义表单：从Workfront中选择一个或多个自定义表单。 您可以选择自定义表单，而无需先选择对象类型。
1. 单击&#x200B;**+**，然后单击&#x200B;**添加字段**。
这些字段将添加到表格视图和记录的详细信息页面。

