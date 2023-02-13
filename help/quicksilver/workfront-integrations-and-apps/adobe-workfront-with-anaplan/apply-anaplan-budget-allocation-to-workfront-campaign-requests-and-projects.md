---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 营销活动请求或营销活动项目
description: 此集成方案会同步在 [!DNL Anaplan] 返回 [!DNL Workfront]. 方案会提取所有关联的促销活动预算项，然后在预算值发生更改时将预算值传递到关联的Workfront项目。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 8ae28911-fa18-459a-aa50-cfb347e70e61
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 营销活动请求或营销活动项目

此集成方案会同步在 [!DNL Anaplan] 返回 [!DNL Workfront]. 方案会提取所有关联的营销活动预算项目，然后将预算值传递到关联的 [!DNL Workfront] 项目。

>[!IMPORTANT]
>
>本文中的“营销活动”是指此方案表示的营销活动用例，并且与 [!DNL Workfront Fusion] Adobe Campaign连接器或最近弃用的 [!UICONTROL Campaign] 对象 [!DNL Workfront].


## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

&#42;&#42;有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 触发事件

此方案计划每15分钟执行一次。

## 预期 [!DNL Workfront] 配置

您必须在 [!DNL Workfront] 要使用此方案，请执行以下操作：

* 中的用户配置文件 [!DNL Workfront] 已命名 **[!DNL Anaplan Integration]**，具有系统管理员权限。

   有关在 [!DNL Workfront]，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 预期 [!DNL Anaplan] 配置

您必须在 [!DNL Anaplan] 要使用此方案，请执行以下操作：

* 中的用户配置文件 [!DNL Anaplan] 已命名 **[!UICONTROL [!DNL Workfront]集成]**，具有系统管理员权限。
* 的 [!DNL Anaplan] 要用于此方案的模型。
* 中的列表 [!DNL Anaplan] 捕捉促销活动预算的模型。

   列表的模块必须支持接收以下属性：

   * [!UICONTROL [!DNL Workfront] 请求GUID]
   * [!UICONTROL [!DNL Workfront] 项目GUID]
   * [!UICONTROL 营销活动名称]
   * [!UICONTROL 所申请的劳动基金]
   * [!UICONTROL 预计收入]
   * [!UICONTROL 品牌]

   此列表和模块必须存储其他详细信息，这些详细信息是正常功能所必需的 [!DNL Anaplan]，包括能够设置预算并告知预算列表项已准备好同步回 [!DNL Workfront].

* 中的视图 [!DNL Anaplan] 调用 **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**.

   此视图必须按以下顺序包含以下列：

   1. [!UICONTROL 项目名称]

   2. [!UICONTROL [!DNL Workfront] 请求GUID]

   3. [!UICONTROL [!DNL Workfront] 项目GUID]

   4. [!UICONTROL 营销活动名称]

   5. [!UICONTROL 预算]

   6. [!UICONTROL 预计收入]

   7. [!UICONTROL 品牌]
   应筛选视图以显示具有 [!UICONTROL [!DNL Workfront] 项目GUID] 一些指标表明应将预算拨款转交Workfront。

有关这些操作中任何一项的说明，请参阅 [!DNL Anaplan] 文档。

## 部署到Workfront Fusion

完成以下步骤以将此集成方案部署到您的Fusion帐户。 仅应在完成所需的 [!DNL Workfront] 和 [!DNL Anaplan] 配置。

1. 导航到 [!UICONTROL 模板] 菜单 [!DNL Workfront Fusion] ，然后单击 **[!UICONTROL 应用 [!DNL Anaplan] 预算分配给Workfront促销活动请求和项目]** 方案模板。
1. 替换以下变量值 [!DNL Anaplan] 变量：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>变量名称</th> 
      <th>将值替换为</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 工作区ID]</td> 
      <td>工作区的ID，来自 [!DNL Anaplan] 帐户。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 模型ID] </td> 
      <td>您的 [!DNL Anaplan] 帐户和选定的工作区。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL营销活动列表名称]</td> 
      <td>您的 [!DNL Anaplan] 帐户和选定的工作区和模型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] 视图名称]</td> 
      <td> <p>包含已准备好传输到的营销活动预算的视图的名称 [!DNL Workfront].</p> <p>(示例：[!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅 [!DNL Anaplan] 设置文档。

1. 选择或添加 [!DNL Anaplan] 连接配置文件。
1. 更新所有剩余 [!DNL Anaplan] 模块 [!DNL Anaplan] 连接时。
1. 在 **[!UICONTROL 将CSV转换为JSON对象]** 模块中，添加一个新的数据结构，以将CSV列映射到可用的JSON对象。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 出现提示时，为此方案部署中的其他模块选择此数据结构。
1. 在 **[!UICONTROL 检查链接的项目]** 模块，选择或添加 [!DNL Workfront] 连接配置文件。
1. 更新所有剩余 [!DNL Workfront] 模块 [!DNL Workfront] 连接时。

## 其他推荐的方案模板

要完成此模板表示的工作流，您还必须部署以下其他模板：

* [[!UICONTROL 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 营销活动请求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)

支出优化的其他方案包括：

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 项目更新至 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 实际小时更新到 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 支出 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
