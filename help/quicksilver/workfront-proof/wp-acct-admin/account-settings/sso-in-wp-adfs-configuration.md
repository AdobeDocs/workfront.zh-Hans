---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: “单点登录” [!DNL Workfront Proof]:AD FS配置
description: 如果您是AD服务器上的管理员，则可以安装和配置AD FS。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---

# 单点登录 [!DNL Workfront Proof]:AD FS配置

>[!IMPORTANT]
>
>本文介绍独立产品中的功能 [!DNL Workfront Proof]. 有关内部校对的信息 [!DNL Adobe Workfront]，请参阅 [校对](../../../review-and-approve-work/proofing/proofing.md).

如果您是AD服务器上的管理员，则可以安装和配置AD FS。

## 安装和配置AD FS

1. 下载 [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) 到您的计算机。
1. 打开下载的AdfsSetup.exe文件以启动ADFS（Active Directory联合身份验证服务）安装向导。
1. 在“服务器角色”屏幕上，选择一个选项（至少需要一个联合服务器）。
1. 如果您不想将AD服务器上的IIS公开给Internet（HTTP和HTTPS的端口80和443），则可以先在防火墙后设置联合服务器，然后再构建一个联合服务器代理，该代理将请求通过防火墙传递到联合服务器。
1. 完成AD FS设置后，选择 **[!UICONTROL 启动AD FS 2.0管理管理单元]**，然后单击 **[!UICONTROL 完成]**. 完成后，应立即打开AD FS 2.0管理窗口。 如果没有，您可以从 **[!UICONTROL 开始]** > **[!UICONTROL 管理工具]** > **[!UICONTROL AD FS 2.0管理]**. 这是主AD FS控制应用程序。

1. 首先，单击AD FS 2.0联合服务器配置向导。
这将帮助您配置AD FS，并通过IIS和AD将其连接到Internet。
1. 如果要配置新的AD FS服务器，请选择 **[!UICONTROL 创建新的联合身份验证服务]**.
1. 选择 **[!UICONTROL 独立联合服务器]** （用于测试和评估目的）。

1. 要获得高可用性和负载平衡，请单击“新建联合服务器场”。
1. 指定您的联合身份验证服务名称。
默认情况下，配置向导会检索绑定到IIS中默认网站的SSL证书，并将使用此处指定的主题名称。 如果您使用通配符证书，则需要输入联合身份验证服务名称。
如果IIS中未配置SSL证书，则配置向导将在本地计算机证书存储区中搜索任何有效证书。 这些参数显示在SSL证书下拉列表中。 如果找不到证书，则可以使用IIS中的服务器证书生成器创建一个证书生成器。

1. 继续配置，然后单击 **[!UICONTROL 关闭]** 完成后。

## 配置 [!DNL Workfront Proof] 单点登录

如果您是 [!DNL Workfront Proof] 管理员，您可以在 [!DNL Workfront Proof] 侧。 有关更多信息，请参阅 [单点登录 [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. 单击 **[!UICONTROL 设置]** > **[!UICONTROL 帐户设置]**，然后打开 **[!UICONTROL 单点登录]** 选项卡。

1. 在 **SSO URL** 框中，粘贴您的实体ID。
以下是实体ID的示例：http://*&lt;adfs.your-company.com>*/adfs/services/trust您的实体ID可在您的联合元数据XML文件中找到。
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. 联合元数据可在AD FS 2.0管理单元>服务>端点文件夹中找到。 在元数据部分中，找到具有联合元数据类型的元数据。 要查看元数据，请将此端点粘贴到浏览器中。 您还可以直接转到以下链接：https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml)。
1. 在 **[!UICONTROL 登录URL]** 框中，粘贴您的SSO登录。
1. 以下是SSO登录示例：
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. 此链接可以位于联合元数据XML文件中。
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. 在 **[!UICONTROL 注销URL]** 框中，输入链接并保存。
以下是注销URL的示例：https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. 转到您的AD FS经理>信任关系>信赖方信任 — ProofHQ属性。
   1. 在“端点”下，单击 [!UICONTROL 添加和条目] 具有以下详细信息：

      * 端点类型= SAML注销
      * 绑定=POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * 在AD FS中配置信赖方信任后，可以完成此步骤（请参阅下文）。
   1. 在 **[!UICONTROL 证书指纹]** 框中，输入证书中的数据。
   1. 转到ADFS 2.0管理单元，导航到服务>证书>令牌签名。
   1. 右键单击此条目可查看证书。
   1. 从 [!UICONTROL 证书详细信息] 选项卡，复制指纹并将其粘贴到 **[!UICONTROL Workfront Proof单点登录]** “配置”选项卡。

   1. 指纹字符可以用冒号或空格分隔，但我们建议删除这些字符。 如果您的单点登录配置遇到任何问题，请联系客户支持团队。


## 添加信赖方信任

配置完成后，您需要在AD FS的信赖方信任部分中工作。

1. 导航到 **[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信托]** 文件夹，然后单击 **[!UICONTROL 添加信赖方信任]** 以启动配置向导。

1. 选择您的数据源。
您的 [!DNL ProofHQ] 帐户位于如下链接下：https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq这将配置大多数信赖方信任。

   >[!NOTE]
   >
   >* 如果您在从URL建立连接时遇到任何问题，请将元数据另存为文件，然后选择从文件导入数据。
   >* 当您在 [!DNL ProofHQ] 帐户将整个“{yoursubdomain}.proofhq.com”部分替换为您自己的域，以创建您的 [!DNL ProofHQ] 元数据链接。



## 配置声明规则

在您的信赖方信任配置完成后，您就可以配置声明规则以完成设置。 您将为ProofHQ配置两个声明规则：电子邮件和名称ID。

1. 打开 **[!UICONTROL 编辑声明规则]** 对话框。
1. 转到 **[!UICONTROL ProofHQ信赖方信任]**，然后单击 **[!UICONTROL 编辑声明规则]** (1)。\
   如果您在配置信任结束时选择了此选项，则应会自动打开弹出窗口。

1. 单击 **[!UICONTROL 添加规则]** (2)打开索赔配置窗口。

   * 电子邮件（将LDAP属性作为声明规则模板发送）
   * NameID（转换传入声明规则模板）
