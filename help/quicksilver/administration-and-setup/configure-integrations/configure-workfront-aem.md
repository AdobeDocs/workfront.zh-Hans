---
title: 配置 [!DNL Workfront] with [!DNL Adobe Experience Manager] 旧连接器
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 作为 [!DNL Adobe Workfront] 管理员，您可以集成 [!DNL Workfront] Adobe Experience Manager(AEM)资产，并为贵组织提供了一个全面的内容管理解决方案，用于在您的工作流中创建、共享和维护资产。
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1893'
ht-degree: 0%

---

# 配置 [!DNL Workfront] with [!DNL Adobe Experience Manager] 旧连接器

作为 [!DNL Adobe Workfront] 管理员，您可以集成 [!DNL Workfront] with [!UICONTROL Adobe Experience Manager(AEM)Assets] 并为贵组织提供全面的内容管理解决方案，用于在您的工作流中创建、共享和维护资产。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证*</td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关 [!DNL Workfront] 管理员，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可类型或访问权限，请联系您的 [!DNL Workfront] 管理员。

## [!DNL Workfront for AEM Assets]

的 [!DNL Workfront for AEM Assets connector] 允许贵组织执行以下操作：

* 通过将AEM资产和文件夹关联到 [!DNL Workfront].

   有关配置与第三方应用程序的文档集成的更多信息，请参阅  [配置文档集成](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* 与集成 [!DNL AEM Digital Asset Managemen]t(DAM)存储库，允许您使用 [!DNL Workfront] 管理和共享存储在DAM中的数字资产。

   有关链接文档和资产文件夹的更多信息，请参阅   [从外部应用程序链接文档](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* 将两个应用程序中的元数据合并并应用于资产。
* 查看资产的全包通信流。 在 [!DNL Workfront] 或 [!UICONTROL AEM Assets] 同步到其他应用程序，以建立与资产进行通信的全面历史记录。

   有关在 [!DNL Workfront]，请参阅 [向文档添加更新](../../documents/managing-documents/add-update-documents.md).

## 安装的先决条件 [!DNL AEM Assets] 连接器

安装之前 [!DNL Workfront] 连接器 [!UICONTROL AEM Assets]，请确保满足以下先决条件：

* [!UICONTROL AEM Assets] 已安装并配置了版本6.5或更高版本。 有关安装的信息 [!UICONTROL AEM Assets]，请参阅 [[!DNL Adobe Experience Manager] 文档](https://experienceleague.adobe.com/docs/experience-manager.html).
* （视情况而定）如果您的防火墙规则不允许按预期的流量，请将群集的IP地址和/或域添加到您的允许列表。 有关更多信息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## 安装 [!DNL Workfront for AEM Assets] 连接器软件包 {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>以下说明适用于 [!DNL Workfront with AEM Assets] 旧版连接器，已被替换为 [[!DNL Workfront for Experience Manager] 增强连接器](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). 有关详细信息，请联系您的客户代表。

安装 [!DNL Workfront for AEM Assets] 连接器中，必须使用 [!UICONTROL CRX包管理器].

1. 在已安装AEM的工作站上，下载 [!DNL Workfront for AEM Assets] 连接器安装文件。

   您可以获取 [!DNL Workfront for AEM Assets] 连接器 [!DNL Workfront] 代表。

1. 使用管理员帐户登录AEM。
1. 单击 **[!UICONTROL 工具]** > **[!UICONTROL 部署]** > **[!UICONTROL 包]**.

   的 [!UICONTROL CRX包管理器] 打开。

1. 单击 **[!UICONTROL 上传包].**

1. 在 [!UICONTROL 上传包] 对话框，浏览并选择 [!UICONTROL Workfront Connector] 包，然后单击 **[!UICONTROL 确定]**.\
   包将显示在 [!UICONTROL CRX包管理器].

1. 单击 **[!UICONTROL 安装].**

1. 在 [!UICONTROL 包] 对话框，忽略高级设置并单击 **[!UICONTROL 安装]**.
1. （可选）要确认连接器已成功安装，请确保在 [!UICONTROL 活动日志]:

   ```
   Package installed in <time>
   ```

1. 关闭 [!UICONTROL CRX包管理器].

   连接器已安装，您现在可以配置 [!DNL AEM Assets] 与集成 [!DNL Workfront].

1. 继续 [配置 [!DNL AEM Assets] 与集成 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## 配置 [!DNL AEM Assets] 与集成 [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

安装连接器后，将连接器包导入AEM，并配置AEM以与 [!DNL Workfront].

有关安装连接器的信息，请参阅  [安装 [!DNL Workfront for AEM Assets] 连接器软件包](#install-the-workfront-for-aem-assets-connector-package).

* [先决条件](#prerequisites)
* [将AEM与 [!DNL Workfront]](#integrate-aem-with-workfront)
* [配置 [!UICONTROL AEM外部器]](#configure-the-aem-externalizer)

### 先决条件 {#prerequisites}

在开始之前，必须启用workfront服务的权限：

1. 在AEM中，转到 **[!UICONTROL 工具]**> **[!UICONTROL 安全性]**> **[!UICONTROL 权限]**.
1. 在左上角，选择 **[!UICONTROL 用户]**&#x200B;在下拉菜单中，然后输入 *[!UICONTROL 工作流服务]* 在 **[!UICONTROL 搜索]**&#x200B;。 选择 [!UICONTROL 工作流服务] 用户。
1. 在屏幕的右侧，选择 **[!UICONTROL 添加ACE]** 创建新条目。
1. 在&#x200B;**[!UICONTROL 添加新条目]**&#x200B;的 **[!UICONTROL 路径]**&#x200B;字段，然后选择文件夹： */conf*
1. 在权限字段中，输入： *jcr:read*
1. 选择 **[!UICONTROL 添加]**&#x200B;右上角
1. （可选）重复这些步骤以创建更多条目。

### 将AEM与 [!DNL Workfront] {#integrate-aem-with-workfront}

1. 以管理员身份登录AEM Assets。
1. 单击 **[!UICONTROL 工具]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Workfront集成配置]** >**[!UICONTROL 全球Workfront].**&#x200B;**&#x200B;**

1. （视情况而定）如果您尚未执行此操作，请创建 [!DNL Workfront] 云配置文件。

   1. 单击  **[!UICONTROL 创建]** 的右上角 [!DNL Global-Workfront] 页面。
   1. 在 **[!UICONTROL Workfront URL]** 框中，指定 [!DNL Workfront] 实例。

      例如， [!DNL https]://`<account>`.my.workfront.com，其中 `<account>` 是用于与AEM集成的帐户。

   1. 在&#x200B;**[!UICONTROL 基本文件夹]** ，选中复选框图标，然后在下拉菜单中选择链接文档的路径 [!DNL Workfront] 对象被存储。
   1. 在显示的AEM模式中，按照文件夹的路径(包含与 [!DNL Workfront] 对象。 选择文件夹并按 **[!UICONTROL 选择]**&#x200B;中。

      您可以链接到根/content/dam/下的任何文件夹。

   1. 在 **[!UICONTROL Workfront API密钥]** 框中，指定 [!UICONTROL Workfront] API密钥。

      检索 [!DNL Workfront] API密钥：

      1. 打开浏览器选项卡，然后登录 [!DNL Workfront] as a [!DNL Workfront] 管理员。
      1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

      1. 单击 **[!UICONTROL 系统]** >**[!UICONTROL 客户信息]**.

         如果您已经生成API密钥，则您的 [!DNL Workfront] API密钥显示在用户的API密钥标签下。

      1. （视情况而定）如果您尚未生成API密钥，则需要生成一个：

         1. 在 **[!UICONTROL API密钥设置]** 部分，确保 **[!UICONTROL 创建后，API密钥将在]** 选项设置为“无”。

            如果选择过期期限，则API密钥过期后，连接器将停止工作。 然后，您需要重新生成API密钥并更新 [!DNL Workfront] 配置。

         1. 在 **[!UICONTROL 用户的API密钥]** 标签，单击 **[!UICONTROL 生成API密钥]**.

            适用于的API密钥 [!DNL Workfront] 生成并显示。
      1. 将API密钥复制到剪贴板。
      1. 打开AEM Connector的浏览器选项卡，然后在 **[!DNL Workfront API Key]** 框中，粘贴您复制的API密钥。
   1. （视情况而定）单击 **[!UICONTROL 高级]** 选项卡 [!UICONTROL [!DNL Workfront] 集成配置] ，并选择以下选项（如果适用）：

      **[!UICONTROL 允许收藏集浏览]:**&#x200B;如果贵组织允许 [!DNL Workfront] 用户将AEM Assets收藏集关联到 [!DNL Workfront] 对象。

      **[!UICONTROL 用户Federated ID]:** 如果贵组织在登录Workfront时使用Federated ID或单点登录(SSO)，请选择此选项。

      **[!UICONTROL 忽略电子邮件域]:** 如果您的AEM用户在其用户ID中未使用域名，请选择此选项。

      **[!UICONTROL 限制访问]:** 选择此选项可指定 [!DNL Workfront] 需要添加到的IP地允许列表址。 有关的更多信允许列表息，请参阅 [配置防火墙的允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. 单击 **[!UICONTROL 基本]** 选项卡，然后单击 **[!UICONTROL 连接]**.

      >[!NOTE]
      >
      >更改可能需要一些时间才能应用。 重新启动包可能会加快该过程。



1. （视情况而定）如果您已经创建 [!DNL Workfront] 云配置文件，选择 **[!UICONTROL 全球 —[!DNL Workfront]]**，然后在左上角单击 **[!UICONTROL 属性]**.

1. 通过单击 **[!UICONTROL 生成密钥],** 然后，将AEM API密钥复制到剪贴板。

   您稍后在配置 [!UICONTROL Workfront] 与集成 [!UICONTROL AEM Assets]. 有关更多信息，请参阅 [配置Workfront以与AEM资产集成](#configure-workfront-to-integrate-with-aem-assets).

1. 在右上角，单击 **[!UICONTROL 保存]**.

   的 [!UICONTROL 全球 — [!DNL Workfront]] 窗口。

   ![Properties.png](assets/properties-350x117.png)

1. （可选）同步AEM与 [!DNL Workfront].

   1. 单击 **[!UICONTROL 全球 — [!DNL Workfront]].**
   1. 在窗口的左上角，单击 **[!UICONTROL 属性]**.

      的 [!UICONTROL [!DNL Workfront] 集成配置] 页面。

      ![属性2.png](assets/properties2-350x444.png)

   1. （可选）要在 [!UICONTROL AEM Assets] 和 [!DNL Workfront]，单击 **[!UICONTROL 启用注释同步]**.

      >[!IMPORTANT]
      >
      >必须启用 [!UICONTROL 文档同步] 以同步资产。

   1. （可选）要关闭注释同步，请单击 **[!UICONTROL 禁用注释同步].**

      或

      删除 [!UICONTROL 注意创建] 已注册到AEM实例的事件订阅。

      有关事件订阅的信息，请参阅 [事件订阅API](../../wf-api/general/event-subs-api.md).

1. 继续 [配置 [!UICONTROL AEM外部器]](#configure-the-aem-externalizer).

### 配置 [!UICONTROL AEM外部器] {#configure-the-aem-externalizer}

的 [!UICONTROL AEM外部器] 允许AEM以可在 [!DNL Workfront]. 如果未正确配置， [!DNL Workfront] 无法调用AEM API，并且在Workfront中关联AEM文档的URL将不起作用。

1. 在AEM中，单击 **[!UICONTROL 工具]** > **[!UICONTROL 操作]** >**[!UICONTROL Web控制台]**.

1. 单击 **[!UICONTROL OSGI]**，然后单击 **[!UICONTROL 配置]** 中。

1. 在配置列表中，选&#x200B;择&#x200B;**[!UICONTROL Day CQ链接外部器].**

   的 [!UICONTROL 外部器] 页面。

1. 在 **[!UICONTROL 域]** 部分，确保 [!UICONTROL 作者] 字段是AEM用户可从外部访问的域名。

   中的域名 [!UICONTROL 作者] 字段应与AEM实例URL行中列出的域相匹配。

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. （视情况而定）如有必要，请在 [!UICONTROL 作者] 字段。
1. 单击&#x200B;**[!UICONTROL 保存]**。

   [!UICONTROL AEM Assets] 现在配置为将文档与 [!DNL Workfront]

1. 继续 [配置 [!DNL Workfront] 与集成 [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## 配置 [!DNL Workfront] 与集成 [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

安装 [!UICONTROL Workfront for AEM Assets] 连接器(如 [安装 [!UICONTROL Workfront for AEM Assets] 连接器软件包](#install-the-workfront-for-aem-assets-connector-package))和配置 [!UICONTROL AEM Assets] (如 [配置[!UICONTROL  AEM Assets] 与集成 [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront))，则需要配置 [!DNL Workfront] 链接文档 [!DNL Workfront] 和 [!DNL AEM Assets].

1. 登录到 [!DNL Workfront] as a [!UICONTROL Workfront] 管理员。

   >[!TIP]
   >
   >[!UICONTROL Workfront] 建议创建 [!UICONTROL Workfront] 专门用于您的AEM集成的管理员。 有关分配 [!UICONTROL Workfront] 用户的管理员访问级别，请参阅 [授予用户对特定区域的管理访问权限](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe Workfront]，然后单击 **[!UICONTROL 设置]** ![](assets/gear-icon-settings.png).

1. 单击 **[!UICONTROL 文档]**> **[!UICONTROL 自定义集成].**

1. 单击 **[!UICONTROL 添加自定义集成]**.
1. 在 **[!UICONTROL 名称]** 框中，指定自定义集成的名称。

   这是用户在中使用集成时看到的名称 [!UICONTROL Workfront];例如，您可以在 *&quot;[!DNL AEM Assets]&quot;* 的名称。

1. 在 **[!UICONTROL 基本API URL]** 框中，指定AEM实例的URL。

   基本API URL由AEM实例的URL以及路径组成：/bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. 在 **[!UICONTROL 身份验证类型]** 下拉菜单，选择 **[!UICONTROL ApiKey].**

1. 在&#x200B;**[!UICONTROL API密钥]** 框中，粘贴您在配置时复制的AEM API密钥 [!UICONTROL AEM Assets].
1. 单击&#x200B;**[!UICONTROL 保存]**。
1. （可选）确保集成已标记 [!UICONTROL 活动].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] 现在配置为使用 [!DNL AEM Assets].

   要在AEM中访问资产，每个 [!DNL Workfront] 需要使用连接器的用户必须在AEM中设置为用户。 有关创建用户的信息，请参阅  [设置用户以使用连接器](#set-up-users-to-use-the-connector).

## 设置用户以使用连接器 {#set-up-users-to-use-the-connector}

用户要访问连接器，必须在AEM中具有用户配置文件，且属于 [!DNL Workfront] 具有包含 [!UICONTROL 创建] 和 [!UICONTROL 删除] 权限。

有关 [!DNL Workfront] 权限，请参阅 [创建或修改自定义访问级别](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [在 [!DNL AEM assets]](#set-up-users-in-aem-assets)

### 在 [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. 登录到 [!DNL AEM Assets] as a [!DNL Workfront] 管理员。
1. 单击 **[!UICONTROL 工具]** >**&#x200B;**&#x200B;**[!UICONTROL 安全性]** >**[!UICONTROL 用户]**.

1. （视情况而定）如果用户在AEM中没有用户配置文件，请创建AEM用户配置文件。

   1. 单击 **[!UICONTROL 创建用户].**
   1. 输入用户的个人信息。

      ![64NewUser.png](assets/64newuser-350x524.png)

      唯一的必填字段是ID字段。 用户的AEM ID必须匹配 [!DNL Workfront] ID，用户的 [!DNL Workfront] 电子邮件地址。

      如果您选择了 [!UICONTROL 忽略电子邮件域] 选项。当您配置AEM与 [!DNL Workfront]，则AEM ID将与 [!DNL Workfront] 电子邮件地址。

1. （视情况而定）如果用户具有AEM配置文件，请打开用户的AEM配置文件。

   1. 单&#x200B;击&#x200B;**[!UICONTROL 用户].**

      的 [!UICONTROL 用户管理] 页面。

   1. 单击要添加的用户，然后单击 **[!UICONTROL 属性]**.

      此时会显示用户的设置页面。

1. 单击 **[!UICONTROL 群组]** 选项卡。

   ![](assets/groupstab.png)

1. 确保用户至少属于一个 [!DNL Workfront] 具有包含 [!UICONTROL 创建] 和 [!UICONTROL 删除] 权限。

   1. 要将用户添加到现有群组，请在 **[!UICONTROL 类型组名称]** 框中，然后在下拉菜单中选择显示的群组。

      或

      要选择用户所属的组，请在 **[!UICONTROL 此用户所属的组]** 中。

1. 单击&#x200B;**[!UICONTROL 保存]。**
