---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: 为用户配置共享设置
description: 作为Adobe Workfront管理员或Workfront校样管理员，您可以配置可与其共享校样的用户帐户，用户是否可以看到校样的所有版本，以及用户获得共享项目访问权限的时间。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# 为用户配置共享设置

作为Adobe Workfront管理员或Workfront校样管理员，您可以配置可与其共享校样的用户帐户，用户是否可以看到校样的所有版本，以及用户获得共享项目访问权限的时间。

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>当前计划：Pro或更高版本</p> <p>或</p> <p>旧版计划：Premium或Select</p> <p>有关使用不同计划校对访问权限的更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的校对功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>当前计划：工作或计划</p> <p>旧版计划：任意（必须为用户启用校样）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>您必须在校样权限配置文件中选择管理员。 有关更多信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">配置用户的校对访问权限</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 配置与其他帐户共享

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。

1. 单击 **设置** > **帐户设置**，然后单击 **设置** 选项卡。

1. 在 **共享** 的 **允许与共享**，单击 **设置**.

1. 在显示的下拉列表中，选择一个选项以指定您是希望向任何人提供校样，限制仅将校样共享到您自己的帐户，还是将校样限制到您自己的帐户以及您正在与之协作的任何合作伙伴帐户。
1. 单击 **保存。**

## 配置共享校样所有版本的可见性

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。

1. 单击 **设置** > **帐户设置**，然后单击 **设置** 选项卡。

1. 在 **共享** 的 **收件人可以查看所有版本**，选择 **启用** 或 **禁用** 来指示在启用校样URL后，是否允许收件人在校样查看器中查看校样的所有版本。

## 根据工作流阶段活动配置校样可见性

您可以指定与给定阶段关联的用户何时能够看到自动工作流的校样。

>[!NOTE]
>
>* 此选项仅在使用独立的Workfront校样应用程序时可用；当使用与Workfront集成的Workfront校样实例时，或在Workfront内进行校样时，此变量不可用。
>* 用户只有在校样进入与用户关联的阶段后（无论如何设置）才会收到有关校样的电子邮件通知。
>


要配置用户何时能够看到使用自动工作流进行校样：

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。

1. 单击 **设置** > **帐户设置**，然后单击 **设置** 选项卡。

1. 在 **共享** 部分，启用或禁用 **基于阶段激活的校样可见性**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>已禁用</strong> （默认）</td> 
      <td>在创建校样时，校样对用户可见。<br><p>在创建校样后，任何与校样工作流中的阶段关联的用户都可以在搜索结果中立即看到校样。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>已启用</strong> </td> 
      <td> <p>只有在用户关联的舞台变为 <strong>活动。</strong></p> <p><b>注释</b>:   
        <ul> 
         <li><em style="font-style: normal;">启用此选项后，现有校样仍对创建时可以查看该选项的用户可见。</em> </li> 
         <li>在用户获得对校样版本的访问权限（因为用户与之关联的舞台变为活动状态）后，用户只能查看激活了舞台的版本。 如果以前的版本从未达到与用户关联的阶段，则用户看不到该版本的校样。</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
