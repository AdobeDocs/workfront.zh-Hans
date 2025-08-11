---
title: 使用以前的数据自动填写请求
content-type: reference
description: 您可以使用AI通过来自先前请求的数据自动填写请求字段。
author: Becky
feature: Get Started with Workfront
source-git-commit: cf2ae77ed27b1dd30144f6de31bec474f53f1efb
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# 使用以前的数据自动填写请求

>[!NOTE]
>
>* 此功能将作为公开测试版在以下时间表中提供：
>
>   * 每月发布： 2025年9月11日
>   * 季度发布： 2025年10月16日

AI可帮助您根据先前的请求自动填写请求字段。 您可以在提交请求之前批准或拒绝这些建议。

自动填写不会覆盖您已填写的任何字段。

用户不会收到他们无权访问的数据建议。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新文档：参与者或更高版本</p>
   或
   <p>当前：请求或更高版本</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对问题的访问权限</p>  </td> 
  </tr> 
   <td role="rowheader">对象权限</td> 
   <td><p>将请求添加到请求队列的权限</p> <p>查看现有请求或更高权限</p> <p>有关设置请求队列的信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>。 </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

## 在填写表单时获取建议

自动填写可以在您填写表单时建议字段值。 在请求字段中输入值时，Workfront会将这些值与以前的请求进行比较。 如果输入的值与以前请求中类似上下文中的其他字段值紧密相关，则Workfront会推荐这些值。

例如，如果诊所始终使用相同的计费代码，那么在输入诊所名称时，Workfront会建议在适当的字段中输入该计费代码。

要根据以前的请求使用建议，请执行以下操作：

1. 开始创建请求。

   有关说明，请参阅[创建并提交请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

1. 开始填写字段。

   当您填写字段时，其他字段可能会显示建议。

1. 对于每个字段建议，请为该字段选择&#x200B;**接受**&#x200B;或&#x200B;**拒绝**。

   ![接受或拒绝建议](assets/accept-reject-suggestion.png)

   或

   选择页面顶部的&#x200B;**全部接受**&#x200B;或&#x200B;**全部拒绝**&#x200B;以接受或拒绝所有建议。

   >[!NOTE]
   >
   >当您提交请求时，任何未审核的建议都将被自动接受。
