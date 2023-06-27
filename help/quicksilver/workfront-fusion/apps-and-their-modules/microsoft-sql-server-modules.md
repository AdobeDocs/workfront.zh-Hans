---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server模块
description: 您可以使用 [!DNL Adobe Workfront Fusion] 以连接到Microsoft SQL Server。
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 1%

---

# [!DNL Microsoft SQL Server] 模块

您可以使用 [!DNL Adobe Workfront Fusion] 以连接到 [!UICONTROL Microsoft SQL Server].

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
   <td>
   <p>当前许可证要求：否 [!DNL Workfront Fusion] 许可证要求。</p>
   <p>或</p>
   <p>旧版许可证要求： [！UICONTROL [!DNL Workfront Fusion] 用于工作自动化和集成] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">产品</td> 
   <td>
   <p>当前产品要求：如果您有[！UICONTROL Select]或[！UICONTROL Prime] [!DNL Adobe Workfront] 计划，您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。 [!DNL Workfront Fusion] 包含在[！UICONTROL Ultimate]中 [!DNL Workfront] 计划。</p>
   <p>或</p>
   <p>旧版产品要求：您的组织必须购买 [!DNL Adobe Workfront Fusion] 以及 [!DNL Adobe Workfront] 以使用本文中所述的功能。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

要了解您拥有什么计划、许可证类型或访问权限，请联系贵机构的 [!DNL Workfront] 管理员。

有关以下项的信息 [!DNL Adobe Workfront Fusion] 许可证，请参见 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用 [!DNL Microsoft SQL Server] 模块

您可以通过存储过程直接在数据库服务器上执行自定义逻辑。 [!DNL Adobe Workfront Fusion] 动态加载输入/输出参数和记录集的接口，以便每个参数或值可以单独映射。 在开始配置方案之前，请确保用于连接到数据库的帐户具有读取权限 `INFORMATION_SCHEMA.ROUTINES` 和 `INFORMATION_SCHEMA.PARAMETERS` 视图。

时间 [!DNL Fusion] 建立与 [!DNL SQL server] 目标， [!DNL Fusion] 用户标识主机（托管服务器的域名或IP地址）和端口。 [!DNL Fusion] 可以连接到任何可用的主机和端口。

有关使用的特定IP地址的信息 [!DNL Workfront Fusion]，请参见 [用于访问的IP地址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

要了解有关创建存储过程的更多信息，请参见 [!DNL Microsoft SQL Server] 文档。

>[!NOTE]
>
>[!DNL Workfront Fusion] 不支持多个记录集。 仅处理第一个实例。

## 错误疑难解答 [!UICONTROL ER_LOCK_WAIT_TIMEOUT：超过锁定等待超时；请尝试重新启动事务]

使用多个模块修改相同数据时，会发生此错误。 它由SQL事务引起。

执行任何SQL模块时，都会启动一个事务。 事务在方案完全执行后完成。

如果另一个模块尝试访问相同的数据，则必须等待上一个事务完成。 由于第一个事务将在方案完成后完成，因此第二个事务永远不能开始。

### 解决方案：

打开自动提交。 自动提交在模块执行完成后立即完成（提交）每个事务。

1. 单击 [!UICONTROL 方案设置] 图标 ![](assets/scenario-settings-icon.png)在屏幕底部。
1. 单击 **[!UICONTROL 自动提交]** 复选框。
1. 单击 **[!UICONTROL 确定]** 以保存方案设置。
