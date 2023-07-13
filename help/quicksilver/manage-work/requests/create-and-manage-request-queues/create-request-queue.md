---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建请求队列
description: 您可以设置请求队列，用户可以在其中输入未在项目上计划工作的临时请求。
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: ddb8f39e3ef400b02b443230f237b6a563d99d5f
workflow-type: tm+mt
source-wordcount: '2571'
ht-degree: 2%

---

# 创建请求队列

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

您可以设置请求队列，用户可以在其中输入未在项目上计划工作的临时请求。 例如，可以设置技术支持请求队列来捕获来到IT部门的所有用户请求。

## 访问要求

<!--drafted for P&P: replace the table below with this:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>Current license: Stadard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator
-->

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系

## 请求队列概述

您可以将请求队列设置为项目。 将项目指定为请求队列时，可以从Adobe Workfront的请求区域访问该队列。 在自定义请求队列时，您还可以自定义用户在提交请求时填写的表单。

本文介绍了如何从现有项目创建请求队列。 但是，要构建请求引入流程的一致性或向其中添加多个层以用于报告和更好的管理，您还可以配置请求队列的其他构建块，如下表所述。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">队列详细信息</td> 
   <td> <p>必须在队列详细信息区域将项目设置为请求队列。 此步骤是必需的。 </p> <p>欲了解更多信息，请参见 <a href="#create-a-request-queue" class="MCXref xref">创建请求队列</a> 章节。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">主题组</td> 
   <td> <p>它们是附加菜单，可根据常见功能对请求进行分类。 例如，对于IT请求队列，您可能需要“现场”和“远程”主题组。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">创建主题组</a>. </p> <p>这是可选的。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">队列主题</td> 
   <td> <p>它们是附加菜单，可根据常见功能对属于同一主题组的请求进行分类。 主题组可以包含多个队列主题。 </p> <p>例如，IT请求队列的“现场”主题组可能包含“硬件”、“软件”和“网络”队列主题。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">创建队列主题</a>. </p> <p>这是可选的。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">路由规则</td> 
   <td> <p>利用它们，可将每个请求路由到用户、工作角色、团队或项目。 </p> <p>有关更多信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">创建路由规则</a>. </p> <p>这是可选的。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 创建请求队列

将项目设置为请求队列时，项目状态必须为当前才能在Workfront的请求区域显示。

要创建请求队列，请执行以下操作：

1. 转到要设置为请求队列的项目。
1. （可选）单击 **项目详细信息** 在左侧面板中添加 **描述** 至中的项目 **概述** 区域。 此信息将显示在所有新请求中。
1. 单击 **队列详细信息** （在左侧面板中）。 您可能需要单击 **显示更多**，则 **队列详细信息**.

   这将打开队列详细信息部分。

   ![](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)

1. 指定以下信息：

   * **作为帮助请求队列发布：** 选择此选项可将此项目标识为请求队列。 所有传入问题都被视为请求。\
     如果未选择此选项，则项目的行为类似于Workfront中的标准项目，并且所有传入问题都是问题。

   * **可以将请求添加到此队列的人员：** 选择哪些用户有权向此队列添加请求。 您可以允许以下用户组在全局导航栏的“请求”区域中查看请求队列：

     | 谁可以输入请求 | 描述 |
     |---|---|
     | 任何人 | 任何拥有活动帐户的Workfront用户都可以查看此请求队列并向其添加请求 |
     | 拥有查看此项目的权限的用户 | 对项目具有查看权限的用户可以查看请求并将其添加到此队列 |
     | 在这个项目公司工作的人 | 属于与此项目关联的公司的用户可以查看请求并将其添加到此队列。 如果有一个公司与项目相关联，则该公司的名称将列在此设置后面的括号中。 |
     | 在这个项目组工作的人 | 属于与此项目关联的组的用户可以查看请求并将其添加到此队列。 如果存在与项目关联的组，则该组的名称将列在此设置后面的括号中。 |

     {style="table-layout:auto"}

   * **通过以下链接共享：** 通过以下选项，您可以向Workfront外部的用户或使用外部页面的Workfront用户提供对请求队列及其关联表单的直接访问。 有关在功能板中作为外部页面嵌入请求队列的信息，请参阅 [在功能板中嵌入请求队列](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     用户必须已拥有对请求队列的访问权限，才能获得直接访问权限。 使用此处描述的任一选项都不会自动授予用户访问权限。

     >[!TIP]
     >
     >用户从其他应用程序访问“请求队列”页面时，必须先登录到Workfront，然后才能获得对请求队列的访问权限。

      * **直接访问URL：** 当用户从浏览器访问此URL时，用户将直接转到请求区域的新请求部分，并且默认情况下会为他们选择此请求。

        ![](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >您可以在功能板中将“请求队列”显示为外部页面。 在这种情况下，会预先选择请求队列，但您可以从请求类型字段中选择任何其他请求队列。 用户可以更改请求类型。 还会显示请求的导航组件。

      * **嵌入代码：** 使用此HTML代码，可以将请求队列表单作为iframe嵌入到任何HTML页面中。\
        如果用户查看嵌入了代码的页面时尚未通过Workfront身份验证，则会显示“Workfront登录”对话框。 用户登录后，将显示“请求队列”表单。

        >[!NOTE]
        >
        在iframe中显示请求队列时，仅显示请求表单，请求名称会预先选定并变暗。 用户无法更改请求类型。 请求区域的导航组件不显示。

        为了在使用此嵌入代码时显示请求队列表单，您必须在系统设置中启用“允许在iframe中嵌入Workfront”设置。 有关在iframe中启用Workfront嵌入的更多信息，请参阅 [配置系统安全首选项](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). 如果未启用此设置，则iframe将显示为空白。

        您可以调整嵌入表单的显示方式的各个方面，如下所示：

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>功能</strong> </p> </th> 
           <th> <p><strong>解决方案</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>调整框架的大小</p> </td> 
           <td> <p>修改“宽度”和“高度”属性。</p> <p>默认情况下，宽度为“500”，高度为“600”</p> </td> 
          </tr> 
          <tr> 
           <td> <p>将用户定向到特定的队列主题或主题组</p> </td> 
           <td> <p>将“path”参数添加到src URL。 您可以通过导航到非嵌入表单中所需的队列主题或主题组并检查URL来查找路径参数。</p> </td> 
          </tr> 
          <tr> 
           <td> <p>显示并允许用户更改预配置的主题组下拉列表</p> </td> 
           <td> <p>使用“path”参数，方法是添加 <code>showPreSelectedOptions=true</code> 参数到 <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>检测表单何时提交</p> </td> 
           <td> <p>将“message”事件侦听器添加到网页窗口，并检查是否 <code>event.data.type</code> 是 <code>requestSubmitted</code>. <code>event.data.newIssueID</code> 将设置为已创建问题的ID。</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **请求类型：** 从下面的默认选项中选择。

     Workfront管理员可以重命名默认的请求类型。 有关重命名请求类型的更多信息，请参阅 [自定义默认问题类型](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * 错误报告
      * 更改顺序
      * 问题
      * 请求

        这是必填字段，您必须至少选择一个选项。

     >[!NOTE]
     >
     仅当在“队列详细信息”和“队列主题”页面中都选择了“请求类型”时，“请求类型”才会在“请求”区域显示为选项。 有关设置项目的队列详细信息区域的信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     此处选择的每个类型都将显示在表单上（您可以选择多个类型）。 选择多种类型可帮助组织传入的多个请求。\
     例如，如果您在IT项目的请求队列中使用表单，则队列中可能会包含以下请求类型：硬件、软件、错误修复和问题。

   * **默认持续时间：** 默认持续时间是完成问题通常需要的时间。 这会成为所有传入问题的默认值，可以手动修改。 持续时间通常以小时、天或周为单位设置。 问题的默认持续时间与问题的已计划小时数相同。 问题的计划完成日期根据此字段计算。\
     问题“持续时间”的默认值为1天或8小时。 如果您的Workfront管理员将每个工作日的典型小时数设置为小于8小时，则问题的默认持续时间仍为8小时。 例如，如果“每个工作日的典型小时数”设置为7小时，则问题的默认持续时间为1.14天或8小时。 有关如何设置系统“每个工作日的典型小时数”的更多信息，请参阅文章中的“时间线计算”部分 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **同一公司的人将为所有请求继承相同的访问权限。：** 选中后，提交到队列的所有请求对同一公司的用户可见。 用户可以在位于请求区域的所有请求部分中查看这些请求。 启用或禁用此设置时，它会影响所有未来的请求；而不会对信息产生追溯性影响。
   * **当有人提出请求时，自动授予：** 当用户向请求队列发出请求时，将自动授予用户您选择用于该请求的权限级别。 从以下权限级别中选择：

      * **查看**
      * **参与**. 这是默认选项。
      * **管理**

     有关Workfront权限模型的信息，请参阅 [对象权限共享概述](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     在此处设置权限可节省时间，而不必为每个传入请求授予权限。 选择此选项将影响所有未来的请求，但不会追溯影响现有请求。

   * **默认审批**：将审批流程与此请求队列关联。 此下拉菜单中仅显示“问题批准流程”。 提交到此队列的所有问题都将与此审批流程关联。 在将Workfront管理员与请求队列关联之前，您必须定义系统级别的批准流程。 对批准流程具有管理权限的用户还可以创建特定于组的批准流程。

     >[!IMPORTANT]
     >
     如果项目组发生更改，则附加到现有问题的组特定审批流程将变成一次性审批流程。 有关对项目组的更改或审批流程中的更改如何影响审批设置的更多信息，请参阅 [组和审批流程更改如何影响分配的审批流程](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     如果您有多个与请求队列相关的队列主题，我们建议您改为将审批流程与队列主题相关联。 有关创建队列主题的详细信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     将审批流程添加到请求队列时，请考虑以下事项：

      * 列表中仅显示有效的审批流程。
      * 列表中将显示系统范围和组特定的批准流程。 与项目组以外的组关联的审批流程不会显示在列表中。

   * **默认路由**：将路由规则与此请求队列关联。 使用传送规则，可以将提交至请求队列的新问题自动分配给正确的资源（用户、工作角色或团队），并分配给正确的项目。 提交到此队列的所有问题都将与此路由规则关联。 必须先配置路由规则，然后才能将其与请求队列关联。\
     如果有一个请求队列与多个队列主题相关联，我们建议您改为将路由选择规则与队列主题相关联。 有关创建路由规则的详细信息，请参阅 [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **新问题字段：** 在向所有用户显示以下所选字段部分中，选择您希望对提交请求到项目或向项目或任务添加问题的所有用户可见的任何字段。

     >[!TIP]
     >
     在队列详细信息部分中选择的新问题字段还与添加到项目或“问题”部分中的任务的任何新问题相关联。

     当您启用任何“分配至”、“工作角色”或“团队”字段时，它们始终会在请求表单中重命名为“分配”，但您只能在此处指定选定的分配类型。

     >[!NOTE]
     >
     如果您在“队列详细信息”区域中选择了“任务负责人”，则只能在“请求”表单的“任务”字段中输入用户。 在这种情况下，您无法输入工作角色或团队。


   * **文档**：如果选择在新请求表单中显示文档部分，请选择文档上传部分的放置位置。 从以下项中选择：

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">自定义表单后</td> 
        <td><span>文档部分显示在请求表单的底部。</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">自定义表单前</td> 
        <td> <p><span>文档部分显示在Workfront字段和请求表单的自定义字段之间。</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **将所有选定的和未选定的字段显示给：** 选择要查看表单上所有字段的用户。 以下选项控制对表单上字段的访问。

     | 哪些用户可以查看请求表单上的所有字段 | 描述 |
     |---|---| 
     | 所有用户（计划许可证） | 所有拥有计划许可证的用户都可以看到选定的和未选定的字段。 |
     | 拥有查看此项目权限的用户（计划许可） | 那些拥有计划许可证、也拥有此项目查看权限的用户可以查看选定和未选定的字段。 其他可以向此项目提交请求的用户只能看到选定的字段。 |
     | 无用户 | 没有用户可以看到未选择的字段。 所有能够向此项目提交请求的用户只能看到所选的字段。 |

   * **自定义Forms**：选择要与请求队列关联的自定义表单。 只有问题自定义Forms可供从该下拉菜单中选择。 提交到“请求队列”的所有问题都将具有与其关联的选定表单。\
     如果您有多个与请求队列关联的队列主题，我们建议您将自定义表单与队列主题关联。 有关为“请求队列”创建子部分的更多信息，请参阅 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![](assets/custom-forms-on-queue-details.png)

     如果您有多个与请求队列关联的自定义表单，请拖放这些表单，以按所需的顺序对它们进行排序，顺序如下： **重新排序Forms** 部分。

     >[!TIP]
     >
     添加到“队列详细信息”部分的自定义表单还与添加到项目的任何新问题或“问题”部分中的任务相关联。

1. 继续选择 **电子邮件队列设置** 区域，允许用户通过电子邮件将请求发送到请求队列项目。

   有关更多信息，请参阅 [允许用户通过电子邮件将问题发送到请求队列项目](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. 单击&#x200B;**保存**。\
   您的项目现在已配置为请求队列，用户现在可以向其中添加请求。

1. （可选）要增强“请求队列”功能，请为您的队列构建其他子部分，以及用于将传入请求路由到正确团队、被分派人或项目的规则。

   * 有关为请求队列创建子部分的信息，请参阅相关文章 [创建队列主题](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) 和 [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).
   * 有关将请求路由到适当的被分配人、团队和适当项目的信息，请参阅 [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
