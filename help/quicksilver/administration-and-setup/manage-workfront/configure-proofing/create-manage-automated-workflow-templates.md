---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: 创建和管理自动化工作流模板
description: 作为Adobe Workfront管理员，如果贵组织的内容审阅过程经常重复或内容经常由同一人员审阅，您可以创建自动工作流模板，其中包含具有您指定的验证角色和通知设置的审阅人。 自动化工作流模板可能很简单，只需一个或两个审阅人，也可能包含多个阶段和依赖项。
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: ccfea4cdf7280f992068bc64bab27e63aaab8b74
workflow-type: tm+mt
source-wordcount: '2056'
ht-degree: 0%

---

# 创建和管理自动化工作流模板

<!-- Audited: 2/2024 -->

作为Adobe Workfront管理员，如果贵组织的内容审阅过程经常重复或内容经常由同一人员审阅，您可以创建自动工作流模板，其中包含具有您指定的验证角色和通知设置的审阅人。 自动化工作流模板可能很简单，只需一个或两个审阅人，也可能包含多个阶段和依赖项。

使用自动化工作流模板，可以轻松创建具有自动化工作流的验证。 当用户创建验证时，他们只需选择所需的模板即可。

您可以随时轻松更改任何自动工作流模板，添加或删除审阅人和暂存。 使用该模板的验证创建者可以添加或删除验证的审阅人。

使用自动工作流模板时，请考虑以下事项：

1. 自动工作流模板的设置确定您可以使用自动工作流执行哪些操作以进行验证。 例如，如果在模板中禁用了添加暂存按钮，则当您使用验证的自动工作流设置时，该按钮将不可见。
1. 当有人在自动工作流模板中被添加到阶段，但也以审阅者身份出现在验证中时，应用模板会将审阅者从阶段中删除。 如果不将其他审阅人添加到阶段，则会显示一条消息，提示您添加审阅人。
1. 能否修改自动工作流模板取决于Workfront管理员配置的模板设置，如中所述。 如果禁用了修改模板的功能，则只有模板所有者可以修改模板。

有关自动化工作流的信息，请参阅 [自动化工作流概述](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## 访问要求

您必须具备以下条件：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>新建：任何</p><p>当前： Pro或更高版本</p><p>旧版：Premium或Select</p> <p>有关验证不同计划的访问权限的详细信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">访问Workfront中的验证功能</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td> <p>新增：标准</p><p>当前：工作或计划</p> <p>旧版：任意（您必须为用户启用验证）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须在验证权限配置文件中选择管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参见 [Workfront文档中的访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 创建自动化工作流模板

{{step1-to-proofing}}

1. 单击 **工作流** 在左侧面板中。
1. 在 **工作流** 选项卡，单击 **新建** > **新建模板**.

1. 在 **详细信息** 部分，指定以下信息：

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
      <td>您可以选择将管理模板的Workfront管理员或Workfront Proof管理员。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板组</td> 
      <td> <p> 如果贵组织的自动工作流划分为多个组，则可以选择组的名称。 请参阅 <a href="#create-automated-workflow-template-groups" class="MCXref xref">创建自动工作流模板组</a> 有关更多信息，请参阅本文后面的部分。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">模板时区 </td> 
      <td> <p>模板的默认时区是您正在使用的时区。 如果验证创建者和将使用该模板的审阅人的时区不同，您可以在此处更改它以确保为这些用户在正确的时间设置暂存截止时间。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许</td> 
      <td> <p>您可以选择希望人员可以使用模板创建验证的阶段活动。</p> 
      <p><b>警告</b>：如果未选择添加阶段和将人员添加到阶段选项，则模板所有者和使用此模板的任何验证的所有者将无法添加阶段或共享验证。 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **暂存** 部分，配置自动工作流模板的每个阶段。

   您可以添加多个阶段并在它们之间创建。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名称</td> 
      <td> <p>阶段名称显示在“工作流”部分顶部的自动工作流图中、验证详细信息页面上，以及发送给审阅人的电子邮件通知中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">激活阶段</td> 
      <td> <p>指定是自动激活阶段还是手动激活阶段。 对于第一个阶段，您可以选择 <strong>创建验证时</strong>， <strong>在特定日期和时间</strong>，或 <strong>手动</strong>.</p> <p>添加第二个阶段时，其他选项将变为可用，因为它们要求您选择父阶段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">截止日期计算自</td> 
      <td> <p>指定您希望如何计算截止日期：</p> 
       <ul> 
        <li> <p><strong>校对创建</strong>：在下拉列表中的 <strong>截止日期（+个工作日）</strong>，选择要添加到验证创建日期的工作日数以自动设置验证的截止日期。</p> </li> 
        <li><strong>阶段开始时</strong>：在下拉列表中的 <strong>截止日期（+个工作日）</strong>，选择要添加到阶段激活日期的工作日数以自动设置验证截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">锁定阶段</td> 
      <td>指定是否允许将舞台锁定以供评论。 选项包括手动或自动锁定阶段，无论是在下一阶段启动时还是在父级上做出所有决策时。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">主要决策者</td> 
      <td> <p>仅在将审阅者添加到舞台后，可用的决策制定者才会显示在列表中。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">只需一个决定</td> 
      <td>一旦决策人之一提交决定，该阶段的审查进程即告完成。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中配置验证设置</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">专用阶段</td> 
      <td>将中的评论和决策隐藏给未添加到阶段或不是Workfront管理员的用户。 有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">不允许删除此阶段</td> 
      <td> <p>将阶段设置为必需。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 如果始终将使用此模板的验证发送给阶段中的相同人员，请在此处添加它们，以便用户不必每次创建验证时都添加它们。

   选择每个人的 **角色** 在将要使用此模板和 **电子邮件警报** 您希望用户在处理使用此模板的验证时接收。

   有关验证角色的信息，请参阅 [配置默认验证角色](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). 有关验证电子邮件提醒的信息，请参阅部分 [为用户配置校对默认值](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) 在文章中  [在Workfront Proof中配置电子邮件通知设置](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   每个用户只能添加到一个阶段。 您可以向阶段添加所需数量的用户。

   >[!TIP]
   >
   >您可以在阶段图上的阶段之间拖放审阅者名称。 可用阶段以蓝色突出显示。

1. 对要添加到模板的任何其他阶段重复前两个步骤。

   在顶部 **工作流** 部分，您可以查看所设置的自动工作流的图表。 在继续添加阶段时，它们会显示在图表上，其中行显示它们之间的依赖关系。 您可以单击图中的某个阶段，以查看该阶段的设置。

   如果您不需要查看图，可以单击 **隐藏图表**.

1. 在 **共享模板** 部分中，单击某个选项（如果模板尚未与整个组织共享）以指定能够使用该模板的人员。

   默认情况下，新的自动工作流模板会与您组织中的每个人共享。

1. 单击 **创建**.

## 修改自动工作流模板

作为Workfront Proof管理员，您可以修改自动工作流模板。 所做的更改会在您进行时自动保存。

{{step1-to-proofing}}

1. 单击 **工作流** 在左侧面板中。
1. 在 **工作流模板** 在显示的列表中，单击要修改的模板。
1. 在 **详细信息** 部分，指定以下信息：

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
      <td>您可以选择将管理模板的Workfront管理员或Workfront Proof管理员。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板组</td> 
      <td> <p> 如果贵组织的自动工作流划分为多个组，则可以选择组的名称。 请参阅 <a href="#create-automated-workflow-template-groups" class="MCXref xref">创建自动工作流模板组</a> 有关更多信息，请参阅本文后面的部分。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">模板时区 </td> 
      <td> <p>模板的默认时区是您正在使用的时区。 如果验证创建者和将使用该模板的审阅人的时区不同，您可以在此处更改它以确保为这些用户在正确的时间设置暂存截止时间。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">允许</td> 
      <td> <p>选择您希望使用模板创建验证的用户可用的暂存活动。 </p> <p><b>警告</b>：如果未选择添加阶段和将人员添加到阶段选项，则模板所有者和使用此模板的任何验证的所有者将无法添加阶段或共享验证。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. 在 **工作流** 部分，更改任何阶段的名称并展开其设置 ![](assets/arrow-button.png) 要进行任何需要的更改，请执行以下操作：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">截止日期计算自</td> 
      <td> <p>指定您希望如何计算截止日期：</p> 
       <ul> 
        <li> <p><strong>从验证创建计算出的截止日期</strong>：在 <strong>设置阶段截止日期</strong> 下拉列表中，选择要添加到验证创建日期的工作日数以自动设置验证的截止日期。</p> </li> 
        <li><strong>从阶段激活计算的截止日期</strong>：在 <strong>设置阶段截止日期</strong> 在下拉列表中，选择要添加到阶段激活日期的工作日数以自动设置验证截止日期。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">激活阶段</td> 
      <td> <p>指定是自动激活阶段还是手动激活阶段。 对于第一个阶段，您可以选择 <strong>创建验证时</strong>， <strong>在特定日期和时间</strong>，或 <strong>手动</strong>.</p> <p>添加第二个阶段时，其他选项将变为可用，因为它们要求您选择父阶段。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">锁定阶段</td> 
      <td>指定是否允许将舞台锁定以供评论。 选项包括手动或自动锁定阶段，无论是在下一阶段启动时还是在父级上做出所有决策时。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">决定</td> 
      <td>第一次由决策人提交决策时结束。 有关更多信息，请参阅 <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">在Workfront Proof中配置验证设置</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">隐私</td> 
      <td>将中的评论和决策隐藏给未添加到舞台或帐户中不是主管或以上级别的人员。 有关更多信息，请参阅 <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">自动化工作流概述</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">阶段删除</td> 
      <td>将阶段设置为必需。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">更多 <img src="assets/more-icon.png"></td> 
      <td>将审阅人添加到舞台或删除舞台。<p>如果您的每个验证在特定阶段发送给相同的人员，您可以在此处指定他们的姓名，这样您就不必每次创建验证时都添加它们。 键入并选择要添加到阶段的用户的名称，然后添加其 <strong>角色</strong> 在证明和 <strong>电子邮件警报</strong> 用户所需的设置。 有关校对角色的信息，请参阅 <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">配置默认验证角色</a>. 有关验证电子邮件提醒的信息，请参阅部分 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">为用户配置校对默认值</a> 在文章中 <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">在Workfront Proof中配置电子邮件通知设置</a>.</p><p>您可以向阶段添加所需数量的用户</p><p>提示：您可以在阶段图上的阶段之间拖放审阅者名称。 可用阶段以蓝色突出显示。</p></td> 
     </tr> 
    </tbody> 
   </table>

1. 对要添加到模板的任何其他阶段重复该步骤。

   在顶部 **工作流** 部分，您可以查看所设置的自动工作流的图表。 在继续添加阶段时，它们会显示在图表上，其中行显示它们之间的依赖关系。 您可以单击图中的某个阶段，以查看该阶段的设置。

   如果您不需要查看图，可以单击 **隐藏图表**.

1. 在 **共享对象** 部分，如果要删除用户，请单击更多 ![](assets/more-icon.png) 按钮，然后单击 **移除**.

## 创建自动工作流模板组 {#create-automated-workflow-template-groups}

作为Workfront管理员，您可以查看和管理组织帐户中的所有自动工作流模板。 将模板组织到组中会很有用。

要创建自动化工作流模板组，请执行以下操作：

{{step1-to-proofing}}

1. 单击 **工作流** 在左侧面板中。
1. 在 **工作流** 选项卡，单击 **新建** > **新建模板组**.
1. 键入新模板组的描述性名称，然后按 **输入**.

可以通过拖放方式在组之间移动模板。

## 管理自动化工作流模板

{{step1-to-proofing}}

1. 在Workfront Proof的左侧面板中，单击 **工作流**.
1. 在 **工作流** 在出现的页面中，执行以下任一操作：

   * 添加新模板
   * 添加新模板组
   * 删除一个或多个模板组
   * 访问模板的详细信息
   * 将模板拖到其他模板组
