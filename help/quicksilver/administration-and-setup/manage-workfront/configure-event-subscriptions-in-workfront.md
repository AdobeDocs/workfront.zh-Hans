---
user-type: administrator
content-type: how-to
product-area: system-administration
navigation-topic: manage-workfront
title: 在Workfront中配置事件订阅
description: 作为Adobe Workfront管理员，您可以在“设置”区域创建、查看和删除事件订阅，以将Workfront事件发送到外部端点。
feature: System Setup and Administration
role: Admin
author: Courtney
source-git-commit: 5a44679115dcfda871e2fe40c0c8443649fc43cf
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 5%
---

# 在Workfront中配置事件订阅

{{highlighted-preview-article-level}}

作为Adobe Workfront管理员，您可以在“设置”区域创建、查看和删除事件订阅。 事件订阅在发生指定事件时将Workfront事件信息发送到外部端点。

您可以在Workfront中创建和删除事件订阅，但无法编辑现有订阅。 如果您需要更改订阅，请删除它并创建一个新订阅。

有关活动订阅的详细信息，请参阅[活动订阅](/help/quicksilver/wf-api/api/event-subscriptions.md)下的文章。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 包</td>
   <td>“任一”</td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront许可证</td>
   <td>
    <p>标准</p>
    <p>规划</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">访问级别配置</td>
   <td>您必须是Workfront管理员。</td>
  </tr>
 </tbody>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建事件订阅

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**系统**，然后单击&#x200B;**事件订阅**。
1. 单击&#x200B;**新建事件订阅**。
1. 在&#x200B;**对象**&#x200B;字段中，选择要监视的Workfront对象。
1. 在&#x200B;**事件类型**&#x200B;字段中，选择是在创建、更新、删除还是共享对象时触发事件订阅。
1. 在&#x200B;**Webhook URL**&#x200B;字段中，输入应接收事件有效负载的终结点。
1. 在&#x200B;**身份验证令牌**&#x200B;字段中，输入用于向您的端点验证请求的令牌。
1. 如果您希望Workfront在发送有效负载之前对其进行编码，请启用选项以将有效负载作为Base64发送。
1. 如果需要，请添加一个或多个过滤器以限制触发订阅的事件。 可用的过滤器基于所选对象。
1. 单击&#x200B;**创建**。

有关端点要求的信息，请参阅[事件订阅提交要求](/help/quicksilver/wf-api/general/setup-event-sub-endpoint.md)。

## 查看事件订阅

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**系统**，然后单击&#x200B;**事件订阅**。

在事件订阅页面中，您可以查看为您的环境配置的订阅。 您还可以查看贵组织拥有的总订阅数，以及处于活动状态、已禁用或冻结状态的订阅数。

* **已禁用订阅**：由于多次交付失败，这些订阅已被自动禁用。
* **冻结的订阅**：由于传递问题，这些订阅被暂时冻结。

## 删除事件订阅

{{step-1-to-setup}}

1. 在左侧导航面板中，单击&#x200B;**系统**，然后单击&#x200B;**事件订阅**。
1. 选择要删除的事件订阅。
1. 单击&#x200B;**删除**。
