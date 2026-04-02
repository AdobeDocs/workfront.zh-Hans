---
content-type: overview
product-area: projects
navigation-topic: financials
title: 定义加班率
description: 您可以定义任务的超时比率，以调整任务分配的计划收入计算。
author: Lisa
feature: Work Management
source-git-commit: bf8dcc9dfa9697c8d212072bb511c57aa01e7529
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 5%

---

# 定义加班率

{{highlighted-preview-article-level}}

将加班比率添加到任务时，加班比率将应用于任务的所有分配。 它会将该任务的所有计划小时数相乘，并且影响计划收入计算。

同一任务中的分配的加班率不能改变。 如果需要不同的超时乘数，则必须在父任务下创建单独的子任务。

>[!NOTE]
>
>没有验证阻止将加班率添加到非加班任务。

## 计划收入的加班计算

系统首先使用标准记帐费率层次结构确定记帐费率。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

如果任务中存在超时比率，则计算方式为：
计划收入=记帐费率×加班费率×计划小时数

如果加班率为空，则计算方式为：
计划收入=记帐费率×计划小时数

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront 包</td> 
   <td>工作流 Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront许可证</td> 
   <td>标准</td> 
  </tr> 
  <tr> 
   <td>访问级别配置</td> 
   <td>编辑对任务、项目和财务数据的访问权限</td> 
  </tr> 
  <tr> 
   <td>对象权限</td> 
   <td><p>管理包含编辑记帐费率的任务的权限</p>
     <p>为项目分配或更高权限</p></td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 先决条件

任务收入类型必须是每小时用户和角色。 有关详细信息，请参阅[收入和成本层次结构概览](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)。

必须在布局模板上启用&#x200B;**超时比率**&#x200B;字段。

1. 在布局模板中，单击&#x200B;**自定义用户看到的内容**&#x200B;下的向下箭头，然后单击&#x200B;**任务**。
1. 在&#x200B;**详细信息**&#x200B;部分中，选择&#x200B;**财务**&#x200B;区域中的&#x200B;**超时比率**&#x200B;字段。

   有关详细信息，请参阅[使用布局模板自定义详细信息视图](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)。

## 定义任务的超时比率

1. 转到要编辑的任务。

   有关详细信息，请参阅[在任务详细信息部分](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md)中管理任务财务。

1. 单击左侧面板中的&#x200B;**任务详细信息**。
1. 在&#x200B;**财务**&#x200B;区域中，在&#x200B;**加班比率**&#x200B;字段中输入加班乘数。
1. 单击&#x200B;**保存更改**。

