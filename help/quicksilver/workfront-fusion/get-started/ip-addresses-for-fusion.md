---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: 用于访问Adobe Workfront Fusion的IP地址
description: 除了Adobe Workfront许可证之外，Adobe Workfront Fusion还需要Adobe Workfront Fusion许可证。
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 55a4fda46f6d314c71d9ef98864b21b84f946b09
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 用于访问[!DNL Adobe Workfront Fusion]的IP地址

>[!NOTE]
>
>除[!DNL Adobe Workfront license]外，[!DNL Adobe Workfront Fusion]还需要[!DNL Adobe Workfront Fusion]许可证。

列入允许列表如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须将某些IP地址添加到其，以允许您的环境与[!DNL Adobe Workfront Fusion]之间的开放通信。

将以下IP地址添加到您的允许列表以使[!DNL Workfront Fusion]能够访问您的系统。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 欧盟数据中心</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美国数据中心</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li>
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] 在Microsoft Azure群集上</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

此外，如果贵组织使用出站网络过滤，请将以下域添加到您的以使您的允许列表能够访问Workfront Fusion。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 欧盟数据中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 美国数据中心</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] 在Microsoft Azure群集上</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>出站网络过滤不常见。 请咨询网络管理员，了解是否需要更新允许列表以适应环境。

列入允许列表 列入允许列表有关设置组织的详细信息，请参阅[配置防火墙的](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
