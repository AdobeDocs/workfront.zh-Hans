---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置防火墙的允许列表
description: 列入允许列表如果您的防火墙或邮件服务器配置为仅允许某些供应商访问，则必须将某些IP地址添加到其。 这将打开环境与Adobe Workfront服务器之间的通信，并允许用户从Workfront发送消息，以及在Active Directory或LDAP中使用SSO。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: ee4cf80bc69416e3224c895c1f04628432ce2f4c
workflow-type: tm+mt
source-wordcount: '1646'
ht-degree: 0%

---

# 配置防火墙的允许列表

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>本页中介绍的过程仅适用于尚未加入该Admin Console的组织。 如果贵组织已载入到Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>若要在贵组织已登记到Adobe Admin Console的情况下配置您的允许列表，请参阅[允许Adobe应用程序和服务的域](https://helpx.adobe.com/cn/enterprise/kb/network-endpoints.html)。
>
>有关因贵组织是否已登记到Adobe Admin Console而不同的过程列表，请参阅[基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)。

>[!NOTE]
>
>每个机构配置其允许列表的方式都是独一无二的。 与您的IT团队合作，确定贵组织的过程并实施这些补充内容。

列入允许列表如果您的防火墙或邮件服务器配置为仅允许某些供应商访问，则必须将某些IP地址添加到其。 这样可在您的环境与Adobe Workfront服务器之间打开通信，并允许以下流程：

* 从Workfront应用程序发送消息

  >[!NOTE]
  >
  >如果您组织的Workfront实例已启用Adobe IMS，则此项不可用。 如果需要更多信息，请咨询您的网络或IT管理员。

* 配置自定义文档集成时使用文档Webhook
* 使用Workfront事件订阅

  有关详细信息，请参阅[事件订阅API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680)。

您还需要打开某些端口，以便在发送电子邮件时对其进行加密。

## Workfront允许列表可供您使用

如果您的组织拥有企业计划，您还可以配置两个Workfront 列入允许列表：

* **电子邮件允许列表**：可让您控制用户通过电子邮件发送存储在Workfront中的数据的位置。 有关详细信息，请参阅[配置电子邮件允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md)。
* **IP 允许列表**：将对Workfront的访问限制为您指定的75个IP地址或IP地址范围，从而为Workfront应用程序提供额外的安全层。 有关详细信息，请参阅[通过IP地址限制对Adobe Workfront的访问](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md)。

## 找到Workfront群集

必须在防火墙上添加到允许列表的IP地址取决于运行生产环境的群集。

要查找组织的群集，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧导航中，单击&#x200B;**系统**，然后选择&#x200B;**客户信息**。
1. 在页面的右上角找到&#x200B;**群集设置**&#x200B;字段。 此处列出了您组织的群集。

   CL01指的是Cluster 1，CL02指的是Cluster 2，依此类推。

有关详细信息，请参阅[防火墙概述](../../administration-and-setup/get-started-wf-administration/firewall-overview.md)一文中的[查看组织的群集和Workfront计划](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan)部分。

## 要添加到允许列表的IP地址

>[!IMPORTANT]
>
>某些Workfront集成在启用允许列表时不起作用，因为它们不能使用静态IP地址进行配置。 列入允许列表若要使用以下集成，必须禁用。
>
>* 适用于Google的Workfront Workspace
>* 适用于Outlook的Workfront
>* 适用于Salesforce的Workfront

* 允许群集1、2、3、5、7、8和9[&#128279;](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)的IP地址
* 允许群集4[&#128279;](#ip-addresses-to-allow-for-cluster-4)的IP地址
* 允许群集6[&#128279;](#ip-addresses-to-allow-for-cluster-6)的IP地址
* [允许群集10的IP地址](#ip-addresses-to-allow-for-cluster-10)
* [允许使用测试驱动器的IP地址](#IP%20Addre2)
* 实施事件订阅时允许的[IP地址](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* 要添加[个IP地址以访问Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* 要添加以供使用Workfront for Jira的[个IP地址](#ip-addresses-to-add-for-using-workfront-for-jira)
* [要为Workfront的所有群集添加的URL](#urls-to-add-for-all-clusters-workfront)

### 允许群集1 、 2 、 3 、 5 、 7 、 8和9的IP地址 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

如果您的生产环境位于群集1、2、3、5、7、8或9上，则必须允许以下IP地址。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">对于SSO、文档Webhook或其他功能</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">从Workfront应用程序接收电子邮件</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>有关以下IP地址的信息，请参阅<a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Adobe Workfront 21.1版本的电子邮件新IP地址</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 允许群集4使用的IP地址 {#ip-addresses-to-allow-for-cluster-4}

如果您的生产环境位于群集4上，请为SSO添加以下IP地址，记录webhook集成，并接收来自Workfront应用程序的电子邮件：

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

有关以下IP地址的信息，请参阅[Adobe Workfront 21.1版本的电子邮件新IP地址](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23.251.239.98
* 23.251.239.99

### 允许群集6的IP地址 {#ip-addresses-to-allow-for-cluster-6}

如果您的生产环境位于群集6上，请添加以下IP地址。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">从Workfront应用程序接收电子邮件</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">使用电子邮件服务</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">使用Mailgun电子邮件服务</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 允许群集10的IP地址

* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

### 用于允许测试驱动器的IP地址

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">使用试用版时从Workfront应用程序接收电子邮件</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对于使用测试驱动时的SSO和文档webhook集成</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188：</p> <p>还必须将此地址添加到您的允许列表，以便您的用户接收来自Workfront的电子邮件。</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 实施事件订阅时允许的IP地址  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

对于所有环境，请添加以下IP地址以从Workfront事件订阅接收负载。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 适用于欧洲客户</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对于位于欧洲以外地区的客户</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 要添加的用于访问Workfront Fusion的IP地址  {#ip-addresses-to-add-for-accessing-workfront-fusion}

将以下IP地址添加到您的允许列表，以使Workfront Fusion能够访问您的系统。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU数据中心</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront美国数据中心</p> </td> 
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

此外，如果贵组织使用出站网络过滤，请将以下域添加到您的以使您的允许列表能够访问Workfront Fusion。 这些URL用于Fusion中的Webhook。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU数据中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront美国数据中心</p> </td> 
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

### 要使用Workfront for Jira添加的IP地址 {#ip-addresses-to-add-for-using-workfront-for-jira}

将以下IP地址添加到您的允许列表以使用Workfront for Jira集成。

jira.workfront.com域还必须可从您的公司服务器访问。 此域是必需的，因为它用作Workfront和Jira之间的中间件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 适用于欧洲客户</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对于位于欧洲以外地区的客户</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 用于访问Workfront的添加域

如果贵组织使用出站网络过滤，请将以下域添加到您的允许列表中，以使您的系统能够访问Workfront。

>[!NOTE]
>
>出站网络过滤不常见。 请咨询网络管理员，了解是否需要更新允许列表以适应环境。

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* fonts.gstatic.com
* dpm.demdex.net
* storage.googleapis.com
* *.aptrinsic.com
* *.static.workfront.com


  这是一个静态域，其中涵盖了以下所有域。 如果您愿意，可以添加单个域：

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com

如果您的组织使用Unified ExperienceAdobe，则它会使用以下域。 这些域包含在`*.adobe.com`中，但可以根据需要添加。

* &lt;您的域>.my.workfront.adobe.com
* &lt;您的域>.preview.workfront.adobe.com
* &lt;您的域>.sb01.workfront.adobe.com
* &lt;您的域>.sb02.workfront.adobe.com


对于Workfront Fusion，请添加以下域：

* 对于不在Unified ExperienceAdobe上的组织：
   * app.workfrontfusion.com (美国AWS)
   * app-eu.workfrontfusion.com (欧盟AWS)
   * app-az.workfrontfusion.com (US Azure)

* 对于AdobeUnified Experience上的组织
（这些域包含在`*.adobe.com`中，但如果需要，可以添加。）

   * fusion.adobe.com
   * app-eu.fusion.adobe.com
   * app-az.fusion.adobe.com



## 要为Workfront的所有群集添加的URL {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">允许在您的Workfront环境中显示帮助内容</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">要允许Workfront Proof访问任何群集上的Workfront，请将这些群集添加到所有环境中</td> 
   <td> 
    <ul> 
     <li>*.workfront.com — 需要在Workfront中查看验证</li> 
     <li>*.proofhq.com — 需要在Workfront Proof中查看验证</li> 
     <li>*.proofhq.eu — 需要在Workfront Proof中查看验证</li> 
    </ul> <p><b>注释</b>：  <p>我们不支持向您的Workfront Proof允许列表添加IP地址。 在Workfront迁移到AWS后，这些指标一直处于动态状态。 为此，我们建议您仅允许Workfront Proof域。</p> <p>如果将这些域添加到允许列表时出现问题，您需要改用IP地址，请联系Workfront客户支持。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 要添加的用于访问Workfront Proof的IP地址和URL

必须将以下IP地址添加到允许列表中，才能使用各种功能。

* [对于回调和Webcapture校样](#for-callbacks-and-webcapture-proofs)
* [用于传出电子邮件](#for-outgoing-email)

### 对于回调和Webcapture校样 {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US（群集1、2、3、5和7）</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU（集群4）</td> 
   <td> 
    <ul> 
    <li>34.255.252.190</li>
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>注意</b>：不再支持DNS服务器选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 用于传出电子邮件 {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US（群集1、2、3、5和7）</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU（集群4）</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 打开端口以实现最佳的Workfront Proof性能

如果您在加载校样时遇到问题或无法在Workfront Proof中使用，请打开以下端口：

* 5671
* 5672
* 15671

## 为加密电子邮件打开的端口

来自Workfront应用程序的电子邮件使用端口465和587进行加密发送。 如果您的邮件服务器不支持加密电子邮件，则使用端口25不加密地发送电子邮件。

## 来自Workfront支持的电子邮件通知

如果您没有收到来自Workfront支持的电子邮件，请确保添加所需的Salesforce IP地址和域。 有关更多信息，请参阅有关Salesforce IP要允许的地址和域的Salesforce帮助文章。
