---
title: 启用或禁用AI助手
content-type: reference
description: 您可以控制组织中哪些访问级别有权访问AI助手。
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---

# 启用或禁用AI助手

作为Workfront管理员，您可以控制组织中哪些用户启用了AI助手。 这是通过访问级别管理的。

必须为组织启用AI助手，然后才能为访问级别启用。

## 访问权限要求

+++ 展开可查看本文所述功能的访问权限要求。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 包</td> 
   <td> <p>“任一” </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront许可证</td> 
   <td><p>标准</p>
   <p>规划</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>您必须是Workfront管理员</p> </td> 
  </tr> 
 </tbody> 
</table>

有关信息，请参阅Workfront文档中的[访问要求](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)。

+++

## 为您的组织启用或禁用AI助手

要为您的组织启用AI助手，请执行以下操作：

{{step-1-to-setup}}

1. 在左侧导航中选择&#x200B;**系统**，然后选择&#x200B;**首选项**。
1. 向下滚动到&#x200B;**AI首选项**&#x200B;部分。
1. 打开&#x200B;**启用AI**&#x200B;切换开关。

>[!IMPORTANT]
>
>在使用AI Assistant之前，您必须与Adobe签订文件上的Gen AI协议。
>有关Gen AI协议的更多信息，请参阅Workfront中的AI助手一文中的[签署Adobe Gen AI协议](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)。

## 启用或禁用访问级别的AI助手

要为给定的访问级别启用AI助手：

{{step-1-to-setup}}

1. 在左侧导航中选择&#x200B;**访问级别**。
1. 选择所需的访问级别，然后单击列表上方的&#x200B;**编辑** ![编辑图标](assets/edit-icon.png)图标。
1. 在&#x200B;**编辑访问级别**&#x200B;框的&#x200B;**设置其他限制……**&#x200B;区域中，取消选中&#x200B;**禁用Workfront AI助手**&#x200B;复选框。
1. 单击&#x200B;**保存**。
1. 对要为其启用AI助手的每个访问级别重复步骤3-5。



>[!NOTE]
>
>* 默认情况下，非管理员的用户会禁用AI助手。
>* 如果非管理员与Workfront中的AI助手图标交互，则显示AI助手协议，请求非管理员接受条款和条件。 如果接受协议，则即使布局模板中禁用了AI助手，他们也可以使用AI助手。

