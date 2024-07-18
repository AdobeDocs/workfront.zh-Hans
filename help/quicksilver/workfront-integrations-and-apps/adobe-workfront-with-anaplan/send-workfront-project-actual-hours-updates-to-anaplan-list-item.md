---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 向 [!DNL Anaplan] 列表项发送 [!DNL Adobe Workfront] 实际小时更新
description: 此集成方案共享在具有 [!DNL Anaplan] 预算列表项的 [!DNL Adobe Workfront] 项目上捕获的实际小时详细信息。 共享此信息可让您更好地利用 [!DNL Anaplan] 提供的支出优化和财务分析。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 0%

---

# 将[!DNL Adobe Workfront]实际小时更新发送到[!DNL Anaplan]列表项

此集成方案共享在具有[!DNL Anaplan]预算列表项的[!DNL Adobe Workfront]项目上捕获的实际小时详细信息。 共享此信息可让您更好地利用[!DNL Anaplan]提供的支出优化和财务分析。

此场景模板提供过去3个月在活动项目上按项目、日期和角色记录的汇总小时列表。

>[!IMPORTANT]
>
>本文中的“营销活动”是指此方案所代表的营销活动用例，并且绝不会连接到[!DNL Workfront Fusion] Adobe Campaign连接器或[!DNL Workfront]中最近弃用的[!UICONTROL 营销活动]对象。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[！UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

&#42;&#42;有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 触发事件

此方案计划每15分钟执行一次。

## 预期[!DNL Workfront]配置

[!DNL Workfront]中必须具有下列内容才能使用此方案：

* [!DNL Workfront]中名为&#x200B;**[!UICONTROL Anaplan集成]**&#x200B;的用户配置文件，具有系统管理员权限。

  有关在[!DNL Workfront]中创建用户的信息，请参阅[添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 预期[!DNL Anaplan]配置

[!DNL Anaplan]中必须具有下列内容才能使用此方案：

* [!DNL Anaplan]中名为&#x200B;**[!UICONTROL [!DNL Workfront]集成]**&#x200B;的用户配置文件，具有系统管理员权限。
* 要用于此方案的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中要用于此方案的列表。
* [!DNL Anaplan]中名为&#x200B;**[!UICONTROL Anaplan实际小时数导入]**&#x200B;的文件，它包含以下列（按此顺序）：

   1. [!UICONTROL Workfront项目GUID]

   2. [!UICONTROL 小时]

   3. [!UICONTROL 小时估计成本]

   4. [!UICONTROL 输入日期]

   5. [!UICONTROL 角色名称]

   6. [!UICONTROL 促销活动名称]

   7. [!UICONTROL [!DNL Anaplan]列表项ID]

  要准备[!DNL Anaplan]实际费用报表文件：

   1. 将以下内容复制并粘贴到文本编辑器或[!DNL Excel]中
   1. 以CSV格式保存文件
   1. 将文件上载到[!DNL Anaplan]。

      有关说明，请参阅有关将数据从文件导入模块的[!DNL Anaplan]文档。

   1. 请记下您为文件提供的名称；该文件将在[!UICONTROL Fusion]方案模板的部署期间使用。

  示例CSV内容

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* 准备执行&#x200B;**[!UICONTROL 项目实际小时导入]**&#x200B;进程，以导入文件上传中传递的数据。

有关上述任何操作的说明，请参阅[!DNL Anaplan]文档。

## 部署到[!DNL Workfront Fusion]

完成以下步骤将此集成方案部署到您的[!DNL Fusion]帐户。 此操作只应在完成所需的[!DNL Workfront]和[!DNL Anaplan]配置之后完成。

1. 导航到[!DNL Workfront Fusion]中的[!UICONTROL 模板]菜单，然后单击&#x200B;**[!UICONTROL 将Workfront实际小时更新发送到[!DNL Anaplan]列表项]**&#x200B;方案模板。
1. 替换以下[!DNL Anaplan]个变量的变量值：

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>变量名称</th> 
      <th>替换值为</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[！UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>[!DNL Anaplan]帐户中的工作区ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL [!DNL Anaplan]模型ID] </td> 
      <td>[!DNL Anaplan]帐户和所选工作区的模型ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL营销活动列表名称]</td> 
      <td>您的[!DNL Anaplan]帐户和所选工作区和模型的列表名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL文件名：实际小时数导入]</td> 
      <td> <p>将接收项目实际小时数数据的文件的名称。</p> <p> （示例：WorkfrontUpdateLinkedProjects_HoursRoles.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL进程名称：实际小时数导入]</td> 
      <td> <p>将执行项目小时数据导入的进程的名称。</p> <p>（示例： WF Int — 按角色加载项目小时数）</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL [!DNL Workfront]子域]</td> 
      <td>[!DNL Workfront]帐户的子域。 这用于在可能生成的注释中创建指向[!DNL Workfront]项目的链接。</td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅[!DNL Anaplan]设置文档。

1. 选择或添加[!DNL Anaplan]连接配置文件。
1. 出现提示时，更新具有[!DNL Anaplan]连接的所有其余[!DNL Anaplan]模块。
1. 选择或添加[!DNL Workfront]连接配置文件。
1. 出现提示时，更新具有[!DNL Workfront]连接的所有其余[!DNL Workfront]模块。

## 其他建议的方案模板

此方案模板与以下支出优化方案模板相辅相成，这些模板也可部署：

* [[!UICONTROL 将 [!DNL Adobe Workfront] 项目更新发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 将 [!DNL Adobe Workfront] 费用发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

链接预算请求的其他方案：

* [[!UICONTROL 根据 [!DNL Adobe Workfront] 预算请求创建 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

关联营销活动请求的其他方案：

* [[!UICONTROL 根据 [!DNL Adobe Workfront] 营销活动请求创建 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 营销活动请求或营销活动项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
