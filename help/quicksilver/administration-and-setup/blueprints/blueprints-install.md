---
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: 安装Blueprint
description: 您可以在生产环境或沙箱环境中安装蓝图。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 546e19ab-dc50-4d23-b5f6-31bde1c82b6a
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 4%

---

# 安装蓝图

<!-- Audited: 5/2025 -->

您可以在生产环境或沙箱环境中安装蓝图。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td>“任一”</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td>
   <p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td>Workfront管理员</td> 
  </tr> 
 </tbody> 
</table>

有关此表中的信息的更多详细信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 应在何处安装蓝图？ {#where-should-i-install-a-blueprint}

您可以在以下任一环境中安装包：

<table style="table-layout:auto">
        <tr>
        <td><strong>生产</strong></td>
        <td>生产环境是您的实时环境。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 预览</strong></td>
        <td>沙盒预览是一个测试环境，用作实时环境的副本，每个周末由Adobe Workfront刷新。 所有支持包都可以访问“沙盒预览”。 有关详细信息，请参阅<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">预览Sandbox环境[!DNL Adobe Workfront]</a>。</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1和2</strong></td>
        <td>自定义刷新沙盒是一个单独的测试环境，由您手动刷新。 获取自定义刷新沙盒需要额外付费。 有关详细信息，请参阅<a href="../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md">自定义刷新沙箱环境[!DNL Adobe Workfront]。</a></td>
    </tr>
</table>

>[!TIP]
>
>我们建议首先在沙箱环境中安装蓝图。 这样，您就可以测试蓝图的内容，并确保它非常适合您的组织，而无需对实时数据进行更改。

>[!NOTE]
>
>某些蓝图只能安装在Preview环境中用于测试目的。 如果您在生产环境、沙箱1或沙箱2中访问仅预览内容，则“安装”按钮不活动，您可能会看到警告消息。\
>此外，在访问仅预览内容时，环境切换功能受到限制，即使您处于“预览”环境中也是如此。

## 安装Blueprint

{{step1-to-blueprints}}

1. 查找要安装的Blueprint。 您可以按用例、成熟度级别、安装状态和页面右侧的类型进行过滤。
1. （可选）单击&#x200B;**[!UICONTROL 详细信息]**&#x200B;以了解Blueprint的工作方式。
1. 单击&#x200B;**[!UICONTROL 安装]**。
1. 选择安装在生产环境或沙盒环境中。\
   有关详细信息，请参阅[我应该从何处安装Blueprint？本文中的](#where-should-i-install-a-blueprint)节。
1. 在&#x200B;**配置**&#x200B;页面上，您可以选择执行以下操作之一：

   * 按原样安装蓝图。 对于不需要任何配置的蓝图类型，这是唯一选项。 对于需要配置的Blueprint类型，可以选择立即安装Blueprint并在以后对其进行配置。 单击&#x200B;**[!UICONTROL 按原样安装]**。
   * 在安装之前配置Blueprint，适用于需要配置的Blueprint。 进行配置选择，然后单击&#x200B;**[!UICONTROL 安装Blueprint]**。

     有关详细信息，请参阅[配置Blueprint](../../administration-and-setup/blueprints/configure-template-package.md)。

   安装完成，并显示一条消息，其中列出了成功与Blueprint一起安装的特定对象（如角色、团队或组）以及任何无法安装的对象。

安装Blueprint后，可能需要执行一些其他操作才能完全部署它。 有关信息，请参阅安装Blueprint后要执行的[操作](../../administration-and-setup/blueprints/best-next-actions-after-install.md)。
