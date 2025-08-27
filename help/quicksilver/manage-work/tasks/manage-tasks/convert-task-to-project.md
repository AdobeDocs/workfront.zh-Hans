---
product-area: projects
navigation-topic: manage-tasks
title: 将任务转换为项目
description: 当项目中的任务需要比您最初计划更大的工作量完成时，您可以将其转换为项目。
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: 7288c6fb0f5d45758e0a82b8d1283e1f43ae94e6
workflow-type: tm+mt
source-wordcount: '1198'
ht-degree: 2%

---

# 将任务转换为项目

<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>-->

当项目中的任务需要比您最初计划更大的工作量完成时，您可以将其转换为项目。

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
   <td> <p>规划 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置*</td> 
   <td> <p>编辑对任务和项目的访问权限</p> <p>使用模板转化为项目时，具有对模板的查看或更高访问权限</p> <p>注意：如果您仍然没有访问权限，请咨询Workfront管理员是否对您的访问级别设置了其他限制。 有关Workfront管理员如何修改您的访问级别的信息，请参阅<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">对象权限</td> 
   <td> <p>管理任务的权限</p> <p>如果使用模板转换为项目，则查看模板权限</p> <p>创建项目后，您便拥有该项目的管理权限</p> <p>有关请求其他访问权限的信息，请参阅<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">请求访问对象</a>。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;要了解您拥有什么计划、许可证类型或访问权限，请与Workfront管理员联系。

## 将任务转化为项目的注意事项

* 您可以使用模板将任务转换为空白项目或项目。
* 已删除原始任务。
* 所有子任务、问题和注释将汇总到新项目中。
* 文档、文档版本和校样将移至新项目。
* 将任务转化为项目时存在5分钟的处理限制。 如果任务附加了大量文档且无法转换，您可能需要删除某些文档并重试。
* 所有子任务和问题的状态和完成百分比将保留。
* 任务被分派人和将任务转化为项目的用户成为项目中的共享用户。
* 项目开始日期设置为任务的开始日期。
* 下表列出了项目信息以及项目信息是从模板还是从任务转移：

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>描述</td> 
    <td> <p>转移到新项目的任务的描述。 </p> <p> 如果任务没有描述，则模板中的描述将转移到项目。 </p> <p>如果任务和模板的“描述”字段为空，则项目中的字段为空。 </p> </td> 
    </tr> 
    <tr> 
    <td>状态</td> 
    <td> 为模板上的组选择的默认状态。 如果模板未与组关联，则项目状态将设置为Workfront管理员在“设置”的“项目偏好设置”区域中设置的默认状态。 有关信息，请参阅<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">配置系统范围的项目首选项</a>

  存在以下用于更新项目状态的方案：
  <ul>
    <li> 如果任务状态为“新建”，则项目状态将设置为“计划”。</li>
    <li> 如果任务状态为“进行中”，则项目状态将设置为“当前”。</li>
    <li> 如果任务状态为“完成”，则项目状态将设置为“完成”。</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>优先级</td> 
    <td>从任务转移到项目，或者从模板转移（如果在转换中使用模板）。 </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>任务中的URL将传输到新项目。 </p> <p> 如果未在任务中指定URL，则模板中的URL将传输到项目。 </p> <p>如果问题和模板的URL字段为空，则项目中的字段为空。 </p> </td> 
    </tr> 
    <tr> 
    <td>项目完成情况类型</td> 
    <td>从模板进行传输。</td> 
    </tr> 
    <tr> 
    <td>项目完成情况</td> 
    <td>与Workfront管理员在设置区域中确定的系统级默认首选项匹配。 有关信息，请参阅<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">将自定义条件设置为项目的默认值</a>
    </td> 
    </tr> 
    <tr> 
    <td>时间表开始日期</td> 
    <td>从模板进行传输。</td> 
    </tr> 
    <tr> 
    <td>项目日期</td> 
    <td> 
      <ul> 
      <li> <p><b>计划开始日期</b>：应根据模板计划的时区，预先选择基于模板计划工作时间的最近工作时间。 如果“计划起始日期”字段设置为“完成日期”，则此字段将被禁用。 </p> </li> 
      <li> <p><b>计划完成日期</b>：应根据模板计划的时区，预先选择基于模板计划工作时间的最近工作时间。 如果“计划起始日期”字段设置为“起始日期”，则此字段将被禁用。 </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>组合</td> 
    <td>从模板进行传输。 否则，此字段为空。</td> 
    </tr> 
    <tr> 
    <td>项目群</td> 
    <td>从模板进行传输。 否则，此字段为空。</td> 
    </tr> 
    <tr> 
    <td>组</td> 
    <td><p> 存在以下情况：</p>
      <ul><li>如果在转换期间指定了组，则该组将成为项目的组</li>
      <li>如果您使用模板转换为项目，并且模板上有一个组，并且在转换过程中未指定组，则模板组将成为新项目的组</li>
      <li> 如果模板上无组，并且在转换过程中未指定组，则原始问题项目的组将变成新项目的组</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>公司</td>    
    <td>  从模板进行传输。 否则，此字段为空。</td>

  </tr> 
    <tr> 
    <td>项目所有者</td> 
    <td>从模板的“模板所有者”字段转移。 否则，它会设置为正在执行转换的登录用户。 </td> 
    </tr> 
    <tr> 
    <td>项目赞助者</td> 
    <td>从模板上的模板发起人字段传输。 否则，此字段为空。</td> 
    </tr> 
    <tr> 
    <td>资源管理器</td> 
    <td>从模板进行传输。 否则，此字段为空。</td> 
    </tr> 
    <tr> 
    <td>任务设置</td> 
    <td>从模板转移。</td> 
    </tr> 
    <tr> 
    <td>问题设置</td> 
    <td>从模板转移。 </td> 
    </tr> 
    <tr> 
    <td>访问</td> 
    <td> <p>从模板上的Access部分转移。 </p> </td> 
    </tr> 
    <tr> 
    <td>审批</td> 
    <td>从模板转移。 与任务关联的审批将在转换期间删除。 </td> 
    </tr> 
  </tbody> 
  </table>


## 将任务转换为项目

1. 转到要转换为项目的任务。
1. 单击&#x200B;**更多**&#x200B;图标![](assets/more-icon.png)，然后单击&#x200B;**转换为项目**。
1. 选择以下任一选项：

   * **新建项目**，在不使用模板的情况下创建项目
   * **从模板中选择**&#x200B;部分中的模板

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. 在出现的通知上单击&#x200B;**继续**。
1. 在&#x200B;**转换为项目**&#x200B;框中，指定以下内容：

   * **名称**：为您的项目命名。 默认名称是任务的名称。 这是必填字段。
   * **描述**：描述此项目的用途。
   * （视情况而定）如果已选择从模板创建项目，请更新&#x200B;**转化为项目**&#x200B;框中的可用字段。

     有关编辑项目字段的详细信息，请参阅[编辑项目](../../../manage-work/projects/manage-projects/edit-projects.md)。

     >[!TIP]
     >
     >要更新转换至项目框财务分区中的字段，您必须对您的访问级别的财务数据具有“编辑”权限。 如果您拥有访问级别的查看财务数据的权限，则模板中的所有财务信息都将传输到新项目，并且在转换问题时无法编辑它。 有关信息，请参阅[授予对财务数据的访问权限](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)和[共享模板](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md)。

   * （可选）将&#x200B;**自定义Forms**&#x200B;添加到新项目中。

     >[!TIP]
     >
     >如果将附加到任务的多对象自定义表单配置为与任务和项目一起使用，则在进行转换时，将保留表单中保存的所有信息。
     >
     >
     >如果您将模板用于转化，并且附加到模板的自定义表单包含自定义字段（也可在附加到任务的自定义表单中找到），则任务的字段值将用于新项目。 但是，如果任务上的自定义字段为空，则使用来自模板的值。

1. 单击&#x200B;**保存更改** <!--<span class="preview">or **Convert to Project**</span>-->。
