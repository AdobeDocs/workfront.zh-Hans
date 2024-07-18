---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 为组织配置校样设置
description: 作为Adobe Workfront管理员或Workfront Proof管理员，您可以自定义组织的默认校样设置。 这些设置包括默认共享选项、品牌等。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 0%

---

# 为组织配置校样设置

作为Adobe Workfront管理员或Workfront Proof管理员，您可以自定义组织的默认校样设置。 这些设置包括默认共享选项、品牌等。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：专业版或更高版本</p> <p>或</p> <p>旧版计划：Premium或Select</p> <p>有关使用其他计划进行验证访问的更多信息，请参阅<a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须在验证权限配置文件中选择管理员。 有关详细信息，请参阅<a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">配置用户的验证访问权限</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 配置操作

有关在校对查看器中使用操作的信息，请参阅[对校对评论使用操作](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)。

您可以通过以下方式为组织配置操作：

* [添加或重命名操作](#add-or-rename-an-action)
* [停用或重新激活操作](#deactivate-or-reactivate-an-action)
* [重新排序操作](#reorder-actions)

### 添加或重命名操作 {#add-or-rename-an-action}

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击Workfront Proof界面右上角的&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 执行以下任一操作：

   * 要创建新操作，请在&#x200B;**操作**&#x200B;部分中单击&#x200B;**新建操作**。

     您可以在帐户中设置的操作数量没有限制。

   * 若要重命名现有操作，请单击该操作旁边的&#x200B;**设置**。

1. 键入操作的名称，然后单击&#x200B;**保存**。
1. 单击&#x200B;**保存。**

### 停用或重新激活操作 {#deactivate-or-reactivate-an-action}

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击Workfront Proof界面右上角的&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 单击要取消激活或重新激活的操作旁边的&#x200B;**设置**。
1. 选择&#x200B;**激活**&#x200B;或&#x200B;**停用**，然后单击&#x200B;**保存**。

### 重新排序操作 {#reorder-actions}

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击Workfront Proof界面右上角的&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 单击&#x200B;**设置**&#x200B;旁边的蓝色上箭头和下箭头可重新排列操作。

   ![重新排序操作.png](assets/re-order-actions-350x103.png)

## 为验证配置自定义设备

您可以将任何自定义设备添加到系统中，从而允许用户查看交互式内容并模拟内容在特定设备上的显示方式。

有关用户在查看交互式内容时如何选择设备的信息，请参阅[在验证查看器中更改交互式验证分辨率](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

要添加自定义设备，请执行以下操作：

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击Workfront Proof界面右上角的&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 在&#x200B;**验证自定义设备**&#x200B;部分中，单击&#x200B;**添加新设备**。

1. 在出现的&#x200B;**添加新设备**&#x200B;框中，指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td>用户在桌面验证查看器中选择设备时看到的名称，如<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">更改验证查看器的交互式验证分辨率</a>中所述。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">维度</td> 
      <td>指定要用于此设备的尺寸。 用户会看到设备名称下方显示的维度。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">比例</td> 
      <td>指定设备的比率。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">类型</td> 
      <td>选择设备是移动设备、平板电脑还是桌面。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">用户代理字符串</td> 
      <td>输入设备的用户代理，提供使软件按照设备设计运行和显示的信息。<p>您可以从设备转到<a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a>获取用户代理。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">已禁用</td> 
      <td>如果选择此选项，则用户在查看交互式验证时无法选择设备。</td> 
     </tr> 
    </tbody> 
   </table>

1. 单击&#x200B;**创建**。

## 为验证配置弹出消息

您可以配置校样上的弹出消息，以将一般信息传达给组织中的所有审阅人。

您可以配置要在以下情况下显示的消息：

* **加载时消息**：在验证首次打开时显示。 用于向用户解释如何审查证明或者提供免责声明或其他法律文本。
* **决策消息**：用户为验证选择决策时显示。 用于为用户提供品牌或法规合规性等方面的核对清单。 有关决策的信息，请参阅[在验证查看者中做出校对决策](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)。

* **确认按钮文本**：在上面说明的“正在加载”弹出消息的按钮上显示的标签。

要为验证创建弹出消息，请执行以下操作：

1. 单击要自定义的消息右侧的&#x200B;**编辑**。
1. 指定邮件并包含相应的格式，然后单击&#x200B;**保存**。
1. （可选）如果您自定义了“加载时”消息并且还想自定义确认按钮标签，请单击&#x200B;**确认按钮文本**&#x200B;右侧的&#x200B;**编辑**，指定标签，然后单击&#x200B;**保存**。

## 配置校对默认值

有关为组织配置校对默认设置的信息，请参阅[配置默认校对设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md)。


## 配置共享默认值

您可以指定可与谁共享贵组织的验证，哪些版本可供审阅人使用，以及何时与给定阶段关联的用户能够查看使用自动工作流的验证。

有关在Workfront Proof中共享设置的更多详细信息，请参阅[为用户配置共享设置](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md)。

## 品牌化Workfront Proof网站

如果您使用的是Workfront Proof，则可以为网站的以下区域设置品牌策略：

* 加载验证时显示的启动页面
* 登录和注销屏幕
* 电子邮件通知

有关如何将Workfront Proof网站品牌化的详细信息，请参阅[将Workfront Proof网站品牌化](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md)。

## 配置高级密码设置

>[!IMPORTANT]
>
>此选项仅适用于旧版Workfront计划。 如果您使用Pro、Business或Enterprise Workfront计划，则无法再配置高级密码设置。

在&#x200B;**高级密码设置**&#x200B;下，您可以增强用户的密码安全性。

1. 单击要配置的设置右侧的&#x200B;**设置**：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">最小密码长度</td> 
      <td>默认的Workfront Proof密码长度为6个字符。 您可能希望增加此数量，具体取决于贵组织的策略。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>字符组合</strong> </td> 
      <td>您可以强制用户在其密码中混合使用小写、大写、数字和符号。 您可以决定密码应包含多少个字符。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>最大重复字符数</strong> </td> 
      <td>您可以指定每个用户的密码中可重复使用的字符数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">密码自动老化</td> 
      <td>强制用户定期更改其密码。 由您决定他们多久执行一次此操作。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>不允许密码重复次数</strong> </td> 
      <td>配置您的帐户中不允许的密码重复次数。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>配置文件锁定</strong> </td> 
      <td>在您指定的多次失败登录尝试后，将您的用户锁定在帐户之外。 您还可以指定他们再次访问帐户之前应等待的时间。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">如果密码未在30天后重置，则锁定用户</td> 
      <td>如果您的用户在激活用户档案后的30天内未更改其初始密码，则这些用户将被锁定在帐户之外。<br><p>帐户管理员可以解锁（重新激活）被系统自动锁定的用户。 这将为他们额外提供七天的时间来更改密码。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">如果120天未活动，则锁定用户帐户</td> 
      <td>如果您的用户120天内未登录Workfront Proof或登录所需的验证，则这些用户会锁在帐户之外。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>首次登录后更改密码</strong> </td> 
      <td>要求用户在首次登录后更改其临时密码。<p>帐户管理员可以解锁（重新激活）被系统自动锁定的用户。</p><p>有关密码的更多信息，请参阅<a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">登录并更改Workfront Proof的密码和电子邮件</a>。</p></td> 
     </tr> 
    </tbody> 
   </table>
