---
title: 从Workfront OAuth2迁移到Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Workfront的旧版自定义OAuth2应用程序服务即将停用。 了解更改内容、受影响人员以及如何将自定义集成迁移到Adobe Developer Console。
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# 从Workfront OAuth2迁移到Adobe Developer Console

Workfront的旧版自定义OAuth2应用程序服务（您在&#x200B;**设置** > **系统** > **OAuth2**&#x200B;下设置的集成）正在被弃用。 今后，所有针对Workfront进行身份验证的自定义集成都必须改用Adobe Developer Console (developer.adobe.com)身份验证流程。

此更改会影响当前使用Workfront颁发的OAuth2客户端ID和密码进行身份验证的任何自定义集成、脚本或第三方工具。 它不会影响您登录到Workfront的方式，也不会影响Adobe管理的标准集成，例如打包的Microsoft Teams或Slack集成，Adobe将分别迁移这些集成。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront访问级别配置</td> 
   <td><p>系统管理员</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Developer Console权限</td> 
   <td><p>要访问Workfront的Adobe Developer Console，需要拥有完整的IMS组织管理员权限。 这比Workfront产品管理员角色更广泛，因为它管理整个Adobe组织及其下的所有产品。</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## 关键日期

| 日期 | 里程碑 | 这对您意味着什么 |
|---|---|---|
| 2026年11月1日 | 已禁用新应用程序创建 | 您无法再在Workfront中创建新的自定义OAuth2应用程序。 现有应用程序可继续工作。 |
| 2027年2月1日 | 已弃用旧版服务 | 现有自定义OAuth2应用程序完全停止工作。 此时，任何尚未迁移到Adobe Developer Console的集成都将失去对Workfront API的访问权限。 |

>[!IMPORTANT]
>
>我们强烈建议在2026年11月1日之前规划和完成您的迁移，以便您的集成可以继续运行而不会受到干扰，并且您不会在2027年2月1日的硬截止日期之前进行迁移。

## 受影响的组织

如果您的组织具有使用自定义OAuth2客户端ID和通过Workfront旧版OAuth2设置屏幕发布的密钥连接到Workfront的任何集成、脚本或工具，则将会受到此更改的影响。 常见示例包括：

* 您的工程团队根据Workfront API维护的自定义集成。
* 使用Workfront颁发的客户端ID配置的第三方或合作伙伴构建的连接器。 如果您不确定其集成如何进行身份验证，我们建议您与供应商进行核实。
* 直接调用Workfront API的内部自动化、报表或数据同步脚本。

如果您不知道您的组织是否具有这些应用程序，您的Workfront管理员可以检查&#x200B;**设置** > **系统** > **OAuth2**&#x200B;下的OAuth2应用程序列表，以查看当前注册的内容。 有关信息，请参阅[查看和管理自定义OAuth2应用程序](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md)。

## 了解Adobe Developer Console身份验证类型

Adobe Developer Console支持多种身份验证方式。 您可以选择与集成的工作方式匹配的类型：

* **服务器到服务器身份验证**：对于在后端运行的应用程序，该应用程序代表您的组织调用Adobe API，不涉及最终用户。 这是与使用客户端ID和密钥的旧版Workfront OAuth2模式最接近的匹配项，也是大多数自定义Workfront集成、脚本和自动化应使用的类型。
* **用户身份验证**：对于Adobe用户需要登录并授予同意，您的应用程序才能查看或编辑其数据的情况。 如果您的集成需要代表特定登录的Workfront用户（而不是整个组织）进行操作，请改用此类型。

  如果选择“用户身份验证”，则根据应用程序的体系结构，还有三个选项：

  * **OAuth Web应用程序**：用于具有前端UI和后端服务器的应用程序。 服务器安全地存储客户端密钥并获取令牌。
  * **OAuth单页应用程序**：用于没有后端服务器的仅用于浏览器的Web应用程序。 Web应用程序本身会获取令牌。
  * **OAuth本机应用程序**：用于本机在设备上运行而没有后端服务器的移动或桌面应用程序。 本机应用程序会获取令牌。

从旧版OAuth2服务迁移后端集成、脚本或自动化的大多数组织都需要服务器到服务器身份验证。

## 功能比较：旧版OAuth2与Adobe Developer Console

旧版Workfront OAuth2服务（源位于&#x200B;**Setup** > **System** > **OAuth2应用程序**）提供三种应用程序类型，限制每个Workfront实例最多有10个OAuth2应用程序。 下面是这些方面与Adobe Developer Console的比较：

| 旧版Workfront类型 | 流量/身份验证方法 | Developer Console等效项 | 适合 |
|---|---|---|---|
| 机器对机器应用程序（CLI、守护程序、后端脚本） | 包含公钥/私钥对的JWT | 服务器到服务器身份验证 | 与不涉及最终用户的目的相同，但机制发生了变化。 旧版流使用公钥/私钥对和JWT，而服务器到服务器则通过OAuth客户端凭据授权使用客户端ID和客户端密钥。 这不是插入式凭据交换。 需要更改集成的身份验证代码，而不仅仅是凭据值。 有关信息，请参阅[为自定义OAuth 2应用程序使用JWT流程](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md)。 |
| Web应用程序（服务器端应用程序：Go、Java、.NET、Node、PHP） | OAuth 2.0授权代码流 | OAuth Web应用程序（在用户身份验证下） | 最接近的1:1匹配。 它具有相同的流和后端服务器存储客户端密钥的基本形状。 有关信息，请参阅自定义OAuth 2应用程序的[授权代码流](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md)。 |
| 单页Web应用程序(JS、Angular、React、Vue) | 使用PKCE的授权码流，无客户端密码 | OAuth单页应用程序（在用户身份验证下） | 最接近的1:1匹配此流量与基于PKCE的无密码流量相同。 有关信息，请参阅[为OAuth 2应用程序使用PKCE流程](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md)。 |
| （无旧版等效项） | — | OAuth本机应用程序（在用户身份验证下） | 这是一项新功能。 旧版Workfront OAuth2没有用于本机移动设备或桌面应用程序的专用类型。 |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## 迁移过程

### 如果您是Workfront系统管理员

>[!NOTE]
>
>如果您是Workfront产品管理员而不是组织管理员，则需要与组织管理员合作来完成此迁移，或请求进行迁移。

1. 登录到[developer.adobe.com](https://developer.adobe.com)并创建新项目。 项目是控制台组织不同集成或客户端应用程序的方式。
1. 从项目中，添加API，然后选择&#x200B;**Adobe Workfront**。 此API位于Experience Cloud类别下。 所有Workfront API（包括规划、工作流以及审阅和批准）共享此单个API。
1. 选择&#x200B;**服务器到服务器**&#x200B;身份验证选项，如果IMS组织有多个Workfront实例，请选择正确的实例。

   有关选择身份验证类型的指导，请参阅本文中的[了解Adobe Developer Console身份验证类型](#understand-adobe-developer-console-authentication-types)。
1. 在“项目”页面上，打开新的OAuth服务器到服务器凭据的详细信息，以查找您的客户端ID、客户端密钥和生成访问令牌所需的信息。
1. 更新您的集成、脚本或工具以使用这些新凭据进行身份验证，而不是使用旧的Workfront OAuth2客户端ID和密码。
1. 在Workfront中确认访问权限。 创建API客户端会自动将其添加为Workfront用户“`techacct`”。 默认情况下，该用户会被添加为具有有限访问权限的参与者，但您可以像对任何其他用户一样调整其访问级别。
1. （可选）要授予`techacct`用户管理员权限，请添加技术帐户的电子邮件作为Admin Console中相关产品配置文件的管理员。
1. 端到端测试集成。
1. 确认新连接正常工作后，在Workfront中弃用旧的OAuth2应用程序条目。

有关完整的分步详细信息和屏幕截图，请参阅Adobe Developer Console文档中的[获取访问权限](https://developer.adobe.com/workfront-apis/guides/gaining_access/)。

### 如果您不是系统管理员

由于在Adobe Developer Console中设置新凭据需要该级别的访问权限，因此您需要在组织的IMS组织管理员中循环完成迁移。 如果您管理或维护集成，但又知道组织的IMS组织管理员是谁，请联系以下人员之一：

* 您的Workfront客户团队
* 您的内部IT团队
* 您的工程联系人

## 如果不迁移

在2027年2月1日之后仍使用旧版OAuth2客户端ID/密码模式的集成停止能够针对Workfront API进行身份验证，并且任何依赖的工作流、同步或自动化失败。 由于此日期之后没有计划进行任何扩展，因此请提前很长时间迁移您的集成。

## 常见问题

**这是否会影响Adobe提供的打包集成，如Slack或Microsoft Teams？**

不可以。 Adobe管理的全局应用程序正由Adobe直接迁移，无需您自行操作。

**我现有的集成是否将在2027年2月1日之前停止工作？**

不可以。 现有自定义OAuth2应用程序在2027年2月1日之前继续正常运行。 自2026年11月1日起，只有创建新的自定义OAuth2应用程序的功能会受到影响。

**迁移是否需要付费？**

不会，通过Adobe Developer Console进行身份验证不会产生额外费用。

**我可以在哪里获得帮助？**

如果您对特定集成或时间线有任何疑问，请联系您的Workfront客户团队或开立支持案例。 有关包含屏幕截图的最新官方设置演练，请参阅Adobe的Developer Console文档中的[获取访问权限](https://developer.adobe.com/workfront-apis/guides/gaining_access/)。
