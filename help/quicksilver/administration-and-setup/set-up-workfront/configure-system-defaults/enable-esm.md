---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 为您的组织启用Adobe云存储
description: 您可以为组织启用Adobe云存储，以便为所有Adobe产品使用统一存储解决方案。
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 3%

---
# 为您的组织启用Adobe云存储

Adobe云存储是一个统一的基于云的存储解决方案，它充当Adobe企业产品中资产的中央存储库。 本文介绍了如何启用Adobe云存储作为整个组织或特定组的默认存储选项。

这是单个打开新Experience的操作：启用后，新项目将使用Adobe云存储，包括Frame.io查看器和统一批准。 在选择启用Adobe云存储之前，不会发生任何更改。

由于您可以控制时间，因此可以在任何人使用它之前测试体验、更新Workfront Fusion场景并规划报表更改。 有关新增功能以及如何规划转出的更多信息，请参阅[在Adobe云存储上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

## 如何将审批与Adobe云存储结合使用

Adobe cloud storage可确定项目使用的审批服务。 迁移到支持Adobe云存储的Workfront版本不会自动将整个组织切换到统一批准。 相反，批准服务取决于每个项目的存储模型：

* **Adobe云存储项目**&#x200B;默认使用统一批准，在Frame.io查看器中审核和批准。
* **旧版Workfront存储项目**&#x200B;保留已使用的审批服务。 根据您的组织，这可以是统一审批或旧文档审批。

有关Adobe云存储审核和批准体验的更多信息，请参阅[在Adobe云存储上移至Workfront](/help/quicksilver/review-and-approve-work/workfront-storage.md)。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td><p>任何工作流包</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p> <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>您必须是Workfront管理员。 </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为您的组织启用Adobe云存储

要为贵组织启用Adobe云存储，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**首选项**。
1. 向下滚动到&#x200B;**存储首选项**&#x200B;部分。
1. 在默认下拉菜单中，选择&#x200B;**Adobe云存储**。
1. （可选）如果要使用Adobe Cloud Storage和旧版Workfront Storage的组合，请选中&#x200B;**允许用户选择存储提供程序**&#x200B;复选框。

   >[!NOTE]
   >
   >启用此选项允许用户在创建新项目时选择存储提供程序。 Adobe云存储被标记为“新项目”，因为它是默认的存储提供商。 旧版Workfront存储已标记为“旧版项目”。
   >
   >![新项目和旧项目选项](assets/new-esm-project.png)

1. 在“应用于”下拉菜单中，选择以下选项之一：

   * **整个组织**：此选项将默认存储提供程序应用于您的整个Workfront环境。 每当用户创建新项目时，都将使用默认存储提供程序。
   * **特定组**：此选项仅将默认存储提供程序应用于您组织内的特定组。 每当指定组中的用户创建新项目时，都将使用默认的存储提供程序。

     ![存储首选项组](assets/configure-storage-preference.png)

1. 单击&#x200B;**保存**。

   >[!NOTE]
   >
   >现有项目会保留创建它们的存储模型。 例如，在更改默认存储首选项后，使用Adobe云存储的项目将继续使用Adobe云存储。



## 沙盒环境中的Adobe云存储

Adobe云存储在[!DNL Workfront]沙盒环境中可用，允许您先测试本文中描述的功能，然后再在生产环境中推出。 但是，Frame.io查看器在沙盒中不可用，因此必须在生产环境中验证完整的统一审阅和批准体验。

如果您有自定义刷新沙盒，则在升级到支持Adobe云存储的Workfront版本后必须刷新它。 通过刷新，沙盒可以访问Adobe云存储功能，以便您可以开始对其进行测试。 有关详细信息，请参阅[自定义刷新沙盒环境 [!DNL Adobe Workfront] &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)。
