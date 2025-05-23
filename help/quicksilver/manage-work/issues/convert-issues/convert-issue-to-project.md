---
product-area: projects
navigation-topic: convert-issues
title: 在Adobe Workfront中将问题转化为项目
description: 在Adobe Workfront中将问题转化为项目
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1975'
ht-degree: 1%

---

# 在Adobe Workfront中将问题转化为项目

<!--Audited: 01/2024-->

如果在提交问题后需要完成更多工作，您可以将问题转化为项目。

您可以将问题转换为新项目，也可以使用模板将其转换为项目。 本文介绍了将问题转化为项目的两种方式。

>[!IMPORTANT]
>
>有关转化问题的一般信息，我们建议您同时阅读文章[在Adobe Workfront中转化问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

从问题创建项目时，项目上的某些字段会从其他对象填充。 有关详细信息，请参阅文章[创建项目](../../../manage-work/projects/create-projects/create-project.md)中的“新建项目默认设置”部分。

## 访问要求

+++ 展开以查看本文中各项功能的访问要求。

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>新增：标准 </p> 
    <p>当前：计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题、任务和项目的访问权限</p> <p>编辑对财务数据的访问权限以更新从问题转换而来的预计客户的财务信息</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看问题的权限</p> <p>在问题转化后，您可获得对项目的管理权限</p> </td> 
  </tr> 
 </tbody> 
</table>

有关此表中信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 将问题转化为项目

您可以将问题转换为空白项目。

1. 转到项目，然后单击左侧面板中的&#x200B;**[!UICONTROL 问题]**。
1. 在显示的问题列表中，执行以下操作之一：

   * 若要将问题转换为空白项目，请单击问题名称，单击问题名称右侧的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 转换为空白项目]**。


     或

     在问题列表中选择问题，单击列表顶部的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多](assets/more-icon.png)，然后单击&#x200B;**[!UICONTROL 转换为空白项目]**。

     >[!IMPORTANT]
     >
     >只有当您的系统或组管理员在[!UICONTROL 设置]区域中启用了[!UICONTROL 允许用户在不使用模板]首选项的情况下创建项目时，才会显示“转换为空白项目”选项。 有关详细信息，请参阅[配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)。


     在转换问题后，您必须手动将任务添加到项目，或向项目附加模板。

     >[!TIP]
     >   
     >* 如果问题是使用请求队列创建的，则新项目会继承请求队列的组。
     >* 如果问题是通过将其添加到项目的问题部分创建的，则新项目将继承问题项目的组。

     >[!TIP]
     >
     >如果问题与审批流程相关联或已经与解析对象关联，则Workfront会在转换为项目框的顶部显示警告，以通知您审批将被移除或者在转换期间解析对象将被覆盖。 有关详细信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

1. （可选且有条件）单击左侧面板中的&#x200B;[!UICONTROL **选项**]，然后从可用的选项中进行选择：

   * [!UICONTROL **保存原来的问题，并将其解决方案与项目绑定**]

     取消选择时，将删除原始问题。

     >[!NOTE]
     >
     >无权删除问题的用户将无法删除问题，因为他们正在转换问题，无论此设置的状态如何。 有关对问题的访问和权限的信息，请参阅：
     >
     >* [授予对问题的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **允许（用户名）访问此项目**]

     如果未选中，则问题的[!UICONTROL 主要联系人]无权访问新任务。

     >[!NOTE]
     >
     >此处提供的选项取决于Workfront管理员如何为系统中的每个人或您的组配置这些选项。 有关详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
     >
     >
     >或者，如果贵组织中的顶级组单独配置了它们，则此处的可用选项取决于您在步骤6为新项目选择的组。 有关详细信息，请参阅[为组配置任务和问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

1. 单击&#x200B;[!UICONTROL **自定义Forms**]&#x200B;并执行以下任一操作：

   * 查看附加到问题的自定义表单。 如果他们也是项目自定义表单，则将转移到新项目。
   * 添加更多自定义表单
   * 确保所有必填字段都包含有效信息。
   * 通过将自定义表单拖动到所需位置![拖动图标](assets/drag-object-icon.png)来重新排列它们。
   * 单击任何您不想转移到项目中的表单右侧的&#x200B;**x**&#x200B;图标。 这会从项目中删除表单。
   * 如有必要，请将自定义表单信息从问题传输到项目。

     >[!TIP]
     >
     >* 如果附加到问题的多对象自定义表单配置为同时用于问题和项目，那么当您进行转换时，如果问题中以及项目的自定义表单上存在字段，则该表单中保存的所有信息都会保留。
     >* 如果将具有计算字段的多对象自定义表单附加到问题以及项目，则问题和项目必须与表单的计算自定义字段中引用的所有字段兼容。 如果存在不兼容的情况，则会显示一条消息，提醒您进行调整。 有关详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)中的“多对象自定义表单中的计算自定义字段”部分。

1. 单击&#x200B;[!UICONTROL **转换为项目**]。

   >[!TIP]
   >
   >如果您决定删除原始问题，则问题现在为项目。
   >   
   >或
   >  
   >如果您决定保留原来的问题，则问题现在链接到新项目，并且将在项目完成时完成。
   >
   >如果您在转换过程中未更改某些问题字段中的信息，则这些信息会传输到项目。

1. （可选）根据需要设置任何其他项目详细信息&#x200B;（项目所有者、项目日期）和任务。
1. 单击&#x200B;[!UICONTROL **转换为项目**]。

   问题现已转化为项目。 此时将显示项目页面。

## 使用模板将问题转化为项目

您可以使用模板将问题转化为项目。

1. 转到项目，然后单击左侧面板中的&#x200B;**[!UICONTROL 问题]**。
1. 在显示的问题列表中，单击问题名称，单击问题名称右侧的&#x200B;**[!UICONTROL 更多]**&#x200B;菜单![更多菜单](assets/more-icon.png)，然后单击&#x200B;**从模板转换为项目**&#x200B;并开始在&#x200B;**搜索模板**&#x200B;框中键入模板名称，然后单击模板在列表中显示时的名称。 继续执行步骤3。

   >[!TIP]
   >
   >如果将模板添加到“收藏夹”列表，您可以将鼠标悬停在&#x200B;[!UICONTROL **收藏的模板**]&#x200B;菜单上，然后单击要使用的模板。

   此时将显示从模板新建项目框。

   ![从模板新建项目](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* 如果问题与审批流程相关联或已经与解析对象关联，则Workfront会在转换为项目框的顶部显示警告，以通知您审批将被移除或者在转换期间解析对象将被覆盖。 有关详细信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。
   >   
   >* 如果问题是使用请求队列创建的，则新项目会继承请求队列的组。
   >* 如果问题是通过将其添加到项目的问题部分创建的，则新项目将继承问题项目的组。

1. 查看右侧的模板详细信息。

   模板详细信息包括：

   * 模板持续时间
   * 模板所有者
   * 包括前三个任务的名称的顶级任务数
   * 模板中所有任务的数量
   * 模板自定义表单的名称

1. （可选）将鼠标悬停在模板名称上并单击&#x200B;**收藏夹**&#x200B;图标![收藏夹](assets/favorites-icon-small.png)以将其标记为收藏以供将来使用。

   >[!TIP]
   >
   >您最多可以将40个Workfront项目标记为收藏。 这包括模板和其他项目。

1. 单击&#x200B;[!UICONTROL **使用模板**]&#x200B;以选择模板。

   将打开[!UICONTROL 转换为项目]框。

   ![转换为项目](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. 如果模板中已填充某个字段，则该字段会在[!UICONTROL 转换为项目]框中预填充。 您可以编辑预填充的值以更好地匹配您的项目。 有关详细信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

   >[!TIP]
   >
   >* 您的系统或组管理员可以通过更新[!UICONTROL 布局模板]中的项目详细信息来添加或删除[!UICONTROL 转换为项目框]中的字段。
   >
   >* 要更新[!UICONTROL 转化为项目]框的[!UICONTROL 财务]分区中的字段，您必须对您的访问级别中的[!UICONTROL 财务数据]具有[!UICONTROL 编辑]访问权限。 如果您对访问级别为[!UICONTROL 财务数据]具有[!UICONTROL 查看]的访问权限，则模板中的所有财务信息都会传输到新项目，并且在您转换问题时无法对其进行编辑。 有关信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)和[共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

1. （可选且有条件）单击左侧面板中的&#x200B;[!UICONTROL **选项**]，然后从可用的选项中进行选择：

   * [!UICONTROL **保存原来的问题，并将其解决方案与项目绑定**]

     取消选择时，将删除原始问题。

     >[!NOTE]
     >
     >无权删除问题的用户将无法删除问题，因为他们正在转换问题，无论此设置的状态如何。 有关对问题的访问和权限的信息，请参阅：
     >
     >* [授予对问题的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [共享问题](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **允许（用户名）访问此项目**]

     如果未选中，则问题的[!UICONTROL 主要联系人]无权访问新任务。

     >[!NOTE]
     >
     >此处提供的选项取决于Workfront管理员如何为系统中的每个人或您的组配置这些选项。 有关详细信息，请参阅[配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)。
     >
     >
     >或者，如果贵组织中的顶级组单独配置了它们，则此处的可用选项取决于您在步骤6为新项目选择的组。 有关详细信息，请参阅[为组配置任务和问题偏好设置](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)。

   1. 单击&#x200B;[!UICONTROL **自定义Forms**]&#x200B;并执行以下任一操作：

      * 查看附加到模板的自定义表单。 他们将转移到新项目。
      * 查看附加到问题的自定义表单。 如果他们也是项目表单，则将转移到项目。
      * 确保所有必填字段都包含有效信息。
      * 通过将自定义表单拖动到所需位置![拖动图标](assets/drag-object-icon.png)来重新排列它们。
      * 单击任何您不想转移到项目中的表单右侧的&#x200B;**x**&#x200B;图标。
      * 如有必要，请将自定义表单信息从问题传输到项目。

        >[!TIP]
        >
        >* 如果附加到问题的多对象自定义表单配置为同时用于问题和项目，那么当您进行转换时，如果问题中以及项目的自定义表单上存在字段，则该表单中保存的所有信息都会保留。
        >* 如果将具有计算字段的多对象自定义表单附加到问题以及项目，则问题和项目必须与表单的计算自定义字段中引用的所有字段兼容。 如果存在不兼容的情况，则会显示一条消息，提醒您进行调整。 有关详细信息，请参阅[将计算字段添加到表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)。
        >* 如果附加到模板的自定义表单中包含的自定义字段也在附加到问题的自定义表单中找到，则问题中的字段值将用于新项目。 但是，如果问题的自定义字段为空，则使用模板中的值。

1. （可选）根据需要设置任何其他项目详细信息&#x200B;（项目所有者、项目日期）和任务。

   1. 单击&#x200B;[!UICONTROL **转换为项目**]。

      >[!TIP]
      >
      >如果您决定删除原始问题，则问题现在为项目。
      >   
      >或
      >  
      >如果您决定保留原来的问题，则问题现在链接到新项目，并且将在项目完成时完成。
      >
      >有些问题字段已转移到项目。 如果在先前的步骤中未更改模板中定义的大多数字段，则会自动转移到新创建的项目。 有关信息，请参阅[在Adobe Workfront中转换问题的概述](../../../manage-work/issues/convert-issues/convert-issues.md)。

   问题现已转化为项目。 此时将显示项目页面。
