---
title: 2026年第二季度管理员增强功能
description: 2026年第二季度管理员增强功能
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ce152c48-ed72-47ed-b1c5-940c93b4a9ec
source-git-commit: d3a7c3c03b6be87f3adf2fd67b9136bc2be9c24b
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# 2026年第二季度管理员增强功能

本页介绍了在2026年第二季度版本中对“预览”环境所做的管理员增强。 如上所述，这些增强功能将在“生产”环境中提供。

有关2026年第二季度发布周期中此时可用的所有更改列表，请参阅[2026年第二季度发布概述](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md)。

## 现在，自定义季度在设置中作为单独页面提供

>[!NOTE]
>
>预览：2026年3月5日
>生产快速发布： 2026年4月15日
>适用于所有人的生产： 2026年4月16日

我们已从“项目首选项”部分移动了“自定义季度”区域。 它现在是“设置”中的独立部分。 
此更新包括以下内容：

* 自定义季度区域将从设置中的项目偏好设置部分中移除
* 自定义季度部分已添加到设置左侧面板。 功能保持不变。 
* “自定义季度”部分已从组的项目偏好设置部分中移除。 组管理员无法再查看自定义季度设置。 

有关信息，请参阅[启用自定义季度](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md)。

## 默认情况下折叠自定义表单部分

>[!NOTE]
>
>预览：2026年2月26日
>生产快速发布： 2026年3月12日
>适用于所有人的生产： 2026年4月16日

默认情况下，当窗体本身展开时，自定义窗体上的所有部分都会展开。 自定义表单设计器上的新选项允许您在用户打开表单时将节标记为默认折叠。 此选项在部分级别应用，而不是在字段应用。

有关详细信息，请参阅[组织和预览表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md)。

## 富文本字段类型现在可用于自定义表单

>[!NOTE]
>
>预览： 2026年1月29日
>生产快速发布： 2026年2月12日
>为所有人生产：待定
>
>此功能已于2026年2月13日从生产环境中暂时删除。

自定义表单中的新&#x200B;**富文本**&#x200B;字段类型是一个强大的文本编辑器，除了粗体、斜体、下划线、项目符号、编号、超链接和块引号等传统选项外，还具有格式选项，如上标和下标、标题和表格。 字符限制仍为15,000。

富文本字段类型正在将文本替换为格式字段类型。 您可以通过单击右侧字段选项中的按钮，快速将带格式字段的现有文本转换为富文本。 转换时，历史数据将保留在字段中，并在报表中以相同的方式使用。

有关详细信息，请参阅[创建自定义表单](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)。

## 用于Workfront电子邮件通知的新IP地址

我们正在更新用于从Workfront发送电子邮件通知的IP地址。 如果您的组织维护电子邮件或防火墙允许列表，则必须在下面添加新的IP地址，以确保继续发送Workfront通知。

这些更新适用于Workfront应用程序生成的所有出站电子邮件，包括批准、提醒、验证通知和其他系统消息。

美国：

* 206.55.149.212
* 206.55.149.214
* 206.55.149.215
* 206.55.149.213
* 206.55.149.211

欧盟：

* 24.110.76.224
* 24.110.76.223

有关详细信息，请参阅[配置防火墙的允许列表](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md)。
