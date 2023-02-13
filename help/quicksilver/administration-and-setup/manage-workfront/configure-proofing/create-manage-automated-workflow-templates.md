---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 创建和管理自动化工作流模板
description: 作为Adobe Workfront管理员，如果贵组织的内容审阅过程经常重复，或内容经常由同一人员审阅，则可以创建自动工作流模板，其中包含那些具有您指定的校样角色和通知设置的审阅人。 自动化工作流模板可以很简单，只需一个或两个审阅人，或者复杂且包含许多阶段和依赖项。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '2096'
ht-degree: 0%

---

# 创建和管理自动化工作流模板

作为Adobe Workfront管理员，如果贵组织的内容审阅过程经常重复，或内容经常由同一人员审阅，则可以创建自动工作流模板，其中包含那些具有您指定的校样角色和通知设置的审阅人。 自动化工作流模板可以很简单，只需一个或两个审阅人，或者复杂且包含许多阶段和依赖项。

自动工作流模板使用自动工作流轻松创建校样。 当用户创建校样时，他们只需选择所需的模板即可。

您可以随时轻松更改任何自动化工作流模板，以添加或删除审阅人和阶段。 使用模板的校样创建者可以添加或删除校样的审阅者。

使用自动化工作流模板时，请考虑以下事项：

1. 自动工作流模板的设置决定了您可以使用自动工作流进行校样的操作。 例如，如果模板中禁用了添加阶段按钮，则当您使用校样的自动工作流设置时，该按钮将不可见。
1. 当某人在自动工作流模板中添加到页面，但已作为校样的审阅人存在时，应用该模板会将审阅人从舞台中删除。 如果不将其他审阅人添加到舞台，则会显示一条消息，提示您添加一个审阅人。
1. 您能否修改自动工作流模板取决于由Workfront管理员配置的模板设置，如中所述。 如果禁用了修改模板的功能，则只有模板的所有者才能修改模板。

有关自动化工作流的信息，请参阅 [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

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

## 创建自动化工作流模板

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。
1. 单击 **工作流** 中。
1. 在 **工作流** ，单击 **新建** > **新模板**.

1. 在 **详细信息** ，请指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">模板名称</td> 
      <td>（必需）键入模板的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板所有者</td> 
      <td>您可以选择将管理模板的Workfront管理员或Workfront校样管理员。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板组</td> 
      <td> <p> 如果贵组织的自动化工作流被组织为组，则可以选择组的名称。 请参阅 <a href="#create-automated-workflow-template-groups" class="MCXref xref">创建自动化工作流模板组</a> 更多信息，请参阅本文的后面部分。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">模板时区 </td> 
      <td> <p>模板的默认时区就是您正在使用的时区。 如果将使用模板的校样创建者和审阅者的时区不同，您可以在此处更改该时区，以确保在适当的时间为这些用户设置阶段截止日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许</td> 
      <td> <p>您可以选择希望人员可以使用的阶段活动，并使用模板创建校样。</p> <!--
        <p><b>WARNING</b>: If you don't select the options Add a stage and Add people to stages, neither the template owner nor the owner of any proof using this template will be able to add a stage or share the proof. <!--
          <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Test this. Andrzej thinks it's wrong info or a bug.</span>
         --></p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **阶段** 部分，配置自动化工作流模板的每个阶段。

   您可以添加多个阶段并在它们之间创建。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>阶段名称显示在“工作流”部分顶部的“自动工作流”图表、“校样详细信息”页面以及发送给审阅人的电子邮件通知中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">激活阶段</td> 
      <td> <p>指定是自动还是手动激活舞台。 对于第一个阶段，您可以选择 <strong>论校样创建</strong>, <strong>特定日期和时间</strong>或 <strong>手动</strong>.</p> <p>添加第二个阶段时，其他选项将变得可用，因为它们要求您选择父级阶段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">计算的截止日期</td> 
      <td> <p>指定您希望如何计算截止日期：</p> 
       <ul> 
        <li> <p><strong>校样创建</strong>:在下面的下拉列表中 <strong>截止时间（+工作日）</strong>，选择要添加到校样创建日期的工作天数，以自动设置校样的截止日期。</p> </li> 
        <li><strong>舞台开始时</strong>:在下面的下拉列表中 <strong>截止时间（+工作日）</strong>，选择要添加到阶段激活日期的工作天数，以自动设置校样的截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">锁台</td> 
      <td>指定是否允许锁定舞台以供评论。 选项是手动或自动锁定阶段，无论是在下一个阶段开始时还是在父阶段做出所有决策时。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要决策者</td> 
      <td> <p>只有在将审阅人添加到舞台后，才会在列表中显示可用的决策者。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需一个决定</td> 
      <td>一旦一名决策者提交其决定，就将完成阶段审查进程。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校样中配置校样设置</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">私人舞台</td> 
      <td>将中的评论和决策隐藏到未添加到舞台或非Workfront管理员的人员&lt;!&gt; — 在FLARE中起草：主管及以上

       -->. 有关更多信息，请参阅自&lt;a href=&quot;../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md&quot; class=&quot;MCXref xref&quot;>动化工作流概述&lt;/a>。&lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader">不允许删除此阶段</td> 
      <td> <p>将舞台设为强制舞台。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 如果将使用此模板的校样始终发送给舞台上的相同人员，请将其添加到此处，这样用户就不必在每次创建校样时都添加它们。

   选择每个人的 **角色** 在将使用此模板和 **电子邮件警报** 您希望用户在处理使用此模板的校样时收到该校样。

   有关校样角色的信息，请参阅 [配置默认校对角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). 有关校样电子邮件警报的信息，请参阅部分 [为用户配置校样默认值](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) 在文章中  [在Workfront校样中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   每个用户只能添加到一个阶段。 您可以添加任意所需数量的用户加入舞台。

   >[!TIP]
   >
   >您可以在阶段图上的各个阶段之间拖放审阅人名称。 可用阶段以蓝色突出显示。

1. 对要添加到模板的任何其他阶段重复上述两个步骤。

   在 **工作流** 部分，则可以看到您设置的自动化工作流程图。 继续添加阶段时，它们会显示在图表上，并有线条显示它们之间的依赖关系。 您可以单击图表中的某个阶段，以查看该阶段的设置。

   如果您不需要查看图表，可以单击 **隐藏图**.

1. 在 **共享模板** 部分中，单击一个选项（如果模板尚未与整个组织共享）以指定能够使用该模板的人员。

   默认情况下，新的自动化工作流模板会与组织中的每个人共享。

1. 单击&#x200B;**创建**。

## 修改自动化工作流模板

作为Workfront校样管理员，您可以修改自动工作流模板。 所做的更改会在您进行时自动保存。

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。
1. 单击 **工作流** 中。
1. 在 **工作流模板** 列表，单击要修改的模板。
1. 在 **详细信息** ，请指定以下信息：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">模板名称</td> 
      <td>（必需）键入模板的名称。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板所有者</td> 
      <td>您可以选择将管理模板的Workfront管理员或Workfront校样管理员。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板组</td> 
      <td> <p> 如果贵组织的自动化工作流被组织为组，则可以选择组的名称。 请参阅 <a href="#create-automated-workflow-template-groups" class="MCXref xref">创建自动化工作流模板组</a> 更多信息，请参阅本文的后面部分。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板时区 </td> 
      <td> <p>模板的默认时区就是您正在使用的时区。 如果将使用模板的校样创建者和审阅者的时区不同，您可以在此处更改该时区，以确保在适当的时间为这些用户设置阶段截止日期。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许</td> 
      <td> <p>选择希望使用模板创建校样的用户可以使用的阶段活动。 </p> <p><b>警告</b>:如果不选择添加阶段和将人员添加到阶段选项，则模板所有者和使用此模板的任何校样的所有者都将无法添加阶段或共享校样。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **工作流** 部分，更改任何阶段的名称并展开其设置 ![](assets/arrow-button.png) 进行任何所需的更改：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">计算的截止日期</td> 
      <td> <p>指定您希望如何计算截止日期：</p> 
       <ul> 
        <li> <p><strong>通过校样创建计算的截止时间</strong>:在 <strong>设置阶段截止时间</strong> 下拉列表中，选择要添加到校样创建日期的工作天数，以自动设置校样的截止日期。</p> </li> 
        <li><strong>从阶段激活计算的截止时间</strong>:在 <strong>设置阶段截止时间</strong> 下拉列表中，选择要添加到阶段激活日期的工作天数，以自动设置校样的截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">激活阶段</td> 
      <td> <p>指定是自动还是手动激活舞台。 对于第一个阶段，您可以选择 <strong>论校样创建</strong>, <strong>特定日期和时间</strong>或 <strong>手动</strong>.</p> <p>添加第二个阶段时，其他选项将变得可用，因为它们要求您选择父级阶段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">锁台</td> 
      <td>指定是否允许锁定舞台以供评论。 选项是手动或自动锁定阶段，无论是在下一个阶段开始时还是在父阶段做出所有决策时。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">决定</td> 
      <td>第一次一个决策者提交其决定时，这个阶段就结束了。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront校样中配置校样设置</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隐私</td> 
      <td>隐藏对未添加到舞台或帐户中非主管及以上人员的评论和决策。 有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">阶段删除</td> 
      <td>将舞台设为强制舞台。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">更多 <img src="assets/more-icon.png"></td> 
      <td>将审阅人添加到舞台或删除舞台。<p>如果您的每个校样在特定阶段被发送到同一个人，则可以在此处指定其名称，这样您就无需每次创建校样时都添加这些校样。 键入并选择要添加到舞台的用户名称，然后添加其 <strong>角色</strong> 证据和 <strong>电子邮件警报</strong> 设置。 有关校对角色的信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">配置默认校对角色</a>. 有关校样电子邮件警报的信息，请参阅部分 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">为用户配置校样默认值</a> 在文章中 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">在Workfront校样中配置电子邮件通知设置</a>.</p><p>您可以添加任意所需数量的用户以进入舞台</p><p>提示：您可以在阶段图上的各个阶段之间拖放审阅人名称。 可用阶段以蓝色突出显示。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 对要添加到模板的任何其他阶段重复该步骤。

   在 **工作流** 部分，则可以看到您设置的自动化工作流程图。 继续添加阶段时，它们会显示在图表上，并有线条显示它们之间的依赖关系。 您可以单击图表中的某个阶段，以查看该阶段的设置。

   如果您不需要查看图表，可以单击 **隐藏图**.

1. 在 **共享** ，请单击 ![](assets/more-icon.png) 按钮，然后单击 **删除**.

## 创建自动化工作流模板组 {#create-automated-workflow-template-groups}

作为Workfront管理员，您可以在组织的帐户中查看和管理所有自动化工作流模板。 将模板组织到组中会很有帮助。

要创建自动工作流模板组，请执行以下操作：

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。
1. 单击 **工作流** 中。
1. 在 **工作流** ，单击 **新建** > **新建模板组**.
1. 为新模板组键入一个描述性名称，然后按 **输入**.

您可以通过拖放在组之间移动模板。

## 管理自动化工作流模板

1. 在Workfront中，单击主菜单 ![](assets/main-menu-icon.png)，然后单击校对 ![](assets/proofing-in-main-menu.png) 访问Workfront校样。

1. 在Workfront校样的左侧面板中，单击 **工作流**.
1. 在 **工作流** ，请执行以下任一操作：

   * 添加新模板
   * 添加新模板组
   * 删除一个或多个模板组
   * 访问模板的详细信息
   * 将模板拖动到其他模板组
