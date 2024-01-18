---
product-area: projects
navigation-topic: convert-issues
title: 在Adobe Workfront中将问题转化为项目
description: 在Adobe Workfront中将问题转化为项目
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 1%

---

# 在Adobe Workfront中将问题转化为项目

如果在提交问题后需要完成更多工作，您可以将问题转化为项目。

您可以将问题转换为新项目，也可以使用模板将其转换为项目。 本文介绍了将问题转化为项目的两种方式。

>[!IMPORTANT]
>
>有关转化问题的一般信息，我们建议您同时阅读本文 [在Adobe Workfront中转化问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

从问题创建项目时，项目上的某些字段会从其他对象填充。 有关更多信息，请参阅文章中的“新项目默认设置”部分 [创建项目](../../../manage-work/projects/create-projects/create-project.md).

## 访问要求

您必须具有以下权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront计划*</td> 
   <td> <p>任何</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证*</td> 
   <td> <p>计划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对问题、任务和项目的访问权限</p> <p>编辑对财务数据的访问权限以更新从问题转换而来的预计客户的财务信息</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何更改您的访问级别的信息，请参阅 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>查看问题的权限</p> <p>在问题转化后，您可获得对项目的管理权限</p> <p>有关请求其他访问权限的信息，请参阅 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*要了解您拥有的计划、许可证类型或访问权限，请联系您的Workfront管理员。

## 将问题转化为项目

您可以将问题转化为空白项目或使用模板将问题转化为项目。

1. 转到项目并单击 **[!UICONTROL 问题]** 在左侧面板中。
1. 在显示的问题列表中，执行以下操作之一：

   * 要将问题转换为空白项目，请单击问题名称，然后单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-icon.png) 问题名称的右侧，然后单击 **[!UICONTROL 转换为空白项目]**.


     或

     选择问题列表中的问题，单击 **[!UICONTROL 更多]** 菜单 ![](assets/more-icon.png) ，然后单击 **[!UICONTROL 转换为空白项目]**.

     >[!IMPORTANT]
     >
     >“转换为空白项目”选项仅在系统或组管理员启用 [!UICONTROL 允许用户在不使用模板的情况下创建项目] 中的首选项 [!UICONTROL 设置] 区域。 有关更多信息，请参阅 [配置系统范围的项目首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     在转换问题后，您必须手动将任务添加到项目，或向项目附加模板。

     继续执行下面的步骤3e。

     <!--
     Is this accurate?
     -->

     >[!TIP]
     >   
     >* 如果问题是使用请求队列创建的，则新项目会继承请求队列的组。
     >* 如果问题是通过将其添加到项目的问题部分创建的，则新项目将继承问题项目的组。

   * 要使用模板将问题转化为项目，请执行以下操作之一：

      * 单击问题的名称，然后单击 [!UICONTROL **更多**] 菜单 ![](assets/more-icon.png) 问题名称的右侧

        或

      * 在问题列表、报表或功能板中选择问题，单击 **更多** 菜单 ![](assets/more-icon.png) ，然后单击 **从模板转换为项目** 并开始在 **搜索模板** 框，然后在模板显示在列表中时单击模板的名称。 继续执行步骤3。

        <!--      
        (is this accurate?)      
        -->

     >[!TIP]
     >
     >如果将模板添加到“收藏夹”列表，您可以将鼠标悬停在 [!UICONTROL **收藏模板**] 菜单，然后单击要使用的模板。

     此时将显示从模板新建项目框。

     ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

     >[!TIP]
     >
     >如果问题与审批流程相关联或已经与解析对象关联，则Workfront会在转换为项目框的顶部显示警告，以通知您审批将被移除或者在转换期间解析对象将被覆盖。 有关更多信息，请参阅 [在Adobe Workfront中转化问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

1. （视情况而定）如果您选择使用模板将问题转化为项目，请继续执行以下步骤：

   1. 查看右侧的模板详细信息。

      模板详细信息包括：

      * 模板持续时间
      * 模板所有者
      * 包括前三个任务的名称的顶级任务数
      * 模板中所有任务的数量
      * 模板自定义表单的名称

   1. （可选）将鼠标悬停在模板名称上并单击“收藏夹”图标 ![](assets/favorites-icon-small.png) 将其标记为将来最常使用。

      >[!TIP]
      >
      >您最多可以将40个Workfront项目标记为收藏。 这包括模板和其他项目。

   1. 单击 [!UICONTROL **使用模板**] 以选择模板。

      此 [!UICONTROL 转换为项目] 框打开。

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. 如果某个字段已填充到模板中，则该字段会预填充到 [!UICONTROL 转换为项目] 盒子。 您可以编辑预填充的值以更好地匹配您的项目。 有关更多信息，请参阅 [编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* 您的系统或组管理员可以在 [!UICONTROL “转换为项目”框] 方式是更新您网站上的 [!UICONTROL 布局模板].
      >
      >* 要更新 [!UICONTROL 财务] 中的部分 [!UICONTROL 转换为项目] 框您必须拥有 [!UICONTROL 编辑] 访问 [!UICONTROL 财务数据] 在访问级别中。 如果您拥有 [!UICONTROL 视图] 访问 [!UICONTROL 财务数据] 在访问级别中，模板中的所有财务信息将传递到新项目，并且在转换问题时无法编辑这些信息。 有关信息，请参阅 [授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) 和 [共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   1. （可选且视情况而定）单击 [!UICONTROL **选项**] 在左侧面板中，然后从可用的选项中进行选择：

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

        如果未选中，则问题属于 [!UICONTROL 主要联系人] 无权访问新任务。

        >[!NOTE]
        >
        >此处提供的选项取决于Workfront管理员如何为系统中的每个人或您的组配置这些选项。 有关更多信息，请参阅 [配置系统范围的任务和问题首选项](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
        >
        >
        >或者，如果贵组织中的顶级组单独配置了它们，则此处的可用选项取决于您在步骤6为新项目选择的组。 有关更多信息，请参阅 [配置组的任务和问题首选项](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. 单击 [!UICONTROL **自定义Forms**] 并执行以下任一操作：

      * 查看附加到模板的自定义表单。 他们将转移到新项目。
      * 确保所有必填字段都包含有效信息。
      * 通过拖动自定义表单来重新排列它们 ![](assets/drag-object-icon.png) 你希望他们去哪里。
      * 单击 **x** 图标来显示您不希望转移到项目中的任何表单。
      * 如有必要，请将自定义表单信息从问题传输到项目。

        >[!TIP]
        >
        >* 如果附加到问题的多对象自定义表单配置为同时用于问题和项目，那么当您进行转换时，如果问题中以及项目的自定义表单上存在字段，则该表单中保存的所有信息都会保留。
        >* 如果将具有计算字段的多对象自定义表单附加到问题以及项目，则问题和项目必须与表单的计算自定义字段中引用的所有字段兼容。 如果存在不兼容的情况，则会显示一条消息，提醒您进行调整。 有关更多信息，请参阅 [使用旧版表单生成器将计算的数据添加到自定义表单](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* 如果您使用模板进行转化，并且附加到模板的自定义表单包含自定义字段（也可在附加到问题的自定义表单中找到），则问题中的字段值将用于新项目。 但是，如果问题的自定义字段为空，则使用模板中的值。

   1. 单击 [!UICONTROL **转换为项目**].

      >[!TIP]
      >
      >如果您决定删除原始问题，则问题现在为项目。
      >   
      >或
      >  
      >如果您决定保留原来的问题，则问题现在链接到新项目，并且将在项目完成时完成。
      >
      >有些问题字段已转移到项目。 如果在先前的步骤中未更改模板中定义的大多数字段，则会自动转移到新创建的项目。 有关信息，请参阅 [在Adobe Workfront中转化问题概述](../../../manage-work/issues/convert-issues/convert-issues.md).

1. （可选）根据需要设置任何其他项目详细信息&#x200B;（项目所有者、项目日期）和任务。
1. 单击 [!UICONTROL **转换为项目**].

   问题现已转化为项目。

1. 单击 [!UICONTROL **转到项目**] 内部 [!UICONTROL 成功] 通知的页面。 这将打开项目页面。
