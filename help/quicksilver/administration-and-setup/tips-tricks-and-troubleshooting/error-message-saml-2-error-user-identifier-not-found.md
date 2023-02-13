---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: “错误消息：SAML 2.0错误：未找到用户标识符'
description: 无法成功建立与ADFS的连接。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---

# 错误消息：SAML 2.0错误：未找到用户标识符

## 问题

无法成功建立与ADFS的连接。

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>如果您成功建立了测试连接，但仍然遇到问题，则可能存在不正确的属性映射或联合ID问题。 如有问题，请联系客户支持。

## 原因：

ADFS服务器上的声明不正确

## 访问要求

您必须具有以下访问权限才能执行本文中的步骤：

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 计划</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 许可证</td> 
   <td>计划</td> 
  </tr> 
  <tr> 
   <td role="rowheader">访问级别配置</td> 
   <td> <p>你必须是 [!DNL Workfront] 管理员。 有关更多信息，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">授予用户完全管理访问权限</a>.</p> <p><b>注意</b>:如果您仍无权访问，请咨询您的 [!DNL Workfront] 管理员。 有关如何 [!DNL Workfront] 管理员可以修改您的访问级别，请参阅 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">创建或修改自定义访问级别</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 解决方案

在ADFS服务器上，确保对名称ID有声明：

1. 在Windows中，单击 **[!UICONTROL 开始]** > **[!UICONTROL 管理]** > **[!UICONTROL ADFS 2.0管理]**.\
   将显示ADFS 2.0管理对话框。

1. 选择 **[!UICONTROL 信任关系]** > **[!UICONTROL 信赖方信托]** 在左窗格中。

1. 右键单击与Adobe Workfront相关的信赖方信任，然后选择 **[!UICONTROL 编辑声明规则]**.
1. 验证声明是否具有 **[!UICONTROL 传出声明类型]** of **[!UICONTROL 名称ID]**.

![1.png](assets/1-350x287.png)
