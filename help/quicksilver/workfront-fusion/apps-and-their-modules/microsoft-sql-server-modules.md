---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: 连接器
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server模块
description: 您可以使用 [!DNL Adobe Workfront Fusion] 连接到Microsoft SQL Server。
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# [!DNL Microsoft SQL Server] 模块

您可以使用 [!DNL Adobe Workfront Fusion] 连接到 [!UICONTROL Microsoft SQL Server].

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

要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

有关 [!DNL Adobe Workfront Fusion] 许可证，请参阅 [[!DNL Adobe Workfront Fusion] 许可证](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 使用 [!DNL Microsoft SQL Server] 模块

您可以通过存储过程直接在数据库服务器上执行自定义逻辑。 [!DNL Adobe Workfront Fusion] 动态加载输入/输出参数和记录集的接口，以便每个参数或值可以单独映射。 在开始配置方案之前，请确保用于连接到数据库的帐户具有对的读取权限 `INFORMATION_SCHEMA.ROUTINES` 和 `INFORMATION_SCHEMA.PARAMETERS` 视图。

When [!DNL Fusion] 建立与 [!DNL SQL server] 目标， [!DNL Fusion] 用户标识主机（托管服务器的域名或IP地址）和端口。 [!DNL Fusion] 可以连接到任何可用的主机和端口。

有关使用的特定IP地址的信息 [!DNL Workfront Fusion]，请参阅 [用于访问的IP地址 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

要了解有关创建存储过程的更多信息，请参阅 [!DNL Microsoft SQL Server] 文档。

>[!NOTE]
>
>[!DNL Workfront Fusion] 不支持多个记录集。 只处理第一个。

## 故障诊断错误 [!UICONTROL ER_LOCK_WAIT_TIMEOUT:超出锁定等待超时；重新启动事务]

当您使用多个模块修改同一数据时，会发生此错误。 它是由SQL事务造成的。

执行任何SQL模块时，它将启动事务。 在方案完全执行后，事务即告完成。

如果其他模块尝试访问相同的数据，则必须等待上一个事务完成。 由于第一个交易将在方案完成后完成，因此第二个交易永远无法开始。

### 解决方案：

打开自动提交。 自动提交会在模块执行完成后立即完成（提交）每个事务。

1. 单击 [!UICONTROL 方案设置] 图标 ![](assets/scenario-settings-icon.png)屏幕底部。
1. 单击 **[!UICONTROL 自动提交]** 复选框。
1. 单击 **[!UICONTROL 确定]** 以保存方案设置。
