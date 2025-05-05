---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 将 [!DNL Adobe Workfront] 费用发送到 [!DNL Anaplan] 列表项
description: 此集成方案共享来自具有 [!DNL Anaplan] 预算列表项的 [!DNL Adobe Workfront] 项目的费用相关详细信息。 共享此信息可让您更好地利用 [!DNL Anaplan] 提供的支出优化和财务分析。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# 将[!DNL Adobe Workfront]费用发送到[!DNL Anaplan]列表项

此集成方案共享来自具有[!DNL Anaplan]预算列表项的[!DNL Adobe Workfront]项目的费用相关详细信息。 共享此信息可让您更好地利用[!DNL Anaplan]提供的支出优化和财务分析。

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
   <td> <p>[!UICONTROL Pro]或更高版本</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[!UICONTROL 计划]，[!UICONTROL 工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 许可证**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

&#42;&#42;有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)

## 触发事件

此方案计划每15分钟执行一次。

## 预期[!DNL Workfront]配置

[!DNL Workfront]中必须具有下列内容才能使用此方案：

* [!DNL Workfront]中名为&#x200B;*[!UICONTROL *[!DNL Anaplan]集成]**的用户配置文件，具有系统管理员权限。

  有关在[!DNL Workfront]中创建用户的信息，请参阅[添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

* 一个&#x200B;**[!UICONTROL 促销活动摘要]**&#x200B;自定义表单附加到项目对象，用于存储您选择发送到[!DNL Anaplan]的自定义数据值。

  表单必须包含以下字段：

  | 字段名称 | 字段类型 |
  |---|---|
  | [!UICONTROL 上次传输日期] | 日期 |
  | [!UICONTROL 集成注释] | 段落文本字段 |

  有关创建自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 预期[!DNL Anaplan]配置

[!DNL Anaplan]中必须具有下列内容才能使用此方案：

* [!DNL Anaplan]中名为&#x200B;**[!UICONTROL [!DNL Workfront]集成]**&#x200B;的用户配置文件，具有系统管理员权限。
* 要用于此方案的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中要捕获营销活动预算的列表。
* 按此顺序包含以下列的&#x200B;**[!UICONTROL Anaplan实际费用导入]**&#x200B;文件：

   1. [!UICONTROL [!DNL Workfront]费用GUID]

   2. [!UICONTROL [!DNL Workfront]项目GUID]

   3. [!UICONTROL 实际数量]

   4. [!UICONTROL 描述]

   5. [!UICONTROL 费用类型]

   6. [!UICONTROL 生效日期]

   7. [!UICONTROL 促销活动名称]

   8. [!UICONTROL [!DNL Anaplan]列表项ID]

  要准备[!UICONTROL [!DNL Anaplan]实际费用导入]文件，请执行以下操作：

   1. 将以下内容复制并粘贴到文本编辑器或[!DNL Excel]中。
   1. 以CSV格式保存文件。
   1. 将文件上载到[!DNL Anaplan]。

      有关说明，请参阅有关将数据从文件导入模块的[!DNL Anaplan]文档。

   1. 请记下您为文件提供的名称；该文件将在[!UICONTROL Fusion]方案模板的部署期间使用。

  示例CSV内容

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* 按此顺序包含以下列的&#x200B;**[!UICONTROL [!DNL Anaplan]计划费用导入]**&#x200B;文件：

   1. [!UICONTROL [!DNL Workfront]费用GUID]

   2. [!UICONTROL [!DNL Workfront]项目GUID]

   3. [!UICONTROL 实际数量]

   4. [!UICONTROL 描述]

   5. [!UICONTROL 费用类型]

   6. [!UICONTROL 生效日期]

   7. [!UICONTROL 促销活动名称]

   8. [!UICONTROL [!DNL Anaplan]列表项ID]

  要准备[!UICONTROL [!DNL Anaplan]计划费用导入]文件，请执行以下操作：

   1. 将以下内容复制并粘贴到文本编辑器或[!DNL Excel]中
   1. 以CSV格式保存文件
   1. 将文件上传到Anaplan。

      有关说明，请参阅有关将数据从文件导入模块的[!DNL Anaplan]文档。

   1. 请记下您为文件提供的名称；该文件将在[!UICONTROL Fusion]方案模板的部署期间使用。

  示例CSV内容

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* 准备执行&#x200B;**[!UICONTROL 项目更新导入]**&#x200B;进程，以导入文件上传中传递的数据。

>[!NOTE]
>
>计划支出和实际支出有单独的导入文件，以便可以分别在计划支出和有效支出日期中单独报告它们。

有关上述任何操作的说明，请参阅[!DNL Anaplan]文档。

## 部署到[!DNL Fusion]

完成以下步骤将此集成方案部署到您的[!DNL Fusion]帐户。 此操作只应在完成所需的[!DNL Workfront]和[!DNL Anaplan]配置之后完成。

1. 导航到[!DNL Workfront Fusion]中的[!UICONTROL 模板]菜单，然后单击&#x200B;**[!UICONTROL 将Workfront费用更新发送到[!DNL Anaplan]列表项]**&#x200B;方案模板。
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>您要用于此方案的[!DNL Anaplan]帐户中的工作区ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan]模型ID] </td> 
      <td>[!DNL Anaplan]帐户中的模型ID以及要用于此方案的选定工作区。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 营销活动列表名称]</td> 
      <td>[!DNL Anaplan]帐户中的列表名称，以及要用于此方案的选定工作区和模型。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 文件名：实际费用导入]</td> 
      <td> <p>将接收项目实际费用数据的文件的名称。</p> <p> （示例：WorkfrontUpdateLinkedProjects_ActExpenses.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 文件名：计划费用导入]</td> 
      <td> <p>将接收项目计划费用数据的文件的名称。</p> <p> （示例：WorkfrontUpdateLinkedProjects_PlannedExpenses.csv） </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 进程名称：项目更新导入]</td> 
      <td> <p>将执行项目费用数据导入的进程的名称。</p> <p>（示例： WF Int — 加载项目费用）</p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅[!DNL Anaplan]设置文档。

1. 选择或添加[!DNL Anaplan]连接配置文件。
1. 出现提示时，更新具有[!DNL Anaplan]连接的所有其余[!DNL Anaplan]模块。
1. 选择或添加[!DNL Workfront]连接配置文件。
1. 出现提示时，更新具有[!DNL Workfront]连接的所有其余[!DNL Workfront]模块。
1. 在&#x200B;**[!UICONTROL 生成实际费用CSV]**&#x200B;模块中，添加新的数据结构以将项目属性映射到CSV列。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. 在&#x200B;**[!UICONTROL 生成计划费用CSV]**&#x200B;模块中，添加新的数据结构以将项目属性映射到CSV列。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## 其他建议的方案模板

此方案模板与以下支出优化方案模板相辅相成，这些模板也可部署：

* [[!UICONTROL 将 [!DNL Adobe Workfront] 项目更新发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 向 [!DNL Anaplan] 列表项]发送 [!DNL Adobe Workfront] 实际小时更新](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

链接预算请求的其他方案：

* [[!UICONTROL 根据 [!DNL Adobe Workfront] 预算请求创建 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

关联营销活动请求的其他方案：

* [[!UICONTROL 根据 [!DNL Adobe Workfront] 营销活动请求创建 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 营销活动请求或营销活动项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
