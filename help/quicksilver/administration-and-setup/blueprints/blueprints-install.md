---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安装Blueprint
description: 您可以在生产环境或沙盒环境中安装Blueprint。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# 安装Blueprint

您可以在生产环境或沙盒环境中安装Blueprint。

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 计划</strong></td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] 许可证</strong></td> 
   <td>[!UICONTROL计划]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>访问级别配置</strong></td> 
   <td> <p>[!UICONTROL系统管理员]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 我应该在何处安装Blueprint? {#where-should-i-install-a-blueprint}

您可以在以下任何环境中安装包：

<table style="table-layout:auto">
        <tr>
        <td><strong>生产</strong></td>
        <td>生产是您的实时环境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 预览</strong></td>
        <td>“沙盒预览”是一个测试环境，可用作实时环境的副本，并且每周末由Workfront刷新一次。 所有支持包都有权访问“沙盒预览”。 有关更多信息，请参阅 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">的 [!DNL Adobe Workfront] 预览沙盒环境</a>.</td>
    </tr>
    <tr>
        <td><strong>沙盒1和2</strong></td>
        <td>自定义刷新沙盒是一个单独的测试环境，由您手动刷新。 获取“自定义刷新”沙盒需要额外付费。 有关更多信息，请参阅 <a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">的 [!DNL Adobe Workfront] 自定义刷新沙盒环境</a>.</td>
    </tr>
</table>

>[!TIP]
>
>我们建议先在沙盒环境中安装Blueprint。 这样，您就可以测试Blueprint的内容，并确保它非常适合您的组织，而无需更改实时数据。

>[!NOTE]
>
>某些蓝图仅可用于在“预览”环境中安装以进行测试。 如果您在生产环境、沙盒1或沙盒2中访问仅预览内容，则安装按钮不活动，您可能会看到一条警告消息。\
>此外，在访问仅预览内容时，即使您处于预览环境中，环境切换功能也会受到限制。

## 安装Blueprint

1. 单击 **[!UICONTROL 主菜单]** 图标 ![](assets/main-menu-icon.png) 的右上角 [!DNL Adobe] Workfront，然后单击 **[!UICONTROL 蓝图]**.
1. 查找要安装的Blueprint。 您可以按用例、成熟度级别、安装状态进行筛选，并在右侧键入。
1. （可选）单击 **[!UICONTROL 详细信息]** 了解Blueprint的工作原理。
1. 单击 **[!UICONTROL 安装]**.
1. 选择在生产环境或沙盒环境上安装。\
   有关更多信息，请参阅 [我应该在何处安装Blueprint?](#where-should-i-install-a-blueprint) 章节。
1. 在 [!UICONTROL 配置] 页面时，您可以选择执行以下操作之一：

   * 按原样安装Blueprint。 对于不需要任何配置的Blueprint类型，这是唯一的选项。 对于需要配置的Blueprint类型，您可以选择立即安装Blueprint并稍后进行配置。 单击 **[!UICONTROL 按原样安装]**.
   * 在安装前配置Blueprint，以了解需要配置的Blueprint。 选择配置，然后单击 **[!UICONTROL 安装Blueprint]**.\

      有关更多信息，请参阅 [配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md).
安装完成后，将显示一条消息，其中列出了已成功与Blueprint一起安装的特定对象（如角色、团队或组）以及任何未能安装的对象。

安装Blueprint后，可能需要执行一些其他操作才能完全部署它。 有关信息，请参阅 [安装Blueprint后要执行的操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md).
