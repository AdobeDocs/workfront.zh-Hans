---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 使用验证审批报告
description: 您可以使用验证审批报告查看有关您环境中验证的信息。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
TQID: https://experienceleague.adobe.com/ZU6Ej5QhI7v9zoAxurBz1YsFVIuVIh2a8tR2h6vYL18
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a2241fa21f51f8146c1f3725d2ba2235f8458ab4
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 5%

---

# 使用验证审批报告

您可以使用验证审批报告查看有关您环境中验证的信息。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront包</p> </td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront许可证</p> </td> 
   <td> 
   <p>标准</p>
   <p>规划</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>访问级别配置</strong> </td> 
   <td> <p>编辑以下项的访问权限：</p> 
    <ul> 
     <li> <p>创建报告、功能板和日历</p> </li> 
     <li> <p>创建筛选器、视图和分组</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 使用验证审批报告

{{step1-to-reports}}

1. 单击&#x200B;**新建报告**，然后滚动以选择&#x200B;**校对审批**。

   ![校对审批报告](assets/proof-approval-report.png)

1. （可选）添加任何其他字段。
1. 单击&#x200B;**保存+关闭**。

## 其他字段

您可以将以下字段添加到验证审批报告：

* **决策日期**：显示审批者对验证做出决策的日期。 您还可以在证明的打印摘要中找到此日期。
* **审批者阶段**：显示当前阶段信息。
* **工作流模板**：显示附加到验证的任何工作流模板。 如果没有附加模板，则该列为空。
* **等待决定**：当以下条件为true时，显示true表示最新版本未满足决定：

   * 校对未存档
   * 审批者所在的阶段处于活动状态
   * 验证正在等待审批

* **验证截止日期**：显示验证的截止日期。 每个阶段都必须分配有截止日期才能填充此字段。 字段显示最近激活阶段的截止日期。

## 关于批准者决策字段

审批者决策字段显示收件人对验证所做的决策。 在某些情况下，此字段显示连字符(-)而不是决策值，这表示收件人不再处于验证上的决策角色。 有关详细信息，请参阅[审批者决策在验证审批报告](../tips-tricks-and-troubleshooting/approver-decision-shows-hyphen.md)中显示一个连字符。

 
