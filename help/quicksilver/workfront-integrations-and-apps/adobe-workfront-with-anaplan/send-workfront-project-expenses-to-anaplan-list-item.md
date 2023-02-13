---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 发送 [!DNL Adobe Workfront] 支出 [!DNL Anaplan] 列表项目
description: 此集成方案共享与费用相关的详细信息，具体来自 [!DNL Adobe Workfront] 项目 [!DNL Anaplan] 预算列表项。 通过共享此信息，您可以更好地利用 [!DNL Anaplan] 提供。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 2%

---

# 发送 [!DNL Adobe Workfront] 支出 [!DNL Anaplan] 列表项目

此集成方案共享与费用相关的详细信息，具体来自 [!DNL Adobe Workfront] 项目 [!DNL Anaplan] 预算列表项。 通过共享此信息，您可以更好地利用 [!DNL Anaplan] 提供。

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
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

* 中的用户配置文件 [!DNL Workfront] name *[!UICONTROL *[!DNL Anaplan] 集成]**，具有系统管理员权限。

   有关在 [!DNL Workfront]，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL 营销活动摘要]** 附加到项目对象的自定义表单，用于存储您选择要发送到的自定义数据值 [!DNL Anaplan].

   表单必须包含以下字段：

   | 字段名称 | 字段类型 |
   |---|---|
   | [!UICONTROL 上次传输日期] | 日期 |
   | [!UICONTROL 集成说明] | 段落文本字段 |

   有关创建自定义表单的信息，请参阅 [创建或编辑自定义表单](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## 预期 [!DNL Anaplan] 配置

您必须在 [!DNL Anaplan] 要使用此方案，请执行以下操作：

* 中的用户配置文件 [!DNL Anaplan] 已命名 **[!UICONTROL [!DNL Workfront ]集成]**，具有系统管理员权限。
* 的 [!DNL Anaplan] 要用于此方案的模型。
* 中的列表 [!DNL Anaplan] 您希望捕获营销活动预算的模型。
* 安 **[!UICONTROL Anaplan实际费用导入]** 文件，其中按以下顺序包含以下列：

   1. [!UICONTROL [!DNL Workfront] 费用GUID]

   2. [!UICONTROL [!DNL Workfront] 项目GUID]

   3. [!UICONTROL 实际数量]

   4. [!UICONTROL 描述]

   5. [!UICONTROL 费用类型]

   6. [!UICONTROL 生效日期]

   7. [!UICONTROL 营销活动名称]

   8. [!UICONTROL [!DNL Anaplan] 列表项ID]
   准备 [!UICONTROL [!DNL Anaplan] 实际费用导入] 文件：

   1. 将以下内容复制并粘贴到文本编辑器中，或 [!DNL Excel].
   1. 以CSV格式保存文件。
   1. 将文件上传到 [!DNL Anaplan].

      有关说明，请参阅 [!DNL Anaplan] 有关将数据从文件导入模块的文档。

   1. 记下您为文件提供的名称；它将在部署 [!UICONTROL Fusion] 方案模板。

   CSV内容示例

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* 安 **[!UICONTROL [!DNL Anaplan]计划费用导入]** 文件，其中按以下顺序包含以下列：

   1. [!UICONTROL [!DNL Workfront] 费用GUID]

   2. [!UICONTROL [!DNL Workfront] 项目GUID]

   3. [!UICONTROL 实际数量]

   4. [!UICONTROL 描述]

   5. [!UICONTROL 费用类型]

   6. [!UICONTROL 生效日期]

   7. [!UICONTROL 营销活动名称]

   8. [!UICONTROL [!DNL Anaplan] 列表项ID]
   准备 [!UICONTROL [!DNL Anaplan] 计划费用导入] 文件：

   1. 将以下内容复制并粘贴到文本编辑器中，或 [!DNL Excel]
   1. 以CSV格式保存文件
   1. 将文件上传到Anaplan。

      有关说明，请参阅 [!DNL Anaplan] 有关将数据从文件导入模块的文档。

   1. 记下您为文件提供的名称；它将在部署 [!UICONTROL Fusion] 方案模板。

   CSV内容示例

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>


* A **[!UICONTROL 项目更新导入]** 准备执行导入文件上传中传送的数据的进程。

>[!NOTE]
>
>计划费用和实际费用有单独的导入文件，因此可以分别在计划日期和有效日期单独报告这些费用。

有关这些操作中任何一项的说明，请参阅 [!DNL Anaplan] 文档。

## 部署到 [!DNL Fusion]

完成以下步骤，将此集成方案部署到 [!DNL Fusion] 帐户。 仅应在完成所需的 [!DNL Workfront] 和 [!DNL Anaplan] 配置。

1. 导航到 [!UICONTROL 模板] 菜单 [!DNL Workfront Fusion] ，然后单击 **[!UICONTROL 将Workfront费用更新发送到 [!DNL Anaplan] 列表项目]** 方案模板。
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
      <td>您的 [!DNL Anaplan] 帐户和要用于此方案的选定工作区。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL营销活动列表名称]</td> 
      <td>您的 [!DNL Anaplan] 帐户以及要用于此方案的选定工作区和模型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL文件名：实际费用导入]</td> 
      <td> <p>接收项目实际支出数据的文件的名称。</p> <p> (示例：WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL文件名：计划费用导入]</td> 
      <td> <p>接收项目计划费用数据的文件的名称。</p> <p> (示例：WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL进程名称：项目更新导入]</td> 
      <td> <p>将执行导入项目费用数据的流程的名称。</p> <p>(示例：WF Int — 加载项目费用)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅 [!DNL Anaplan] 设置文档。

1. 选择或添加 [!DNL Anaplan] 连接配置文件。
1. 更新所有剩余 [!DNL Anaplan] 模块 [!DNL Anaplan] 连接时。
1. 选择或添加 [!DNL Workfront] 连接配置文件。
1. 更新所有剩余 [!DNL Workfront] 模块 [!DNL Workfront] 连接时。
1. 在 **[!UICONTROL 构建实际费用CSV]** 模块中，添加新的数据结构，以将项目属性映射到CSV列。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. 在 **[!UICONTROL 构建计划费用CSV]** 模块中，添加新的数据结构，以将项目属性映射到CSV列。

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

## 其他推荐的方案模板

此方案模板由以下也可能部署的支出优化方案模板来补充：

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 项目更新至 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 发送 [!DNL Adobe Workfront] 实际小时更新到 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

关联预算请求的其他方案：

* [[!UICONTROL 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 预算请求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

关联营销活动请求的其他方案：

* [[!UICONTROL 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 营销活动请求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 营销活动请求或营销活动项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
