---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 根据 [!DNL Adobe Workfront] 预算请求创建 [!DNL Anaplan] 列表项
description: 此集成方案将 [!DNL Adobe Workfront] 项目（营销活动）与 [!DNL Anaplan] 预算列表项链接。 通过将预算请求添加到需要获得资金的 [!DNL Workfront] 项目来实现此目的。 此方案监视未处理的预算请求，然后执行在 [!DNL Anaplan] 中创建空预算列表项的进程，以在Anaplan中启动预算分配进程。
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# 根据[!DNL Adobe Workfront]预算请求创建[!DNL Anaplan]列表项

此集成方案将一个[!DNL Adobe Workfront]项目（营销活动）与一个[!DNL Anaplan]预算列表项链接。 这是通过将预算请求添加到需要获得资金的[!DNL Workfront]项目来实现的。 此方案监视未处理的预算请求，然后执行一个进程以在[!DNL Anaplan]中创建空预算列表项以在[!DNL Anaplan]中启动预算分配进程。

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
   <td> <p>[！UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</td> 
  </tr>
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

&#42;&#42;有关[!DNL  Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 触发事件

此方案计划每15分钟执行一次。

## 预期[!DNL Workfront]配置

[!DNL Workfront]中必须具有下列内容才能使用此方案：

* [!DNL Workfront]中名为*[!UICONTROL *[!DNL Anaplan]集成]**的用户配置文件，具有系统管理员权限。

  有关在[!DNL Workfront]中创建用户的信息，请参阅[添加用户](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)。

* **[!UICONTROL 预算请求]**&#x200B;自定义表单附加到[!UICONTROL 请求]对象。

  自定义表单上必须包括以下必填字段，以帮助将数据映射到[!DNL Anaplan]：

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>字段名称</th> 
     <th>字段类型</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[！UICONTROL预算请求类型]</td> 
     <td> <p>[！UICONTROL下拉列表]</p> <p>选项：</p> 
      <ul> 
       <li> <p>[！UICONTROL资金调整]</p> </li> 
       <li> <p>[！UICONTROL初始融资]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL Requested Labor Funds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL申请费用基金]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  有关创建自定义表单的信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

* 代表需要资金的营销活动和其他项目的项目模板，配置了[!UICONTROL 预算请求]队列主题。 已分配[!UICONTROL 预算请求]队列主题以使用[!UICONTROL 预算请求]自定义表单。
* 项目对象的&#x200B;**[!UICONTROL 营销活动简报]**&#x200B;表单。

  此表单必须包含以下字段：

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>字段名称</th> 
     <th>字段类型</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[！UICONTROL上市日期]</td> 
     <td>[！UICONTROL日期] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL市场结束日期]</td> 
     <td>[！UICONTROL日期]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL营销活动概述]</td> 
     <td>[！UICONTROL富文本字段]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL Key Message]</td> 
     <td>[！UICONTROL富文本字段]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[！UICONTROL目标受众]</td> 
     <td> <p>[！UICONTROL下拉列表]</p> <p>包含适合您的流程的选项。</p> </td> 
    </tr> 
   </tbody> 
  </table>

  有关创建自定义表单的信息，请参阅[使用表单设计器设计表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 预期[!DNL Anaplan]配置

[!DNL Anaplan]中必须具有下列内容才能使用此方案：

* [!DNL Anaplan]中名为&#x200B;**[!UICONTROL [!DNL Workfront]集成]**&#x200B;的用户配置文件，具有系统管理员权限。
* 要用于此方案的[!DNL Anaplan]模型。
* [!DNL Anaplan]模型中捕获营销活动预算的列表。

  列表的模块必须支持接收以下属性：

   * [!UICONTROL Workfront项目GUID]
   * [!UICONTROL 促销活动名称]
   * [!UICONTROL 已请求劳力资金]
   * [!UICONTROL 已申请费用资金]
   * [!UICONTROL 预算请求类型]
   * [!UICONTROL 资金调整原因]

  此列表和模块必须存储[!DNL Anaplan]正常功能所需的其他详细信息，包括设置预算并告知预算列表项已准备好同步回[!DNL Workfront]的功能。

有关上述任何操作的说明，请参阅[!DNL Anaplan]文档。

## 部署到[!DNL Workfront Fusion]

完成以下步骤将此集成方案部署到您的[!DNL Fusion]帐户。 此操作只应在完成所需的[!DNL Workfront]和[!DNL Anaplan]配置之后完成。

1. 导航到[!DNL Workfront Fusion]中的[!UICONTROL 模板]菜单，然后单击&#x200B;**[!UICONTROL 从Workfront预算请求]**&#x200B;方案模板创建[!DNL Anaplan]列表项。
1. 替换以下[!DNL Anaplan]个变量的变量值：

   | 变量名称 | 替换值为 |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | [!DNL Anaplan]帐户中的工作区ID。 |
   | [!UICONTROL [!DNL Anaplan]模型ID] | [!DNL Anaplan]帐户和所选工作区的模型ID。 |
   | [!UICONTROL [!DNL Anaplan]模块名称] | 描述选定[!DNL Anaplan]列表中的促销活动属性的模块名称。 |
   | [!UICONTROL 营销活动列表名称] | 您的[!DNL Anaplan]帐户和所选工作区和模型的列表名称。 |

   {style="table-layout:auto"}

   有关如何设置文件和进程的详细信息，请参阅[!DNL Anaplan]设置文档。

1. 选择或添加[!DNL Anaplan]连接配置文件。
1. 出现提示时，更新具有[!DNL Anaplan]连接的所有其余[!DNL Anaplan]模块。
1. 选择或添加[!DNL Workfront]连接配置文件。

   部署模板后，如果要将默认映射字段更改为[!DNL Anaplan]，您将更新此模块，以在fields属性的值中添加或删除自定义字段引用。

1. 出现提示时，更新具有[!DNL Workfront]连接的所有其余[!DNL Workfront]模块。

## 其他建议的方案模板

要完成此模板表示的工作流，您还必须部署以下附加模板：

* [[!UICONTROL 将 [!DNL Anaplan] 预算分配应用于 [!DNL Adobe Workfront] 项目]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

支出优化的其他方案包括：

* [[!UICONTROL 将 [!DNL Adobe Workfront] 项目更新发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL 向 [!DNL Anaplan] 列表项]发送 [!DNL Adobe Workfront] 实际小时更新](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL 将 [!DNL Adobe Workfront] 费用发送到 [!DNL Anaplan] 列表项]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
