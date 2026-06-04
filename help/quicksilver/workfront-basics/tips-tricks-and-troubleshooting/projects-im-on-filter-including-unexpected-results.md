---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: 我参与的项目过滤器包括意外结果
description: 阅读本文以对我的项目过滤器进行故障排除，包括意外结果。
feature: Get Started with Workfront
author: Alina
exl-id: 4701464a-4cf5-4be1-bcc0-0892019986ec
TQID: https://experienceleague.adobe.com/xE5RW947MUFg5d2X6ikKhHSftQDUMxDJlC05un0oDH0
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 180
ht-degree: 13%

---

# 我在处理的项目过滤器包括意外结果

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table>
  <tr>
   <td>Adobe Workfront 包
   </td>
   <td>“任一”</td>
  </tr>
  <tr>
   <td>Adobe Workfront 许可证
   </td>
   <td><p>标准</p>
   <p>规划</p>
   </td>
  </tr>
   <tr>
   <td>访问级别配置
   </td>
   <td>您必须是[!DNL Workfront]管理员。
   </td>
  </tr>
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++


## 问题

我所参与的&#x200B;[!UICONTROL **项目**]&#x200B;筛选器包含我无法预料的结果，因为我没有被分配这些项目或与其关联。

## 解决方案

[!UICONTROL **我参与的项目**]&#x200B;过滤器包括的项目包含位于其任何&#x200B;[!UICONTROL **项目详细信息**]&#x200B;字段中的用户的项目，其中包括容易错过或自动填写的字段，如&#x200B;[!UICONTROL **输入者**]&#x200B;或&#x200B;[!UICONTROL **发起人ID**]。 要删除不需要的结果，有两种可能的解决方案：

1. 检查筛选器包含的每个意外项目的&#x200B;[!UICONTROL **项目详细信息**]，并从所有字段中移除您的名称。

   或者

1. 尝试使用类似的过滤器，如&#x200B;[!UICONTROL **我拥有的项目**]，它仅包括专门分配给您的项目。

有关在[!DNL Workfront]中使用筛选器的更多信息，请参阅[筛选器概述](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md)。
