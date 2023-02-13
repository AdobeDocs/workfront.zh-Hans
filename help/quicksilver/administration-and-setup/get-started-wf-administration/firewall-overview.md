---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 防火墙概述
description: 由于Adobe Workfront与贵组织的网络进行通信，因此必须将贵组织的防火墙配置为允许该通信。 防火墙是一种高效的安全措施，可通过将组织的网络与Internet分离来发挥作用。 它们确保只有选定的数据和网络流量才能进入或退出组织的网络。 防火墙允许或阻止基于正在发送或接收数据的站点的数据。 作为Adobe Workfront管理员，您必须确保发送到Workfront或从发送的数据可以通过贵组织的防火墙。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# 防火墙概述

由于Adobe Workfront与贵组织的网络进行通信，因此必须将贵组织的防火墙配置为允许该通信。 防火墙是一种高效的安全措施，可通过将组织的网络与Internet分离来发挥作用。 它们确保只有选定的数据和网络流量才能进入或退出组织的网络。 防火墙允许或阻止基于正在发送或接收数据的站点的数据。 作为Adobe Workfront管理员，您必须确保发送到Workfront或从发送的数据可以通过贵组织的防火墙。

这是通过完允许列表成的，这实质上是“允许”通过防火墙发送或接收数据的站点的“列表”。 可以通过以下两种方式之一来识别网站：

* **IP地址**:一系列数字，如52.31.132.175
* **域**:URL的一部分，如www.thisdomain.com中的“此域”

Workfront使用特定的IP地址和域进行Web通信。 必须先将这些权限添加到贵组允许列表织的中，然后才能在组织中使用Workfront。

通常，网允许列表络管理员会配置。 与贵组织的网络管理员合作，确保防火墙允许这些IP地址。 如果您不知道网络管理员是谁，则贵组织的IT部门可以指向您正确的方向。

>[!IMPORTANT]
>
>作为Workfront管理员，您必须确保将这些IP地址和域添加到贵组织的允许列表。 即使您不自己添加，也是如此。 Workfront无法配置贵组织的允许列表。

## 收集有关配置防火墙的信息

要为Workfront配置防火墙，网络管理员需要知道要添加的IP地址和域。 其中某些信息仅供Workfront管理员使用。 作为Workfront管理员，您必须找到此信息并将其提供给您的网络管理员。

>[!NOTE]
>
>安全性的最佳实践是仅添加IP地址和域，这些地址和域连接到贵组织正在积极使用的功能。 通过提供此信息，您可以确保遵循此最佳实践。

向网络管理员提供以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">允许的特定IP地址和域</td> 
   <td> <p>文章 <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">配置防火墙的允许列表</a> 包含贵组织必须添加到其的IP地址和域允许列表列表。 </p> <p>网络管理员可能无权访问“配置防火墙”一文。 在这种情况下，您必须向他们提供。 我们不建议打印硬（纸）拷贝。 数字副本允许网络管理员复制并粘贴地址，这比从硬拷贝中键入地址更快、更准确。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的群集</td> 
   <td>要找到贵组织的群集，请参阅 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">查看贵组织的群集和Workfront计划</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的Workfront计划</td> 
   <td> <p>贵组织的计划如下所示：</p> 
    <ul> 
     <li> <p>企业 </p> </li> 
     <li> <p>业务 </p> </li> 
     <li> <p>Pro </p> </li> 
     <li> <p>团队 </p> </li> 
    </ul> <p>要查找计划，请参阅 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">查看贵组织的群集和Workfront计划。</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的域</td> 
   <td> <p>要找到您的域，请查看用于连接到Workfront的Web地址。</p> <p>示例：网址 <code>greatcompany.my.workfront.com</code>，则域为“greatcompany”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他Adobe Workfront产品</td> 
   <td> <p>如果您拥有以下任一许可证，请通知网络管理员：</p> 
    <ul> 
     <li> <p>Adobe Workfront校样</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront集成</td> 
   <td>如果您使用以下任一方法，请通知网络管理员：
    <ul>
     <li><p><p>Workfront为吉拉队</p></p></li>
     <li><p>Workfront for G Suite</p></li>
     <li><p>Workfront for Microsoft Teams</p></li>
     <li><p>Workfront for Outlook</p></li>
     <li><p>Workfront for Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他功能</td> 
   <td> <p>如果您使用以下任一方法，请通知网络管理员：</p> 
    <ul> 
     <li> <p>Workfront试驾</p> </li> 
     <li> <p>Workfront晋升</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>如果以后添加这些产品、集成或功能，则必须联系网络管理员以调整允许列表。

### 查看贵组织的群集和Workfront计划 {#view-your-organization-s-cluster-and-workfront-plan}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) 在Adobe Workfront的右上角，单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** 在左侧面板中
1. 要查看群集，请选择 **客户信息**.

   您的群集显示在 **基本信息** 中。

   ![](assets/locate-cluster.png)

1. 要查看Workfront计划，请选择 **许可证**.

   您的计划显示在页面底部附近。

   ![](assets/locate-plan.png)
