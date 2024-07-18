---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建队列主题
description: 队列主题与路由规则配合使用，可自动将传入工作分配给用户、工作角色、团队，或将其置于项目中。 队列主题定义实施路由规则所需的条件。
author: Alina
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# 创建队列主题

<!-- Audited: 12/2023 -->

队列主题与路由规则配合使用，可自动将传入工作分配给用户、工作角色、团队，或将其置于项目中。 队列主题定义实施路由规则所需的条件。

可以分配给主题组或项目的队列主题的数量没有限制。 队列主题是可报告的对象类型。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

<!--drafted - replace table with P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
    <p>新增：标准</p>
    <p>或</p>
    <p>当前：计划</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>编辑对项目的访问权限</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 创建队列主题

1. 创建路由规则、主题组和自定义表单（如果计划将它们与队列主题关联）。\
   有关如何创建路由规则、主题组或自定义表单的更多信息，请参阅以下文章：

   * [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. 转到您选择启用为帮助请求队列的项目以及要创建新队列主题的位置。\
   有关如何将项目指定为帮助请求队列的详细信息，请参阅[创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)。

   可以将相关的队列主题组织到主题组下。 这会在发出请求时为请求者提供一系列下拉菜单。

   或

   可以将队列主题直接嵌套在指定为帮助请求队列的项目下，而无需主题组。

   有关创建主题组的信息，请参阅[创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)。

1. 单击左侧面板中的&#x200B;**队列主题**。 您可能需要单击&#x200B;**显示更多**，然后单击&#x200B;**队列主题**。
1. 单击&#x200B;**新建队列主题**。
1. 在&#x200B;**新建队列主题**&#x200B;窗体中，输入以下内容：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>名称</strong> </td> 
      <td> 队列主题的名称。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>描述</strong> </td> 
      <td>描述请求队列。 在提交新请求的过程中，当用户选择队列主题时，将显示说明。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>添加到主题组</strong> </td> 
      <td> 如果项目中没有主题组，则项目的名称默认为主题组。<br>如果要在此处创建其他主题组，请从下拉菜单中选择<strong>新建主题组</strong>。<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自定义表单</strong> </td> 
      <td>选择要与队列主题关联的任何自定义表单。 必须先创建问题的自定义表单，然后才能将问题与队列主题关联。 有关创建自定义表单的信息，请参阅<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认批准</strong></td> 
      <td> <p>将审批流程与此队列主题关联。 仅问题批准流程在此下拉菜单中可见。 提交到此队列的所有问题都将与此审批流程相关联。 您的Adobe Workfront管理员必须定义系统级别的批准流程，然后才能将其与队列主题关联。 <span>对审批流程具有管理权限的用户也可以创建特定于组的审批流程。</span>有关创建审批流程的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建审批流程</a>。<br></p> 
       <div> 
        <p>重要信息：如果项目组发生更改，则附加到现有问题的组特定审批流程会成为一次性审批流程。 有关对项目组的更改或审批流程中的更改如何影响审批设置的详细信息，请参阅<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>。</p> 
        <p>将审批流程添加到队列主题时，请考虑以下事项： </p> 
        <ul style="list-style-type: circle;"> 
         <li>列表中仅显示有效的审批流程。 </li> 
         <li> <p>系统范围及组特定的批准流程会显示在列表中。 与项目组以外的组关联的审批流程不会显示在列表中。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认持续时间</strong> </td> 
      <td>这是请求的默认持续时间，并根据此值计算请求的规划完成日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认路由</strong> </td> 
      <td>指定要与队列主题关联的路由规则。 必须先创建路由规则，然后才能将其附加到队列主题。 有关信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">创建路由规则</a>。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>请求类型</strong> </td> 
      <td> <p>选择此队列主题存储的请求类型。 可见选项在项目的<strong>队列详细信息</strong>选项卡上设置。 这是必填字段。 </p>

   <p><b>注释</b>：

   仅当在“队列详细资料”页和“队列主题”页中都选择了“请求类型”时，“类型”才会在“请求”区域显示为选择。 有关设置项目的队列详细信息区域的信息，请参阅<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>。 </p> <p>从以下类型中选择：</p>
   <ul>
   <li>错误报告</li>
   <li>更改顺序</li>
   <li>问题</li>
   <li>请求</li>
   </ul> <p>您的Workfront管理员可能已重命名其中一些选项。 </p> </td>
   </tr> 
    </tbody> 
   </table>

   ![新队列主题框](assets/new-queue-topic-box.png)

1. 单击&#x200B;**保存**。\
   现在，队列主题可供使用，并且在选择请求队列和主题组后，该主题会显示在Workfront的请求区域中。
