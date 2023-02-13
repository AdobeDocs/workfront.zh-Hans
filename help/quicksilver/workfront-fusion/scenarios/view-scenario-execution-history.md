---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 在Adobe Workfront Fusion中查看方案的执行历史记录
description: 您可以显示某个方案的所有运行信息，也可以搜索该方案的所有执行以获取特定数据。
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# 在 [!DNL Adobe Workfront Fusion]

您可以显示某个方案的所有运行信息，也可以搜索该方案的所有执行以获取特定数据。

方案的执行历史记录显示了方案在过去30天内执行的所有情况。

## 访问要求

您必须具有以下访问权限才能使用本文中的功能：

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
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]许可证**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] （用于工作自动化和集成） </p><p>[!UICONTROL [!DNL Workfront Fusion] （工作自动化） </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>贵组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中描述的功能。</td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 查看方案的所有执行

### 在 [!UICONTROL 方案详细信息] 页面

1. 单击 **[!UICONTROL 方案]** 选项卡，然后单击方案。

   或

   如果您正在方案编辑器中处理方案，请单击左箭头 ![](assets/exit-editing-arrow.png) 在窗子的左上角附近。

1. 查看右侧列表中的信息。

   ![](assets/open-history-tab-350x202.png)

   C

   您还可以单击以查看此信息的全页视图。 利用全页视图，可过滤历史记录以查看特定执行。

   每次执行方案时，都会列出以下详细信息：

   * 运行的日期 **[!UICONTROL 开始]**
   * **[!UICONTROL 状态]** （成功或失败）
   * 运行 **[!UICONTROL 持续时间]**
   * 数量 **[!UICONTROL 操作]**
   * 大小 **[!UICONTROL 数据传输]**
   * 链接到 **[!UICONTROL 详细信息]**

### 在 [!UICONTROL 历史] 选项卡

的 [!UICONTROL 历史] 选项卡上显示的详细信息比 [!UICONTROL 方案详细信息] 页面。 您还可以在 [!UICONTROL 历史] 选项卡。

1. 单击 **[!UICONTROL 方案]** 选项卡，然后单击方案。

   或

   如果您正在方案编辑器中处理方案，请单击左箭头 ![](assets/exit-editing-arrow.png) 在窗子的左上角附近。

1. 单击 **[!UICONTROL 历史]** 选项卡
1. （可选）有关选定方案运行（包括已处理的包）的详细信息，请单击 **[!UICONTROL 详细信息]** 链接。

   有关处理包的更多信息，请参阅 [中的方案执行流程 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >的 [!UICONTROL 详细信息] 仅当执行具有可用的详细信息时，才会显示链接。

## 过滤方案执行历史记录

您可以过滤执行历史记录，以仅查看具有指定值的执行。

1. 打开方案的整页历史记录，如 [在 [!UICONTROL 历史] 选项卡](#view-scenario-execution-history-on-the-history-tab) 在本文中。
1. 单击 [!UICONTROL 过滤器] 图标 ![](assets/fusion-scenario-filter-icon.png) 在要过滤的列标题中。
1. 在 [!UICONTROL 过滤器] 对话框，输入要过滤的值。
1. 单击&#x200B;**[!UICONTROL 保存]**。

过滤器图标在具有当前活动过滤器的列中为橙色。

## 对方案执行历史记录进行排序

您可以对方案执行历史记录进行排序。

1. 打开方案的整页历史记录，如 [在 [!UICONTROL 历史] 选项卡](#view-scenario-execution-history-on-the-history-tab) 在本文中。
1. 单击 [!UICONTROL 排序] 图标。
1. 可选：要反转排序顺序，请单击 [!UICONTROL 排序] 图标。

## 搜索方案的所有执行

1. 单击 **[!UICONTROL 方案]** 图标 ![](assets/scenarios-icon.png) 在左侧面板中，单击方案。

   或

   如果您正在方案编辑器中处理方案，请单击左箭头 ![](assets/exit-editing-arrow.png) 在窗子的左上角附近。

1. 单击 **[!UICONTROL 历史]** 选项卡。
1. 单击 **[!UICONTROL 全文搜索]** 执行列表的顶部。

   或

   类型 **Ctrl+Shift+F** (Windows)或 **Cmd+Shift+F** (Mac) [!UICONTROL 在历史记录中搜索] 窗口。

1. （可选）要搜索包含特定文本的执行，请在 **[!UICONTROL 在历史记录中搜索]** 窗口。

   要搜索确切的文本，请在文本周围加上双引号(&quot;example&quot;)。

   >[!INFO]
   >
   >**示例：** 如果要查找创建特定项目的执行情况，请在 [!UICONTROL 全文搜索] 栏。
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. （可选）要按日期范围限制搜索，请在 [!UICONTROL 按日期范围] 的上界。

   >[!NOTE]
   >
   >* 仅在过去30天内执行。
   >
   >* [!DNL Workfront Fusion] 存储30天的网页挂钩负载。 在创建Webhook有效负载30天后访问该负载会导致错误“[!UICONTROL 无法从存储中读取文件。]&quot;



1. （可选）要按状态限制搜索，请在 **[!UICONTROL 按状态]** 下拉列表。


   可用状态包括：

   * [!UICONTROL 全部]

   * [!UICONTROL 错误]

   * [!UICONTROL 警告]

   * [!UICONTROL 成功]

1. （可选）更改结果在 **[!UICONTROL 按日期排序]** 下拉列表。

1. （可选）要复制方案执行ID，请单击 **[!UICONTROL 复制执行ID]** 图标 <img src="assets/copy-fusion-execution-id-icon.png"> 在所需执行的行中

1. （可选）单击 [!UICONTROL 全文搜索] 检查包含该信息的方案模块输出包。
