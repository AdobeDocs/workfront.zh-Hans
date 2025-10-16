---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 将 [!DNL Adobe Workfront] 项目更新发送到 [!DNL Anaplan] 列表项
description: 此集成方案共享具有 [!DNL Adobe Workfront] 预算列表项的 [!DNL Anaplan] 项目的进度、状态和关键计划详细信息。 共享此信息可让您更好地利用 [!DNL Anaplan] 提供的支出优化和财务分析。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# 将[!DNL Adobe Workfront]项目更新发送到[!DNL Anaplan]列表项

此集成方案共享具有[!DNL Adobe Workfront]预算列表项的[!DNL Anaplan]项目的进度、状态和关键计划详细信息。 共享此信息可让您更好地利用[!DNL Anaplan]提供的支出优化和财务分析。

>[!IMPORTANT]
>
>本文中的“营销活动”是指此方案所代表的营销活动用例，并且绝不会连接到[!DNL Workfront Fusion] Adobe Campaign连接器或[!UICONTROL 中最近弃用的]营销活动[!DNL Workfront]对象。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront包</td> 
   <td> <p>任何Adobe Workfront Workflow包和任何Adobe Workfront自动化和集成包</p><p>Workfront Ultimate</p><p>Workfront Prime和Select包，以及额外购买的Workfront Fusion。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>标准</p><p>工作或更高</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion许可证</td> 
   <td>
   <p>基于操作：不需要Workfront Fusion许可证</p>
   <p>基于连接器（旧版）：用于工作自动化和集成的Workfront Fusion </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>如果贵组织具有不包含Workfront Automation and Integration的Select或Prime Workfront包，则贵组织必须购买Adobe Workfront Fusion。</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅文档[中的](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)访问要求。

有关Adobe Workfront Fusion许可证的信息，请参阅[Adobe Workfront Fusion许可证](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration)。

## 触发事件

此方案计划每15分钟执行一次。

## 预期[!DNL Workfront]配置

[!DNL Workfront]中必须具有下列内容才能使用此方案：

* [!DNL Workfront]中名为&#x200B;**[!UICONTROL [!DNL Anaplan]集成]**&#x200B;的用户配置文件，具有系统管理员权限。

  有关在[!DNL Workfront]中创建用户的信息，请参阅[添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

* 附加到项目对象的&#x200B;**[!UICONTROL 促销活动简报]**&#x200B;自定义表单，用于存储您选择发送到Anaplan的自定义数据值。

  以下字段表示自定义表单中可包含的字段示例，用于帮助将数据映射到Anaplan，但此集成方案不需要这些字段：

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
     <td role="rowheader">[!UICONTROL 上市日期]</td> 
     <td>[!UICONTROL 日期] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 市场结束日期]</td> 
     <td>[!UICONTROL 日期]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 营销活动概述]</td> 
     <td>[!UICONTROL 段落文本字段]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL 段落文本字段]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL 目标受众]</td> 
     <td> <p>[!UICONTROL 下拉列表]</p> <p>包含适合您的流程的选项。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  有关创建自定义表单的信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## 预期[!DNL Anaplan]配置

[!DNL Anaplan]中必须具有下列内容才能使用此方案：

* [!DNL Anaplan]中名为&#x200B;**[!UICONTROL [!DNL Workfront]集成]**&#x200B;的用户配置文件，具有系统管理员权限。
* 要用于此方案的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中要用于此方案的列表。
* 包含下列列的&#x200B;**[!UICONTROL 项目更新导入]**&#x200B;文件（按此顺序）：

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront]项目GUID]

3. [!UICONTROL 促销活动名称]

4. 已完成[!UICONTROL 百分比]

5. [!UICONTROL 计划开始日期]

6. [!UICONTROL 计划完成日期]

7. [!UICONTROL 计划小时数]

8. [!UICONTROL 计划成本]

9. [!UICONTROL 计划费用成本]

10. [!UICONTROL 实际劳力成本]

11. [!UICONTROL 计划劳力成本]

12. [!UICONTROL 状态]

要准备[!UICONTROL [!DNL Anaplan]计划费用导入]文件，请执行以下操作：

1. 将以下内容复制并粘贴到文本编辑器或[!DNL Excel]中
1. 以CSV格式保存文件
1. 将文件上传到Anaplan。

   有关说明，请参阅有关将数据从文件导入模块的[!DNL Anaplan]文档。

1. 请记下您为文件提供的名称；该文件将在[!UICONTROL Fusion]方案模板的部署期间使用。

示例CSV内容

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>可选列可能包括：

1. [!UICONTROL 促销活动概述]

2. [!UICONTROL 关键消息]

3. [!UICONTROL 上市日期]

4. [!UICONTROL 市场结束日期]

5. [!UICONTROL 目标受众]

还包括在映射中要设置的任何其他字段。

* 准备执行&#x200B;**[!UICONTROL 项目更新导入]**&#x200B;进程，以导入文件上传中传递的数据。

有关上述任何操作的说明，请参阅[!DNL Anaplan]文档。

## 部署到[!DNL Workfront Fusion]

完成以下步骤可将此集成方案部署到您的Fusion帐户。 此操作只应在完成所需的[!DNL Workfront]和[!DNL Anaplan]配置之后完成。

1. 导航到[!UICONTROL 中的]模板[!DNL Workfront Fusion]菜单，然后单击&#x200B;**[!UICONTROL 将Workfront项目更新发送到[!DNL Anaplan]列表项]**&#x200B;方案模板。
1. 替换以下[!DNL Anaplan]个变量的变量值：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>变量名称</th> 
      <th>替换值为</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>[!DNL Anaplan]帐户中的工作区ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan]模型ID] </td> 
      <td>[!DNL Anaplan]帐户和所选工作区的模型ID。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 营销活动列表名称]</td> 
      <td>您的[!DNL Anaplan]帐户和所选工作区和模型的列表名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 文件名：项目更新导入]</td> 
      <td>将接收项目更新数据的文件的名称。<p>（示例：WorkfrontUpdateLinkedProject.csv）</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 进程名称：项目更新导入]</td> 
      <td> <p>执行项目数据导入的进程的名称。</p> <p>（示例： WF Int — 更新促销活动详细信息）</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront]子域]</td> 
      <td>[!DNL Workfront]帐户的子域。 这用于在可能生成的注释中创建指向[!DNL Workfront]项目的链接。</td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅[!DNL Anaplan]设置文档。

1. 选择或添加[!DNL Anaplan]连接配置文件。
1. 出现提示时，更新具有[!DNL Anaplan]连接的所有其余[!DNL Anaplan]模块。
1. 选择或添加[!DNL Workfront]连接配置文件。

   该过滤器配置为纳入所有未完成的链接项目和过去29分钟内完成的项目。 如果更改[!DNL Fusion]方案的频率，则要在部署方案模板后更新此值。

1. 在&#x200B;**[!UICONTROL 生成项目更新CSV]**&#x200B;模块上，添加新的数据结构以将项目属性映射到CSV列。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. 出现提示时，更新具有[!DNL Workfront]连接的所有其余[!DNL Workfront]模块。

## 其他建议的方案模板

此方案模板与以下支出优化方案模板相辅相成，这些模板也可部署：

* [[!UICONTROL 向 [!DNL Adobe Workfront] 列表项 [!DNL Anaplan] 发送]实际小时更新](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 将 [!DNL Adobe Workfront] 费用发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

链接预算请求的其他方案：

* [[!UICONTROL 根据 [!DNL Anaplan] 预算请求创建 [!DNL Adobe Workfront] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

关联营销活动请求的其他方案：

* [[!UICONTROL 根据 [!DNL Anaplan] 营销活动请求创建 [!DNL Adobe Workfront] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 营销活动请求或营销活动项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
