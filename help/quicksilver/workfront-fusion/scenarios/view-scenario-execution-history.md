---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中查看方案的历史记录
description: 您可以显示某个方案的所有运行信息，也可以搜索方案的所有执行以获取特定数据。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 2e26c4e4b5f331ed2e609381ef442f45e90c4faa
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# 在[!DNL Adobe Workfront Fusion]中查看方案的历史记录

您可以显示有关场景的事件或执行的信息，也可以搜索场景的所有执行以获取特定数据。

场景执行表示场景的单次运行。

场景事件是对场景的修改，如编辑、激活或停用场景。

>[!NOTE]
>
>方案的历史记录会显示方案在过去30天内的所有事件和执行。

## 访问要求

您必须具有以下权限才能使用本文中的功能：

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td> <p>[!DNL Pro] 或更高</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td> <p>[！UICONTROL计划]，[！UICONTROL工作]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[！UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td>
   <p>当前许可证要求：无[!DNL Workfront Fusion]许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求：[！UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]，[！UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront]计划，则贵组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]才能使用本文中描述的功能。 [!DNL Workfront Fusion]包含在[！UICONTROL Ultimate] [!DNL Workfront]计划中。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买[!DNL Adobe Workfront Fusion]和[!DNL Adobe Workfront]，才能使用本文中介绍的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请与[!DNL Workfront]管理员联系。

有关[!DNL Adobe Workfront Fusion]许可证的信息，请参阅[[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md)。

## 查看方案历史记录

### 在[!UICONTROL 方案详细信息]页面上查看方案历史记录

1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]**&#x200B;选项卡，然后单击方案。

   或

   如果您在方案编辑器中处理方案，请单击窗口左上角附近的左箭头![](assets/exit-editing-arrow.png)。

1. 在右侧面板的&#x200B;**History**&#x200B;选项卡中查看执行历史记录。

   针对方案的每次执行都列出了以下详细信息：

   * 运行开始日期&#x200B;****
   * **[!UICONTROL 状态]** （成功或失败）
   * 运行&#x200B;**[!UICONTROL 持续时间]**
   * **[!UICONTROL 操作数]**
   * **[!UICONTROL 数据传输的大小]**

   >[!NOTE]
   >
   >方案历史记录会在最近执行的方案旁边显示一个&#x200B;**正在处理**&#x200B;标记，同时将执行详细信息写入存储。 在场景执行后立即进行处理。 并且持续时间不应超过几分钟。 处理执行时，场景执行的详细信息可能不可见。

1. 要查看特定场景执行的详细信息，请单击右侧面板中的该执行。
1. 要查看事件，请单击右侧面板的&#x200B;**事件**&#x200B;选项卡。


### 在[!UICONTROL 历史记录]选项卡上查看方案历史记录

[!UICONTROL 历史记录]选项卡显示的详细信息比[!UICONTROL 方案详细信息]页面上提供的多。 您还可以对[!UICONTROL 历史记录]选项卡上的执行进行过滤和排序。

1. 单击左侧面板中的&#x200B;**[!UICONTROL 方案]**&#x200B;选项卡，然后单击方案。

   或

   如果您在方案编辑器中处理方案，请单击窗口左上角附近的左箭头![](assets/exit-editing-arrow.png)。

1. 单击页面左上角附近的&#x200B;**[!UICONTROL 历史记录]**&#x200B;选项卡
1. （可选）有关所选方案运行的详细信息（包括已处理哪些捆绑包），请单击该行中用于该执行的&#x200B;**[!UICONTROL 详细信息]**&#x200B;按钮。

   有关处理捆绑包的更多信息，请参阅 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md)中的[方案执行流程。

   >[!NOTE]
   >
   >* 仅当执行有详细信息时，[!UICONTROL 详细信息]链接才可见。
   >
   >* 方案历史记录会在最近执行的方案旁边显示一个&#x200B;**处理历史记录**&#x200B;标记，同时将执行详细信息写入存储。 在场景执行后立即进行处理。 并且持续时间不应超过几分钟。 处理执行时，场景执行的详细信息可能不可见。

1. 要查看事件，请启用&#x200B;**显示事件**&#x200B;切换开关。

## 筛选场景执行历史记录

您可以过滤执行历史记录以仅查看具有指定值的执行。

1. 打开方案的全页历史记录，如本文中[!UICONTROL 历史记录]选项卡](#view-scenario-execution-history-on-the-history-tab)上的[查看方案执行历史记录中所述。
1. 单击要作为筛选依据的列标题中的[!UICONTROL 筛选器]图标![](assets/fusion-scenario-filter-icon.png)。
1. 在[!UICONTROL 筛选器]对话框中，输入筛选依据的值。
1. 单击&#x200B;**[!UICONTROL 保存]**。

过滤器图标位于包含当前活动过滤器的列中，且为橙色。

## 对方案执行历史记录排序

您可以对方案执行历史记录进行排序。

1. 打开方案的全页历史记录，如本文中[!UICONTROL 历史记录]选项卡](#view-scenario-execution-history-on-the-history-tab)上的[查看方案执行历史记录中所述。
1. 单击要作为筛选依据的列标题中的[!UICONTROL 排序]图标。
1. 可选：若要反转排序顺序，请再次单击[!UICONTROL 排序]图标。

## 搜索场景的所有执行

1. 打开方案的全页历史记录，如本文中[!UICONTROL 历史记录]选项卡](#view-scenario-execution-history-on-the-history-tab)上的[查看方案执行历史记录中所述。
1. 单击执行列表顶部的&#x200B;**[!UICONTROL 全文搜索]**。

   或

   键入&#x200B;**Ctrl+Shift+F** (Windows)或&#x200B;**Cmd+Shift+F** (Mac)
将打开[!UICONTROL 在历史记录中搜索]窗口。

1. （可选）要搜索包含特定文本的执行内容，请在&#x200B;**[!UICONTROL 在历史记录中搜索]**&#x200B;窗口的搜索栏中输入文本。

   要搜索精确文本，请用双引号将文本括起来（“示例”）。

   >[!INFO]
   >
   >**示例：**&#x200B;如果要查找创建特定项目的执行，请在[!UICONTROL 全文搜索]栏中输入项目ID。
   >
   >“625ef2ef0006036bd1794b6e52d737c5”

1. （可选）要按日期范围限制搜索，请在[!UICONTROL 按日期范围]区域中选择所需搜索的开始和结束日期。

   >[!NOTE]
   >
   >* 执行仅可用于之前的30天。
   >
   >* [!DNL Workfront Fusion]存储webhook负载30天。 创建webhook有效负载超过30天后对其进行访问会导致错误“[!UICONTROL 无法从存储中读取文件。]”


1. （可选）要按状态限制搜索，请在&#x200B;**[!UICONTROL 按状态]**&#x200B;下拉列表中选择所需的状态。


   可用状态包括：

   * [!UICONTROL 全部]

   * [!UICONTROL 错误]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （可选）更改结果在&#x200B;**[!UICONTROL 按日期排序]**&#x200B;下拉列表中的显示顺序。

1. （可选）要复制场景执行ID，请单击&#x200B;**[!UICONTROL 复制执行ID]**&#x200B;图标 所需执行的行中的<img src="assets/copy-fusion-execution-id-icon.png">

1. （可选）单击[!UICONTROL 全文搜索]的结果以检查包含该信息的方案模块输出包。
