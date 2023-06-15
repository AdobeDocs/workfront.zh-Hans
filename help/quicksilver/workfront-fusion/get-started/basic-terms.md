---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的基本术语
description: 除了Adobe Workfront许可证，Adobe Workfront Fusion还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: b911af09c6df14f6504f6fc06adcf1f3a6d2626b
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 中的基本术语 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除了许可证外， [!UICONTROL Adobe Workfront] 许可证。


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td>一个模块，允许您在选定的应用程序或服务中读取或写入捆绑包。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL汇总]</p> </td> 
   <td> <p>一种模块，可将多个捆绑包（多个数据阵列）合并到一个捆绑包中。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[！UICONTROL Adobe Workfront Fusion]中的[！UICONTROL Aggregator]模块</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 密钥</td> 
   <td>唯一代码，用于标识调用软件API（用于身份验证）的用户、开发人员或程序。 从 [!DNL Adobe Workfront Fusion] 模块通过连接API工作，API密钥有时是必需的。 API密钥由需要它们的应用程序分发。 例如，如果您需要 [!DNL ActiveCampaign]，您可以通过贵机构的 [!DNL ActiveCampaign] 帐户。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">应用程序或服务</td> 
   <td> <p>最常见的软件应用程序。</p> <p>应用程序也可以是处理数据的特殊功能，例如迭代器或聚合器。 </p> <p>服务是捆绑包的来源，这些捆绑包可能包括Web API、网页、不同类型的服务器(FTP、SMTP、IMAP)等。 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">应用程序连接器</td> 
   <td>连接到其他系统的应用程序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>捆绑</p> </td> 
   <td> <p>捆绑是由模块返回或接收的基本单元。 捆绑包由项组成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL连接]</p> </td> 
   <td> <p>将应用程序或服务添加到场景时，您很可能必须先创建以下两者之间的连接： [!DNL Workfront Fusion] 和应用程序或服务以检索或发送选定的数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">关于连接 [!DNL Adobe Workfront Fusion] 至应用程序或服务</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>周期</p> </td> 
   <td> <p>周期是指场景运行的两个阶段：操作和提交。 此方案可能包含一个或多个周期。 有关更多详细信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">场景执行、周期和阶段 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数据存储</p> </td> 
   <td> <p>一种工具，用于存储方案中的数据，或允许您在单个方案或方案运行之间传输数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">[！UICONTROL Adobe Workfront Fusion]中的数据存储</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数据传输</p> </td> 
   <td> <p>通过您的方案传输的数据量。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">[！UICONTROL Adobe Workfront Fusion]中的场景详细信息</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>筛选</p> </td> 
   <td> <p>可在两个模块之间应用的附加功能。 过滤器允许您只使用符合特定条件的包。 您可以应用许多不同的过滤器。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">向[！UICONTROL Adobe Workfront Fusion]中的场景添加筛选器</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>用于唯一标识捆绑包的名称。 ID通常用于区分要从给定服务中更新或删除的捆绑包。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>项</p> </td> 
   <td> <p>包的一部分。 捆绑包可以包含多个项目。 有多种不同类型的项目：文本、数字、布尔值（是/否）、日期、时间、缓冲区（二进制数据）、集合、选择菜单、数组和验证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL迭代器]</p> </td> 
   <td> <p>一种模块类型，允许您获取一个数据捆绑（一个数据数组）并划分为单独的捆绑包。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[！UICONTROL Iterator]模块 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>模块</p> </td> 
   <td> <p>方案中的单一步骤，在关联的应用程序或服务中执行功能，例如创建记录。</p> <p>每个应用程序或服务都有各种模块，这些模块定义了它响应请求的方式。</p> <p>模块有4种类型：操作、触发器、迭代器和聚合器。</p> <p> <img src="assets/module.jpg"> </p> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模块类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td> <p>模块执行的任务。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">公钥/私钥</td> 
   <td>公钥和私钥用于对数据进行加密和解密。 公钥可以分发，任何拥有公钥的人都可以加密数据，但只有私钥可以解密。 同样，具有私钥的用户可以加密任何具有公钥的用户都可以解密的数据。 私钥加密可确保数据来自私钥的所有者，并用作数据来源的验证。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[！UICONTROL路由器]</p> </td> 
   <td>允许您复制数据或向场景添加新路由，以便重新路由数据并单独处理不同的数据组。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">中的[！UICONTROL Router]模块 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>方案</p> </td> 
   <td> <p>用户创建的一系列自动化步骤，每个步骤都由一个模块表示和执行。 场景的目的是移动和处理数据。</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[！UICONTROL Adobe Workfront Fusion]中创建方案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>交易</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 使用事务处理捕获方案生命周期。 事务由多个阶段组成，在这些阶段中，数据从一个一致状态转换为另一个一致状态。 有4个阶段：初始化、操作（读取或写入）、提交/回滚和最终化。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>触发器</p> </td> 
   <td> <p>一个模块，允许您抓取自上次运行场景以来添加或更新过的捆绑包。 有两种类型的触发器：轮询和即时(Webhook)。 有关更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>一种特殊类型的触发器，允许您在新捆绑包可用后立即运行场景。 有关更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">[！UICONTROL Adobe Workfront Fusion]中的即时触发器(Webhook)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
