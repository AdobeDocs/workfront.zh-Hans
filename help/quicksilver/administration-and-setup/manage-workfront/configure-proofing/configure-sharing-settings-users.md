---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 配置用户的共享设置
description: 作为Adobe Workfront管理员或Workfront Proof管理员，您可以配置用于共享验证的用户帐户，配置用户是否可以查看验证的所有版本，以及配置用户获得共享项目访问权限的时间。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# 配置用户的共享设置

作为Adobe Workfront管理员或Workfront Proof管理员，您可以配置用于共享验证的用户帐户，配置用户是否可以查看验证的所有版本，以及配置用户获得共享项目访问权限的时间。

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

## 配置与其他帐户的共享

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 在&#x200B;**共享**&#x200B;部分中，**允许与**&#x200B;共享，请单击&#x200B;**设置**。

1. 在出现的下拉列表中，选择一个选项，以指定您是否希望验证可供任何人使用、将验证共享限制在您自己的帐户上，或将其限制在您自己的帐户以及与您合作的任何合作伙伴帐户上。
1. 单击&#x200B;**保存。**

## 配置共享验证所有版本的可见性

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 在&#x200B;**共享**&#x200B;部分中，**收件人可以查看所有版本**&#x200B;的右侧，选择&#x200B;**启用**&#x200B;或&#x200B;**禁用**，以指示在启用了校对URL时，是否允许收件人查看校对查看器中的所有校对版本。

## 根据工作流暂存活动配置验证可见性

您可以指定与给定阶段关联的用户，何时能够看到具有自动工作流的验证。

>[!NOTE]
>
>* 此选项仅在使用独立的Workfront Proof应用程序时可用；在使用与Workfront集成的Workfront Proof实例或在Workfront中进行验证时不可用。
>* 无论此设置如何，用户只有在进入与用户关联的阶段后，才会收到有关验证的电子邮件通知。
>

要配置用户何时可看到具有自动工作流的验证，请执行以下操作：

1. 在Workfront中，单击主菜单![](assets/main-menu-icon.png)，然后单击验证![](assets/proofing-in-main-menu.png)以访问Workfront Proof。

1. 单击&#x200B;**设置** > **帐户设置**，然后单击&#x200B;**设置**&#x200B;选项卡。

1. 在&#x200B;**共享**&#x200B;部分中，启用或禁用基于阶段激活&#x200B;**的**&#x200B;校对可见性。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>已禁用</strong>（默认）</td> 
      <td>在创建验证时，验证对用户可见。<br><p>与验证工作流中某个阶段关联的任何用户都可以在创建验证后立即在搜索结果中查看验证。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>已启用</strong> </td> 
      <td> <p>只有在用户关联的阶段变为<strong>活动状态后，用户才能看到验证。</strong></p> <p><b>注释</b>：   
        <ul> 
         <li><em style="font-style: normal;">启用此选项后，现有验证仍对创建时可以查看该验证的用户可见。</em> </li> 
         <li>在用户获得对某个版本的验证的访问权限后（因为与用户关联的阶段变为活动状态），用户只能看到激活该阶段的版本。 如果以前的版本从未到达用户关联的阶段，则用户看不到该版本的验证。</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
