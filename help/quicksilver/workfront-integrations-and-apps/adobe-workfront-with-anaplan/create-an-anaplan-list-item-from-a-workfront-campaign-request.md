---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 营销活动请求
description: 此集成方案将链接 [!DNL Adobe Workfront] 项目 [!DNL Anaplan] 预算列表项。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 2%

---

# 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 营销活动请求

此集成方案将链接 [!DNL Adobe Workfront] 项目 [!DNL Anaplan] 预算列表项。

此方案会监视添加到请求队列的新促销活动请求。 一旦记录了促销活动请求，则会在 [!DNL Anaplan] 启动资金流程。

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
   <td role="rowheader">[!UICONTROL Adobe Workfront]计划*</td> 
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

* 中的用户配置文件 [!DNL Workfront] 已命名 **[!UICONTROL [!DNL Anaplan]集成]**，具有系统管理员权限。

   有关在 [!DNL Workfront]，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 营销活动摘要]** 附加到的自定义表单 [!UICONTROL 请求] 对象。

   自定义表单中必须包含以下必填字段，以帮助将数据映射到Anaplan:

   | 字段名称 | 字段类型 |
   |---|---|
   | [!UICONTROL 所请求资金共计] |  |
   | [!UICONTROL 所申请的劳动基金] |  |
   | [!UICONTROL 请求的费用基金] |  |
   | [!UICONTROL 发送至 [!DNL Anaplan]] | 复选框 |

   表单上可能存在以下可选字段。 此方案仅映射上述字段，但营销活动摘要中的任何其他字段均可映射。

   <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>字段名称</th> 
     <th>字段类型</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[！市场开始日期中的UICONTROL]</td> 
     <td>日期 </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!Uicontrol In Market End Date]</td> 
     <td>日期</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign概述]</td> 
     <td>段落文本字段</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL密钥消息]</td> 
     <td>段落文本字段</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target受众]</td> 
     <td> <p>下拉</p> <p>包括适合您的流程的选项。</p> </td> 
    </tr> 
   </tbody> 
  </table>

   有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* 设置为请求队列以捕获新促销活动请求的项目。 的 [!UICONTROL 营销活动摘要] 表单必须附加到这些请求。

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
   * [!UICONTROL 请求的费用基金]
   * [!UICONTROL 预算请求类型]

   此列表和模块必须存储其他详细信息，这些详细信息是正常功能所必需的 [!DNL Anaplan]，包括能够设置预算并告知预算列表项已准备好同步回 [!DNL Workfront].

有关这些操作中任何一项的说明，请参阅 [!DNL Anaplan] 文档。

## 部署到 [!DNL Workfront Fusion]

完成以下步骤，将此集成方案部署到 [!DNL Fusion] 帐户。 仅应在完成所需的 [!DNL Workfront] 和 [!DNL Anaplan] 配置。

1. 导航到 [!UICONTROL 模板] 菜单 [!DNL Workfront Fusion] ，然后单击 **[!UICONTROL 创建 [!DNL Anaplan] Workfront促销活动请求中的列表项]** 方案模板。
1. 替换以下变量值 [!DNL Anaplan] 变量：

   | 变量名称 | 将值替换为 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] 工作区ID] | 工作区的ID，来自 [!DNL Anaplan] 帐户。 |
   | [!UICONTROL [!DNL Anaplan] 模型ID] | 您的 [!DNL Anaplan] 帐户和选定的工作区。 |
   | [!UICONTROL [!DNL Anaplan] 模块名称] | 描述所选促销活动属性的模块的名称 [!DNL Anaplan] 列表。 |
   | [!UICONTROL 营销活动列表名称] | 您的 [!DNL Anaplan] 帐户和选定的工作区和模型。 |

   {style=&quot;table-layout:auto&quot;}

   有关如何设置文件和进程的详细信息，请参阅 [!DNL Anaplan] 设置文档。

1. 选择或添加 [!DNL Anaplan] 连接配置文件。
1. 更新所有剩余 [!DNL Anaplan] 模块 [!DNL Anaplan] 连接时。
1. 选择或添加 [!DNL Workfront] 连接配置文件。

   部署模板后，如果要将默认映射的字段更改为 [!DNL Anaplan].

1. 更新所有剩余 [!DNL Workfront] 模块 [!DNL Workfront] 连接时。

## 其他推荐的方案模板

要完成此模板表示的工作流，您还必须部署以下其他模板：

* [[!UICONTROL 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 营销活动请求或营销活动项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

支出优化的其他方案包括：

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 项目更新至 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 实际小时更新到 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 支出 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
