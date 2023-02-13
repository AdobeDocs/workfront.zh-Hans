---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: 创建队列主题
description: 队列主题与路由规则结合使用，以自动将传入的工作分配给用户、作业角色、团队，或将其置于项目中。 队列主题定义要实施路由规则所需的条件。
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# 创建队列主题

队列主题与路由规则结合使用，以自动将传入的工作分配给用户、作业角色、团队，或将其置于项目中。 队列主题定义要实施路由规则所需的条件。

可以分配给主题组或项目的队列主题数量没有限制。 队列主题是可报告的对象类型。

## 访问要求

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

您必须具备以下条件：

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
   <td> <p>编辑对项目的访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员，他们是否在您的访问级别设置了其他限制。 有关Workfront管理员如何修改访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p> 管理项目的权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求对对象的访问 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员

## 创建队列主题

1. 创建路由规则、主题组和自定义表单（如果您计划将它们与队列主题关联）。\
   有关如何创建路由规则、主题组或自定义表单的详细信息，请参阅以下文章：

   * [创建路由规则](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [创建或编辑自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. 转到您选择启用作为帮助请求队列的项目，以及要在其中创建新队列主题。\
   有关如何将项目指定为帮助请求队列的详细信息，请参阅以下文章：\
   [创建请求队列](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   您可以在主题组下或直接在指定为帮助请求队列的项目下组织相关队列主题。 这将在请求者提出请求时提供一系列下拉菜单。\
   您可以将队列主题直接嵌套在指定为帮助请求队列的项目下，而无需主题组。

   有关创建主题组的信息，请参阅 [创建主题组](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. 单击 **队列主题** 中。 您可能需要单击 **显示更多**，则 **队列主题**.
1. 单击 **新建队列主题**.
1. 在 **新建队列主题** 表单中，指定以下内容：

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
      <td>描述请求队列。 当用户在提交新请求的过程中选择队列主题时，将显示描述。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>添加到主题组</strong> </td> 
      <td> 如果项目中没有主题组，则项目名称将默认为主题组。<br>如果要从此处创建其他主题组，请选择 <strong>新建主题组</strong> 下拉菜单中。<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic_png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>自定义表单</strong> </td> 
      <td>选择要与队列主题关联的任何自定义表单。 您必须先为问题创建自定义表单，然后才能将它们与队列主题关联。 有关创建自定义表单的信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">创建或编辑自定义表单</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">默认批准</td> 
      <td> <p>将批准流程与此队列主题关联。 此下拉菜单中仅显示“发行批准流程”。 提交到此队列的所有问题都将与此审批流程相关联。 您的Adobe Workfront管理员必须定义系统级别的审批流程，然后才能将它们与队列主题关联。 <span>对审批流程具有管理访问权限的用户也可以创建特定于组的审批流程。</span> 有关创建审批流程的更多信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">为工作项创建审批流程</a>.<br></p> 
       <div> 
        <p>重要信息：如果项目组发生更改，则附加到现有问题的特定于组的审批流程将变成一次性审批流程。 有关项目组更改或审批流程更改如何影响审批设置的详细信息，请参阅 <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">组和审批流程更改如何影响分配的审批流程</a>.</p> 
        <p>在向队列主题添加批准流程时，请考虑以下事项： </p> 
        <ul style="list-style-type: circle;"> 
         <li>列表中仅显示活动的批准流程。 </li> 
         <li> <p>系统范围和特定于组的审批流程将显示在列表中。 与项目组以外的组关联的批准流程不会显示在列表中。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认持续时间</strong> </td> 
      <td>这是请求的默认持续时间，并根据此值计算请求的计划完成日期。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>默认路线</strong> </td> 
      <td>指定要与队列主题关联的路由规则。 必须先创建路由规则，然后才能将其附加到队列主题。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>请求类型</strong> </td> 
      <td> <p>选择此队列主题存储的请求类型。 可见选项在 <strong>队列详细信息</strong> 选项卡。 这是必填字段。 </p> <p>注意：仅当在“队列详细信息”和“队列主题”页中都选择了“请求类型”时，“请求类型”才会在“请求”区域中显示为一个选项。 有关设置项目的“队列详细信息”区域的信息，请参阅 <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">创建请求队列</a>. </p> <p>从以下类型中进行选择：</p> 
       <ul> 
        <li>错误报告</li> 
        <li>更改顺序</li> 
        <li>问题</li> 
        <li>请求</li> 
       </ul> <p>您的Workfront管理员可能已重命名其中一些选项。 </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. 单击&#x200B;**保存**。\
   队列主题现在可供使用，并在选择请求队列和主题组后显示在Workfront的“请求”区域中。
