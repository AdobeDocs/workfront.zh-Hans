---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion中的基本术语
description: Adobe Workfront Fusion除了需要Adobe Workfront许可证之外，还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# 中的基本术语 [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] 需要 [!DNL Adobe Workfront Fusion] 除 [!UICONTROL Adobe Workfront] 许可证。


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td>用于从选定的应用程序或服务中读取或写入包的模块。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL聚合器]</p> </td> 
   <td> <p>将多个包（多个数据数组）合并到一个包中的模块类型。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的[!UICONTROL Aggregator]模块</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API 密钥</td> 
   <td>唯一代码，用于标识调用软件API（用于身份验证）的用户、开发人员或程序。 自 [!DNL Adobe Workfront Fusion] 模块通过连接API来工作，API密钥有时是必要的。 API密钥由需要它们的应用程序分发。 例如，如果您需要API密钥， [!DNL ActiveCampaign]，您可以通过 [!DNL ActiveCampaign] 帐户。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">应用程序或服务</td> 
   <td> <p>最常用的软件应用程序。</p> <p>应用程序也可以是处理数据的特殊函数，如迭代器或聚合器。 </p> <p>服务是包的源，可能包含Web API、网页、不同类型的服务器(FTP、SMTP、IMAP)等。 </p> <p> <img src="assets/apps-350x420.jpg" style="width: 350;height: 420;"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">应用程序连接器</td> 
   <td>连接到其他系统的应用程序。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>捆绑</p> </td> 
   <td> <p>包是模块返回或接收的基本单元。 包由项目组成。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL连接]</p> </td> 
   <td> <p>在将应用程序或服务添加到方案时，您很可能必须首先在 [!DNL Workfront Fusion] 和应用程序或服务，以检索或发送所选数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">关于连接 [!DNL Adobe Workfront Fusion] 到应用程序或服务</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>周期</p> </td> 
   <td> <p>周期是指方案运行的两个阶段：操作和提交。 方案可能包含一个或多个周期。 有关更多详细信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">方案执行、循环和阶段(位于 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数据存储</p> </td> 
   <td> <p>一种工具，用于存储来自方案的数据，或允许您在单个方案或方案运行之间传输数据。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的数据存储</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数据传输</p> </td> 
   <td> <p>通过您的方案传输的数据量。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的方案详细信息</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>筛选</p> </td> 
   <td> <p>可在两个模块之间应用的其他功能。 然后，过滤器允许您仅使用符合特定条件的包。 您可以应用许多不同的过滤器。 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">向[!UICONTROL Adobe Workfront Fusion]中的方案添加过滤器</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>用于唯一标识包的名称。 ID通常用于区分要从给定服务中更新或删除的包。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>项</p> </td> 
   <td> <p>包的一部分。 包可以包含多个项目。 项目有多种不同类型：文本、数字、布尔值（是/否）、日期、时间、缓冲值（二进制数据）、集合、选择菜单、数组和验证。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL迭代器]</p> </td> 
   <td> <p>一种模块类型，允许您获取一个数据包（数据数组）并划分为多个单独的包。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">中的[!UICONTROL迭代器]模块 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>模块</p> </td> 
   <td> <p>方案中执行功能（例如，在关联的应用程序或服务中创建记录）的单个步骤。</p> <p>每个应用程序或服务都具有各种模块，用于定义它响应请求的方式。</p> <p>模块类型有4种：操作、触发器、迭代器和聚合器。</p> <p> <img src="assets/module.jpg"> </p> <p>有关更多信息，请参阅 <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">模块类型</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td> <p>由模块执行的任务。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">公钥/私钥</td> 
   <td>公钥和私钥用于加密和解密数据。 公钥可以分发，任何有公钥的人都可以加密数据，但只有私钥才能解密。 同样，具有私钥的用户可以加密任何具有公钥的人都可以解密的数据。 私钥加密确保数据来自私钥的所有者，并用于验证数据源。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>允许您复制数据或向方案添加新路由，以便重新路由数据并单独处理不同的数据组。 有关更多信息，请参阅 <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">中的[!UICONTROL Router]模块 [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>方案</p> </td> 
   <td> <p>用户创建的一系列自动化步骤，每个步骤由模块表示和执行。 方案的目的是移动和操作数据。</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> 有关更多信息，请参阅 <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">在[!UICONTROL Adobe Workfront Fusion]中创建方案</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>交易</p> </td> 
   <td> <p>[!DNL Workfront Fusion] 使用事务处理捕获方案生命周期。 事务由多个阶段组成，在这些阶段中，数据从一个一致状态转换为另一个一致状态。 共分4个阶段：初始化、操作（读或写）、提交/回滚和终止化。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>触发器</p> </td> 
   <td> <p>用于获取自上次运行方案以来添加或更新的包的模块。 触发器类型有2种：轮询和即时(webhooks)。 有关更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">中的即时触发器(Webhook) [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>网钩</p> </td> 
   <td> <p>一种特殊类型的触发器，允许您在新包可用后立即运行方案。 有关更多信息，请参阅 <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion]中的即时触发器(Webhooks)</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
