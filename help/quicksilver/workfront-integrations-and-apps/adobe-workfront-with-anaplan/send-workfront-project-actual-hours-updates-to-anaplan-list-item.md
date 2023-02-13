---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 发送 [!DNL Adobe Workfront] 实际小时更新到 [!DNL Anaplan] 列表项目
description: 此集成方案共享在 [!DNL Adobe Workfront] 项目 [!DNL Anaplan] 预算列表项。 通过共享此信息，您可以更好地利用 [!DNL Anaplan] 提供。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# 发送 [!DNL Adobe Workfront] 实际小时更新到 [!DNL Anaplan] 列表项目

此集成方案共享在 [!DNL Adobe Workfront] 项目 [!DNL Anaplan] 预算列表项。 通过共享此信息，您可以更好地利用 [!DNL Anaplan] 提供。

此方案模板提供了一个按项目、日期和角色汇总的小时列表，这些小时记录了过去3个月中活动项目中记录的小时数。

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

* 中的用户配置文件 [!DNL Workfront] 已命名 **[!UICONTROL Anaplan集成]**，具有系统管理员权限。

   有关在 [!DNL Workfront]，请参阅 [添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## 预期 [!DNL Anaplan] 配置

您必须在 [!DNL Anaplan] 要使用此方案，请执行以下操作：

* 中的用户配置文件 [!DNL Anaplan] 已命名 **[!UICONTROL [!DNL Workfront ]集成]**，具有系统管理员权限。
* 的 [!DNL Anaplan] 要用于此方案的模型。
* 中的列表 [!DNL Anaplan] 要用于此方案的模型。
* 文件 [!DNL Anaplan] 已命名 **[!UICONTROL Anaplan实际小时数导入]** 按此顺序包含以下列：

   1. [!UICONTROL Workfront项目GUID]

   2. [!UICONTROL 小时]

   3. [!UICONTROL 预计工时]

   4. [!UICONTROL 输入日期]

   5. [!UICONTROL 角色名称]

   6. [!UICONTROL 营销活动名称]

   7. [!UICONTROL [!DNL Anaplan] 列表项ID]
   准备 [!DNL Anaplan] 实际费用报表文件：

   1. 将以下内容复制并粘贴到文本编辑器中，或 [!DNL Excel]
   1. 以CSV格式保存文件
   1. 将文件上传到 [!DNL Anaplan].

      有关说明，请参阅 [!DNL Anaplan] 有关将数据从文件导入模块的文档。

   1. 记下您为文件提供的名称；它将在部署 [!UICONTROL Fusion] 方案模板。

   CSV内容示例

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL 项目实际工时导入]** 准备执行导入文件上传中传送的数据的进程。

有关这些操作中任何一项的说明，请参阅 [!DNL Anaplan] 文档。

## 部署到 [!DNL Workfront Fusion]

完成以下步骤，将此集成方案部署到 [!DNL Fusion] 帐户。 仅应在完成所需的 [!DNL Workfront] 和 [!DNL Anaplan] 配置。

1. 导航到 [!UICONTROL 模板] 菜单 [!DNL Workfront Fusion] ，然后单击 **[!UICONTROL 将Workfront实际小时数更新发送到 [!DNL Anaplan] 列表项目]** 方案模板。
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
      <td role="rowheader">[!UICONTROL文件名：实际导入小时数]</td> 
      <td> <p>将接收项目实际工时数据的文件的名称。</p> <p> (示例：WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL进程名称：实际导入小时数]</td> 
      <td> <p>执行导入项目小时数据的进程名称。</p> <p>(示例：WF整数 — 按角色加载项目小时数)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] 子域]</td> 
      <td>的子域 [!DNL Workfront] 帐户。 用于创建回您 [!DNL Workfront] 项目。</td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅 [!DNL Anaplan] 设置文档。

1. 选择或添加 [!DNL Anaplan] 连接配置文件。
1. 更新所有剩余 [!DNL Anaplan] 模块 [!DNL Anaplan] 连接时。
1. 选择或添加 [!DNL Workfront] 连接配置文件。
1. 更新所有剩余 [!DNL Workfront] 模块 [!DNL Workfront] 连接时。

## 其他推荐的方案模板

此方案模板由以下也可能部署的支出优化方案模板来补充：

* [[!UICONTROL 发送 [!DNL Adobe Workfront] 项目更新至 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 发送 [!DNL Adobe Workfront] 支出 [!DNL Anaplan] 列表项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

关联预算请求的其他方案：

* [[!UICONTROL 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 预算请求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

关联营销活动请求的其他方案：

* [[!UICONTROL 创建 [!DNL Anaplan] 列表项 [!DNL Adobe Workfront] 营销活动请求]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 应用 [!DNL Anaplan] 预算分配到 [!DNL Adobe Workfront] 营销活动请求或营销活动项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
