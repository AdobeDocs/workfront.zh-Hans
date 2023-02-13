---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: 配置防火墙的允许列表
description: 如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须向其添加特定IP地允许列表址。 这可打开您的环境与Adobe Workfront服务器之间的通信，并允许您的用户从Workfront发送消息，以及将单点登录(SSO)与Active Directory或LDAP结合使用。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 13%

---

# 配置防火墙的允许列表

>[!IMPORTANT]
>
>此页面中描述的过程仅适用于尚未载入Admin Console的组织。 如果贵组织已载入Adobe Admin Console，则必须通过Adobe Admin Console执行此操作。
>
>要配置允许列表您的组织是否已载入Adobe Admin Console，请参阅 [允许Adobe应用程序和服务的域](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>有关根据贵组织是否已载入Adobe Admin Console而有所不同的步骤列表，请参阅 [基于平台的管理差异(Adobe Workfront/Adobe业务平台)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

如果您的防火墙或邮件服务器配置为仅允许访问某些供应商，则必须向其添加特定IP地允许列表址。 这会打开您的环境与Adobe Workfront服务器之间的通信，并允许执行以下进程：

* 从Workfront应用程序发送消息

   >[!NOTE]
   >
   >如果贵组织的Workfront实例通过Adobe IMS启用，则此选项不可用。 如需详细信息，请咨询您的网络或IT管理员。

* 配置自定义文档集成时使用文档Web挂接
* 使用Workfront事件订阅

   有关更多信息，请参阅 [事件订阅API](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

您还需要打开某些端口，以便在发送电子邮件时对其进行加密。

## Workfront允许列表您可以使用

如果贵组织具有企业计划，则还可以配置两个Workfront允许列表:

* **电子邮件允许列表**:允许您控制用户可在何处通过电子邮件发送数据存储在Workfront中。 有关更多信息，请参阅 [配置电子邮件允许列表](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **IP允许列表**:将对Workfront的访问限制为您指定的45个IP地址或IP地址范围，为Workfront应用程序提供了额外的安全层。 有关更多信息，请参阅 [按IP地址限制对Adobe Workfront的访问](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## 要添加到的IP地允许列表址

您必须在防火墙上向添加允许列表的IP地址取决于生产环境运行的群集。 通过查看设置>系统>自定义信息，可以找到这是哪个群集。 有关更多信息，请参阅 [配置基本信息](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md#configuring-basic-info) 在文章中 [配置系统的基本信息](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

>[!IMPORTANT]
>
>启用Workfront后，某些集允许列表成将无法正常工作，因为无法使用静态IP地址配置它们。 要使用以下集成，您必须禁用允许列表。
>
>* Workfront for G Suite
>* Workfront for Outlook
>* Workfront for Salesforce


* [用于群集1、2、3、5、7、8和9的IP地址](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [允许群集4的IP地址](#ip-addresses-to-allow-for-cluster-4)
* [允许群集6的IP地址](#ip-addresses-to-allow-for-cluster-6)
* [允许测试驱动器的IP地址](#IP%20Addre2)
* [实施事件订阅时允许使用的IP地址](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [用于增强身份验证的IP地址](#ip-addresses-to-allow-for-enhanced-authentication)
* [要添加以访问Workfront Fusion的IP地址](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [要添加以使用Workfront for Jira的IP地址](#ip-addresses-to-add-for-using-workfront-for-jira)
* [要添加以使用Workfront Ascent的IP地址](#ip-addresses-to-add-for-using-workfront-ascent)
* [要添加到所有聚类的URL Workfront](#urls-to-add-for-all-clusters-workfront)

### 用于群集1、2、3、5、7、8和9的IP地址 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

如果您的生产环境位于群集1、2、3、5或7上，则必须允许使用以下IP地址。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">对于SSO、文档Web挂接或其他功能</td> 
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
    </ul> <p>有关以下IP地址的信息，请参阅 <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md" class="MCXref xref">21.1版本中Adobe Workfront电子邮件的新IP地址</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 允许群集4的IP地址 {#ip-addresses-to-allow-for-cluster-4}

如果您的生产环境位于群集4上，请为SSO添加以下IP地址，记录Webhook集成，并从Workfront应用程序接收电子邮件：

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

有关以下IP地址的信息，请参阅 [21.1版本中Adobe Workfront电子邮件的新IP地址](../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md)

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
   <td role="rowheader">使用AWS电子邮件服务</td> 
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
 </tbody> 
</table>

### 允许测试驱动器的IP地址

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">使用测试驱动器时从Workfront应用程序接收电子邮件</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对于使用Test Drive时的SSO和文档WebHook集成</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>此地址还必须添加到您的允许列表中，以便用户从Workfront接收电子邮件。</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 实施事件订阅时允许使用的IP地址  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

对于所有环境，添加以下IP地址以从Workfront事件订阅接收负载。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 对于欧洲客户</td> 
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

### 用于增强身份验证的IP地址 {#ip-addresses-to-allow-for-enhanced-authentication}

添加以下IP地址以对预览或生产使用增强的身份验证。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">如果您的环境位于群集1、2、3、5、7、8或9上</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">如果您的环境位于群集4上</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### 要添加以访问Workfront Fusion的IP地址  {#ip-addresses-to-add-for-accessing-workfront-fusion}

将以下IP地址添加到您的允许列表，以启用Workfront Fusion访问您的系统。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe WorkfrontEU数据中心</td> 
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
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

此外，如果贵组织使用出站网络过滤，请将以下域添加到允许列表您的中，以启用系统访问Workfront Fusion。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe WorkfrontEU数据中心</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront美国数据中心</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>出站网络过滤不常见。 请咨询网络管理员，以了解您是否需要更新允许列表以适应此情况。

### 要添加以使用Workfront for Jira的IP地址 {#ip-addresses-to-add-for-using-workfront-for-jira}

将以下IP地址添加到您的允许列表，以使用Workfront进行Jira集成。

jira.workfront.com域也必须可以从公司服务器访问。 此域是必需的，因为它用作Workfront和Jira之间的中间件。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 对于欧洲客户</td> 
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

### 要添加以使用Workfront Ascent的IP地址 {#ip-addresses-to-add-for-using-workfront-ascent}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">通过Workfront Ascent访问Workfront培训资源</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">从Workfront Ascent接收电子邮件通知</td> 
   <td> 
    <ul> 
     <li>23.251.227.75</li> 
     <li>23.251.227.76</li> 
     <li>23.251.227.77</li> 
     <li>23.251.227.78</li> 
     <li>23.251.227.79</li> 
     <li>23.251.227.80</li> 
     <li>23.251.227.81</li> 
     <li>23.251.227.82</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 要添加以访问Workfront的域

如果贵组织使用叫客网络过滤，请将以下域添加到允许列表您的中，以启用系统访问Workfront。

>[!NOTE]
>
>出站网络过滤不常见。 请咨询网络管理员，以了解您是否需要更新允许列表以适应此情况。

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## 要添加到所有聚类的URL Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">允许在Workfront环境中显示帮助内容</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">要允许Workfront校样在任何群集上访问Workfront，请将这些环境添加到所有环境</td> 
   <td> 
    <ul> 
     <li>*.workfront.com — 在Workfront中查看校样时需要使用</li> 
     <li>*.proofhq.com — 在Workfront校样中查看校样时需要使用</li> 
     <li>*.proofhq.eu — 在Workfront校样中查看校样时需要使用</li> 
    </ul> <p><b>注释</b>:  <p>我们不支持将IP地址添加到您的允许列表以进行Workfront校样。 在Workfront迁到AWS后，这些量度变得非常活跃。 我们建议您仅允许Workfront校样域。</p> <p>如果在将这些域添加到您的时出现允许列表问题，而您需要IP地址，请联系Workfront客户支持。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## 用于访问Workfront校样的IP地址和URL

您必须将以下IP地址添加到您的允许列表，才能使用各种功能。

* [用于回调和Web捕获校样](#for-callbacks-and-webcapture-proofs)
* [对于传出电子邮件](#for-outgoing-email)

### 用于回调和Web捕获校样 {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US（Clusters 1、2、3、5和7）</td> 
   <td> 
    <ul> 
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
   <td role="rowheader">Prod-EU(Cluster 4)</td> 
   <td> 
    <ul> 
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
    </ul> <p><b>注意</b>:不再支持DNS服务器选项。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 对于传出电子邮件 {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US（Clusters 1、2、3、5和7）</p> </td> 
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
   <td role="rowheader">Prod-EU(Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## 要打开以获得最佳Workfront校样性能的端口

如果您在校样加载过程中遇到问题或在Workfront校样中无法工作，请打开以下端口：

* 5671
* 5672
* 15671

## 为加密电子邮件打开的端口

来自Workfront应用程序的电子邮件使用端口465和587加密。 如果您的邮件服务器不支持加密电子邮件，则使用端口25发送未加密的电子邮件。

## 来自Workfront支持的电子邮件通知

如果您未收到Workfront支持部门的电子邮件，请确保添加所需的Salesforce IP地址和域。 有关更多信息，请参阅Salesforce帮助文章，介绍Salesforce IP地址和允许的域。
