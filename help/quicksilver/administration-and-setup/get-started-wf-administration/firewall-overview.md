---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: 防火墙概述
description: 由于Adobe Workfront与贵组织的网络通信，因此贵组织的防火墙必须配置为允许该通信。 防火墙是一种高效的安全措施，通过将组织的网络与Internet分隔开来发挥作用。 它们可确保只有选定的数据和网络流量才能移入或移出组织的网络。 防火墙根据发送或接收数据的站点允许或阻止数据。 作为Adobe Workfront管理员，您必须确保发送到Workfront或从发送的数据可以通过贵组织的防火墙。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d74b0aa22644b7c79d3c6c3c3bbd5e67efdff732
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 防火墙概述

由于Adobe Workfront与贵组织的网络通信，因此贵组织的防火墙必须配置为允许该通信。 防火墙是一种高效的安全措施，通过将组织的网络与Internet分隔开来发挥作用。 它们可确保只有选定的数据和网络流量才能移入或移出组织的网络。 防火墙根据发送或接收数据的站点允许或阻止数据。 作为Adobe Workfront管理员，您必须确保发送到Workfront或从发送的数据可以通过贵组织的防火墙。

这可以通过允许列表实现，它实际上是“允许”通过防火墙发送或接收数据的站点的“列表”。 可以通过以下两种方式之一标识站点：

* **IP地址**：一系列数字，如52.31.132.175
* **域**：URL的一部分，如www.thisdomain.com中的“thisdomain”

Workfront使用特定的IP地址和域进行Web通信。 必须将这些组件添加到您组织的允许列表中，然后才能在您的组织中使用Workfront。

通常，允许列表由网络管理员配置。 与贵组织的网络管理员合作，确保您的防火墙允许这些IP地址。 如果您不知道网络管理员是谁，贵组织的IT部门可以引导您向正确的方向前进。

>[!IMPORTANT]
>
>作为Workfront列入允许列表管理员，您必须确保将这些IP地址和域添加到贵组织的中。 即使您自己不添加它们，也是如此。 Workfront无法配置您组织的允许列表。

## 收集用于配置防火墙的信息

要为Workfront配置防火墙，网络管理员需要知道要添加哪些IP地址和域。 这些信息中有一部分仅供Workfront管理员使用。 作为Workfront管理员，您必须找到此信息并将其提供给网络管理员。

>[!NOTE]
>
>确保安全性的最佳实践是仅添加与您的组织正在使用的功能相连的IP地址和域。 通过提供此信息，您可以确保遵循该最佳实践。

向网络管理员提供以下信息：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">允许的特定IP地址和域</td> 
   <td> <p>文章 <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">配置防火墙的允许列表</a> 列入允许列表包含贵组织必须添加到其的IP地址和域的列表。 </p> <p>您的网络管理员可能无权访问“配置防火墙”文章。 在这种情况下，您必须将其提供给他们。 我们不建议打印硬（纸张）副本。 使用数字副本，网络管理员可以复制并粘贴地址，这比从硬拷贝中键入更快、更准确。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的群集</td> 
   <td>要查找组织的群集，请参阅 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">查看贵组织的集群和Workfront计划</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的Workfront计划</td> 
   <td> <p>要查找贵组织的计划，请参阅 <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">查看贵组织的集群和Workfront计划。</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">您的域</td> 
   <td> <p>要查找您的域，请查看用于连接到Workfront的网址。</p> <p>示例：在网址中 <code>greatcompany.my.workfront.com</code>，则域为“greatcompany”</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他Adobe Workfront产品</td> 
   <td> <p>如果您拥有以下任意一项的许可证，请通知网络管理员：</p> 
    <ul> 
     <li> <p>Adobe Workfront Proof</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront集成</td> 
   <td>如果您使用以下任何一种方式，请通知网络管理员：
    <ul>
     <li><p><p>适用于Jira的Workfront</p></p></li>
     <li><p>适用于G Suite的Workfront</p></li>
     <li><p>适用于Microsoft Teams的Workfront</p></li>
     <li><p>适用于Outlook的Workfront</p></li>
     <li><p>适用于Salesforce的Workfront</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">其他功能</td> 
   <td> <p>如果您使用以下任一方式，请通知网络管理员：</p> 
    <ul> 
     <li> <p>Workfront试用方案</p> </li> 
     <li> <p>Workfront上升</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>如果以后添加这些产品、集成或功能，则必须联系网络管理员，以便他们调整允许列表。

### 查看贵组织的集群和Workfront计划 {#view-your-organization-s-cluster-and-workfront-plan}

1. 单击 **主菜单** 图标 ![](assets/main-menu-icon.png) (在Adobe Workfront的右上角)，然后单击 **设置** ![](assets/gear-icon-settings.png).

1. 单击 **系统** 在左侧面板中
1. 要查看群集，请选择 **客户信息**.

   您的集群显示在 **基本信息** 部分。

   ![](assets/locate-cluster.png)

1. 要查看您的Workfront计划，请选择 **许可证**.

   您的计划将在页面底部附近显示。

   ![](assets/locate-plan.png)
