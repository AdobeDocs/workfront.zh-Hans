---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: manage-your-billing-workfront-proof
title: 的 [!DNL Workfront] 校样账单页
description: 访问 [!UICONTROL 帐单] 页面，打开屏幕右上方的“设置”菜单，然后在下拉菜单中选择“帐单”。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f3828671-e950-4649-9f6d-881101100a96
source-git-commit: 1312e3d5256f28ca0197c73a6c06016d6d7c7e2a
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# 的 [!DNL Workfront Proof] 帐单页面

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

## 帐单页面

访问 [!UICONTROL 帐单] 页面，打开 **[!UICONTROL 设置]** 菜单，然后选择 **[!UICONTROL 帐单]** 中。

的 [!UICONTROL 帐单] 页面包含以下内容：

* 帐户名称(1)
* 帐户列表（例如，如果您有卫星帐户）(2)
* 变更计划（三）
* 更改付款详情(4)
* 新卫星账户(5)
* 关闭帐户(6)
* 当前计划信息(7)
* 帐单联系方式和地址(8)
* 使用情况统计(9)
* 账单历史记录(10)
* 账单活动(11)

   ![Billing_page.jpg](assets/billing-page-350x315.jpg)

## [!UICONTROL 当前计划]

本节(7)显示您当前计划的详细信息，包括以下内容：

* 计划的名称
* 当前付款方法
* 当前计划开始和结束日期
* 下一计划类型
* 下一计划付款方法

   有关更多信息，请参阅 [在中选择您的付款方法 [!DNL Workfront Proof]](../../../workfront-proof/wp-billingsettings/manage-your-billing/choose-payment-method-in-wp.md).

## [!UICONTROL 帐单联系人和地址]

此部分(8)显示了您帐户的主要账单联系方式和地址详细信息。

只能从您帐户中设置为账单管理员的用户中选择账单联系人。 在卫星帐户上，只能在此字段中设置主帐户中的账单管理员。

![Billing_Contact.png](assets/billing-contact-350x137.png)

>[!NOTE]
>
> 您的帐户上可以有多个账单管理员，但在 [!UICONTROL 账单联系人] 字段接收所有账单通知和帐户使用情况警报。

这包括以下通知电子邮件：

* 校样用法
* 发票
* 降级
* 延迟付款/帐户暂停警报
* 信用卡故障

   ![Billin_CC.png](assets/billin-cc-350x103.png)

的 [!UICONTROL 账单抄送] 字段中，您还可以添加要在所有与账单相关的电子邮件中复制的电子邮件地址。 单击字段以激活倾斜编辑，并输入您选择的电子邮件地址（这也可以是现有用户的电子邮件地址）。

## [!UICONTROL 帐单地址]

此部分使用内联编辑，因此只需单击字段即可输入/编辑文本。

>[!NOTE]
>
> 我们将此地址包含在您的订阅发票中，以确保此数据始终为最新。

![Billing_Address.png](assets/billing-address-350x199.png)

## [!UICONTROL 使用情况统计信息]

此部分显示当前帐单期间帐户的使用情况统计信息，包括以下内容：

* 已使用的存储
* 使用的校样
* 使用的用户限制

![Usage_Statistics.png](assets/usage-statistics-350x51.png)

### [!UICONTROL 使用警告]

的 [[!UICONTROL 校样权限配置文件] in [!DNL Workfront] 校样](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) 设置为，当您的帐户达到以下状态时，您帐户上的账单联系人(1)将通过电子邮件收到通知：

* 存储容量的75%，然后是98%
* 75%，然后100%的证明限制

![Billing_Contact__1_.png](assets/billing-contact--1--350x74.png)

达到校样或存储限制后，您还将在 [!UICONTROL 帐单] 页面：

* 对于达到的校样限制

   ![Proodms_limit_reached.png](assets/proofs-limit-reached-350x65.png)

* 对于达到的存储限制

![Storage_limit_recaimed.png](assets/storage-limit-reached-350x65.png)

>[!NOTE]
>
>在帐户中创建校样时，校样计数会被用完，并且无法通过删除校样来还原。

可以通过删除校样和文件并清空 [!UICONTROL 垃圾] 之后。

请记住，如果您需要更多校样、存储或用户，您可以随时升级您的帐户；它会立即生效。

## [!UICONTROL 账单历史记录]

此部分显示任何最近计费期的活动。 您也可以从此部分下载发票。

有关更多信息，请参阅 [下载 [!DNL Workfront Proof] 发票](../../../workfront-proof/wp-billingsettings/manage-your-billing/download-wp-invoice.md).&quot;

## [!UICONTROL 计费活动]

此部分显示对您的账单设置的近期更改，例如订阅、升级、降级和续订 [!DNL Workfront Proof] 计划。

如果您将计划更改为具有较低用户限制(1)的计划，则超过新限制的用户将在新计划开始时自动停用。 此活动还将在您的帐户日志(2)中捕获。

![Billing_Downradge_log.png](assets/billing-downgrade-log-350x45.png)

![Account_Activity_-_Deleted_users.png](assets/account-activity---deleted-users-350x94.png)
