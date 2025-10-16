---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 项目
description: 此集成方案将已在 [!DNL Anaplan] 内进行的预算分配同步回 [!DNL Workfront]。 此方案会提取所有链接的营销活动预算项，如果预算值已更改，则将预算值传递到链接的Workfront项目。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: d3f234313677d916318c181c91cb951948454006
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 0%

---

# 将[!DNL Anaplan]预算分配应用于[!DNL Adobe Workfront]项目

此集成方案将已在[!DNL Anaplan]中进行的所有预算分配同步回[!DNL Workfront]。 方案提取所有链接的营销活动预算项，如果预算值已更改，则将预算值传递到链接的[!DNL Workfront]项目。

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

* [!DNL Workfront]中名为&#x200B;**Anaplan集成**&#x200B;的用户配置文件，具有系统管理员权限。

  有关在[!DNL Workfront]中创建用户的信息，请参阅[添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

## 预期[!DNL Anaplan]配置

[!DNL Anaplan]中必须具有下列内容才能使用此方案：

* [!DNL Anaplan]中名为&#x200B;**[!DNL Workfront]集成**&#x200B;的用户配置文件，具有系统管理员权限。
* 要用于此方案的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中捕获营销活动预算的列表。

  列表的模块必须支持接收以下属性：

   * [!UICONTROL Workfront项目GUID]
   * [!UICONTROL 促销活动名称]
   * [!UICONTROL 已请求劳力资金]
   * [!UICONTROL 预计收入]
   * [!UICONTROL 品牌]

  此列表和模块必须存储[!DNL Anaplan]正常功能所需的其他详细信息，包括设置预算并告知预算列表项已准备好同步回[!DNL Workfront]的功能。

* 在Adobe Workfront[!DNL Anaplan]中名为&#x200B;**[!UICONTROL Campaigns.Update Campaigns的]**&#x200B;中的视图。

  此视图必须按以下顺序包含以下列：

   1. [!UICONTROL 项目名称]

   2. [!UICONTROL [!DNL Workfront]项目GUID]

   3. [!UICONTROL 促销活动名称]

   4. [!UICONTROL 预算]

   5. [!UICONTROL 预计收入]

   6. [!UICONTROL 品牌]

  应筛选该视图，以显示具有[!UICONTROL [!DNL Workfront]项目GUID]的项以及预算分配应传输到[!DNL Workfront]的某些指示符。

有关上述任何操作的说明，请参阅[!DNL Anaplan]文档。

## 部署到[!DNL Workfront Fusion]

完成以下步骤将此集成方案部署到您的[!DNL Fusion]帐户。 此操作只应在完成所需的[!DNL Workfront]和[!DNL Anaplan]配置之后完成。

1. 导航到[!UICONTROL 中的]模板[!DNL Workfront Fusion]菜单，然后单击&#x200B;**[!UICONTROL 将[!DNL Anaplan]预算分配应用于Workfront项目]**&#x200B;方案模板。
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
      <td role="rowheader">[！UICONTROL [!DNL Anaplan]模块名称]</td> 
      <td>描述选定[!DNL Anaplan]列表中的促销活动属性的模块名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL营销活动列表名称]</td> 
      <td>您的[!DNL Anaplan]帐户和所选工作区和模型的列表名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[！UICONTROL [!DNL Anaplan]视图名称]</td> 
      <td> <p>包含可传输到[!DNL Workfront]的营销活动预算的视图的名称。</p> <p>（示例：[！UICONTROL Campaigns.Load Campaigns.To [!DNL Adobe Workfront]]） </p> </td> 
     </tr> 
    </tbody> 
   </table>

   有关如何设置文件和进程的详细信息，请参阅[!DNL Anaplan]设置文档。

1. 选择或添加[!DNL Anaplan]连接配置文件。
1. 出现提示时，更新具有[!DNL Anaplan]连接的所有其余[!DNL Anaplan]模块。
1. 在&#x200B;**[!UICONTROL 将CSV转换为JSON对象模块]**&#x200B;中，添加新的数据结构以将CSV列映射到可用的JSON对象。

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. 出现提示时，为此场景部署中的其他模块选择此数据结构。
1. 在&#x200B;**[!UICONTROL 检查链接的项目]**&#x200B;模块上，选择或添加[!DNL Workfront]连接配置文件。
1. 出现提示时，更新具有[!DNL Workfront]连接的所有其余[!DNL Workfront]模块。

## 其他建议的方案模板

要完成此模板表示的工作流，您还必须部署以下附加模板：

* [[!UICONTROL 根据 [!DNL Anaplan] 预算请求创建 [!DNL Adobe Workfront] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

支出优化的其他方案包括：

* [[!UICONTROL 将 [!DNL Adobe Workfront] 项目更新发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL 向 [!DNL Adobe Workfront] 列表项 [!DNL Anaplan] 发送]实际小时更新](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL 将 [!DNL Adobe Workfront] 费用发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
