---
title: 20.4项目管理方面的改进
description: 20.4项目管理方面的改进
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 12bab42ab13935fa284aa334120afcfb602bf412
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# 20.4项目管理方面的改进

本页介绍了20.4版本对“预览”环境所做的所有项目管理增强。 这些增强功能将在2020年11月9日这一周的“生产”环境中提供。

有关20.4版本的所有可用更改列表，请参阅[20.4版本概述](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md)。

## 管理员的新增功能：控制自定义字段的共享方式

为了让您更好地控制谁可以编辑、删除和使用您创建的自定义字段，我们添加了准确配置您希望如何共享这些字段的功能。

此前，当您创建自定义字段时，系统中的每个人都可以编辑它。 这仍然是自定义字段的默认状态，但现在您可以将自定义字段共享限制为仅共享某些用户、角色、团队、组和公司。 并且您可以确定收件人是否可以管理或仅查看自定义字段。

此外，为了让您熟悉这种体验，我们设计了用户界面，以便该功能与在Workfront中共享的其他对象区域类似。

## 管理员的新增功能：标准化的自定义表单共享

我们为自定义Forms实现了标准化共享，以便您可以使用已知的Workfront对象共享流程。 新的共享体验使您能够更好地控制谁可以编辑、删除和使用您创建的自定义Forms。 您可以将自定义表单的共享限制为某些用户、角色、团队、组和公司。 您还可以确定这些收件人是否可以查看或管理自定义表单。

有关详细信息，请参阅[共享自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)。

## 从项目、任务或问题的详细信息部分中导出自定义表单和概述信息

您现在可以将自定义表单信息导出为.pdf文件。 在访问对象的“详细信息”部分中的表单时，可以从项目、任务或问题中导出自定义表单。

除了导出项目、任务和问题的自定义表单之外，您现在还可以将概述区域包含在导出的pdf中。

有关从对象导出自定义表单的信息，请参阅[导出自定义表单和对象详细信息](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md)。

## 快速添加迭代

>[!NOTE]
>
>此功能已从生产环境中暂时删除。 当该功能可用时，将更新此页面。

为了简化创建小版本的体验，我们添加了一个新按钮，允许您从“小版本”选项卡添加小版本。 在这里，您可以创建迭代，然后稍后添加任务和问题。

您仍然可以在积压工作标记上创建迭代，就像之前一样。

有关详细信息，请参阅[创建迭代](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)。

## 项目中可用的新量度部分

为了节省时间并更好地了解项目的总体运行状况，项目中现在提供了“量度”部分，其中包含有关以下内容的信息：

* 完成、未完成、逾期和即将完成的工作
* 按状态或优先级分组的任务和问题金额
* 分配给每个用户的工作投入

您可以在图表上进行选择，以查看项目中任务和问题的不同方面，然后单击某些元素以显示任务信息。

<!--This feature is now included in the [Planner Fundamentals, Part 3 learning path](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) on Workfront One. -->

## 管理员的新增功能：将业务负责人分配给组

为了帮助您更好地组织和定义组，我们添加了将用户指定为组（或子组）的业务负责人的功能。 业务领导是为组制定业务决策的Workfront用户。

新的业务负责人字段可用于报告过滤器、视图和分组。 例如，您可以按特定的业务负责人进行筛选，以仅列出该人员在该角色中分配到的组。

有关详细信息，请参阅[业务负责人概述](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md)。

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## 管理员的新增功能：将项目组合、项目和公司与组关联

当Workfront管理员创建或编辑项目组合、项目或公司时，可以将其分配给组。 通过将组分配给这些对象，可以轻松确定您的组对这些对象的责任。

例如，您可以在报告中列出贵组织的所有项目组合，然后查看“组”列以查看您的组正在处理哪些项目组合。

有关详细信息，请参阅[组概述](../../../administration-and-setup/manage-groups/groups-overview/groups.md)一文中的“关于将组与对象关联”一节。

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## 管理员的新增功能：分配给公司的组的管理员可以管理公司

我们让组管理员可以轻松管理在Workfront中与其组关联的公司。 建立关联后，将自动提供管理公司的权限。 当组管理员对公司没有管理权限时，这一点尤其重要。

有关详细信息，请参阅[创建和编辑公司](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)。

有关对公司的管理访问权限的信息，请参阅[授予用户对特定区域的管理访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)。

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## 将“处理此项工作”按钮替换为“开始”按钮

为了帮助捕获工作项实际开始工作的日期和时间，用户可以将“处理工作”按钮替换为自动更新工作项状态和实际开始日期的“开始”按钮。

9月24日更新：在单击“开始任务”或“开始问题”后，您现在可以选择恢复您的选择，并通过单击“撤消”来指示您可能未准备好开始处理工作项目。 工作项将返回到“新建”状态，并且会删除“提交日期”和“实际开始日期”。 “撤消”选项显示的时间很短，在您离开页面或刷新页面后，该选项会被清除。

有关配置此选项的详细信息，请参阅[将处理它按钮替换为开始按钮](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)。

<!--This feature is now included in the [Worker Fundamentals learning path](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) and the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## 允许一个队列主题使用多个草稿

为了在处理请求时为您提供更大的自由度，您可以为一个队列主题保存多少草稿不再有任何限制。 创建新请求时，您可以从同一队列主题的草稿列表中选择现有草稿，覆盖它并将其作为新请求提交，也可以从头开始创建新请求。

在此增强功能之前，Workfront仅为请求队列中的每个队列主题保存一个草稿。

有关提交请求的信息，请参阅[创建并提交Workfront请求](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md)。

## 将组分配给团队

为了更便于管理和报告与组关联的团队，您现在可以将任何组分配给有权编辑的团队。

将团队分配给组时，其组管理员无需成为团队成员即可管理团队。 在“团队详细信息”页面上，他们可以看到分配给他们管理的组的团队。 他们还可以运行报告列出与特定组相关联的所有团队。

有关详细信息，请参阅[创建团队](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)。

<!--This feature is now included in the [Administrator Fundamentals, Part 1 learning path](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) on Workfront One. -->

## 通过新字段，可报告顶级组及其所有子组的数据

为了帮助您识别与顶级组及其子组关联的数据，我们添加了一个新的顶级父项ID字段，在创建有关组对象的报表时，您可以在筛选器、视图和组中使用该字段。

此字段应该对管理包含多个子组的组的组的组管理员特别有用。

例如，假设您管理一个名为营销的群组，该群组具有子群组字段营销和数字营销。 您可以通过创建具有以下筛选规则的“项目”区域筛选器，列出属于所有3个组的项目：
<pre>组：顶级父代名称&gt;等于&gt;营销</pre>我们还添加了一个新的“顶级父项名称”字段，可用于识别与视图中的顶级组（不在筛选器或分组中）关联的数据。

有关在列表和报告中使用字段的信息，请参阅[Adobe Workfront术语词汇表](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)。

## 放弃请求草稿时取消操作的新选项

放弃已保存的草稿时，您现在可以在通知您将删除草稿的确认消息上单击取消。 这样，您就不会丢失草稿，以防您改变放弃草稿的想法。

此功能仅在新的Workfront Experience中可用。 有关信息，请参阅[创建和提交Workfront请求](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html)。

