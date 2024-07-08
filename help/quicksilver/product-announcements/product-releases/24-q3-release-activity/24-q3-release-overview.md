---
title: 2024年第三季度版本概述
description: 此页面提供了有关2024年第三季度版本中所包含功能的信息。 计划在整个季度内在生产环境中提供这些增强功能。
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 372aa2c2-5deb-49da-aadc-6e870bbd083a
source-git-commit: 0965c9a02496127bbf9b562784ff06c295dc0cf1
workflow-type: tm+mt
source-wordcount: '1740'
ht-degree: 0%

---

# 2024年第三季度发行版概述

本页介绍了2024年第三季度版本中包含的功能信息。 这些增强功能计划本季度在“生产”环境中提供。

24.7版本的实时网络研讨会已取消，但您仍可以 [在此处观看24.7功能的视频演示](https://video.tv.adobe.com/v/3430532/%20).

<span class="preview">周期外功能（在2024年第三季度发布日期之前发布到生产环境的功能）以黄色突出显示。</span>

>[!IMPORTANT]
>
>23.3版本包括将您的组织移至每月版本的选项。 因此，Workfront更改了版本的编号方案，以说明每月和每季度的版本跟踪。 第一个数字表示年份，第二个数字表示发行的月份。 示例：2024年4月的版本为24.4。
>
>除非另有说明，否则每月和每季的发布计划在该月第二整周的星期四提供。
>
>| 每月版本 | 季度版本 |
>|----|----|
>| <ul><li>24.5（2024年5月16日）</li><li>24.6（2024年6月13日）</li><li>24.7（2024年7月18日）</li></ul> | <ul><li>24.7（2024年7月18日）</li></ul> |
>
>欲知快速发布流程的更多信息，请参阅 [启用或禁用快速发布流程](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [财务管理增强功能](#financial-management-enhancements)
* [集成增强功能](#integration-enhancements)
* [项目增强功能](#project-enhancements)
* [校对增强功能](#proofing-enhancements)
* [资源管理增强功能](#resource-management-enhancements)
* [其他增强功能](#other-enhancements)

### 管理员增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">业务规则现已可用</a></p>
                        <p>管理员现在可以在Workfront的“设置”区域中添加业务规则。</p>
                        <p>业务规则允许您对Workfront对象应用验证，并防止用户在满足某些条件时创建、编辑或删除对象。 使用与自定义表单中的计算字段类似的公式来构建规则。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年7月4日</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：使用24.7版本（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">Adobe Workfront中通常提供自定义表单设计器</a></p>
                        <p>在24.7版中，表单设计器将普遍可用，并将成为在Adobe Workfront中创建和编辑自定义表单的默认体验。 在创建新的自定义表单或打开现有表单时，您将看到表单设计器的“画布样式”工作区。</p>
                        <p>此版本发布后，您将无法再选择恢复到旧版表单生成器。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年6月19日</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：随24.7版本一起发布（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">通过环境升级在Workfront环境之间移动对象</a></p>
                        [！BADGE In production ]{type=Informative}
                        <p>利用环境升级，您可以将对象从一个Workfront环境移动到另一个环境，例如从沙箱环境移动到生产环境。 您可以配置和测试对象，而不会对您组织的数据和记录造成任何风险。 然后，您可以将这些对象移至生产环境，而无需重新配置它们，从而节省时间和精力。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>适用于所有客户的生产版本：使用24.6版本（2024年6月13日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">在自定义表单设计器中共享自定义表单和自定义字段</a></p>
                        [！BADGE In production ]{type=Informative}
                        <p>现在，您可以在新的表单设计器中共享自定义表单和自定义字段。 这允许用户在自定义表单上更好地协作。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年6月6日</p>
                            </li>
                            <li>
                                <p><span class="preview">所有客户的生产版本：6月13日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">从“字段”区域添加新的自定义字段</a></p>
                        <p>现在，您可以直接从Workfront中的字段区域添加新的自定义字段或构件，而无需打开自定义表单来创建字段。 这使您可以快速创建可重复使用的自定义字段。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年6月6日</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：随24.7版本一起发布（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-administrator-enhancements.md">表单设计器上提供的多选下拉字段类型</a></p>
                        [！BADGE In production ]{type=Informative}
                        <p>为了帮助您更轻松地定义下拉字段，我们已将多选下拉字段添加到自定义表单设计器。 此字段类型允许用户从下拉列表中选择多个选项。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本： 2024年6月4日</p>
                            </li>
                            <li>
                                <p><span class="preview">适用于所有客户的生产： 2024年6月4日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 财务管理增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-financial-mgmt-enhancements.md" class="MCXref xref" xrefformat="{para}">项目与任务可用的可开单和不可开单费用字段</a></p>
                        [！BADGE In production ]{type=Informative}
                        <p>为了帮助您更轻松地查看支出类型，已将支出分为项目和任务上的可计费支出和不可计费支出。 以下字段可用于添加到视图和报表：</p>
                        <ul>
                            <li><p>规划可记帐费用成本</p></li>
                            <li><p>计划非计费支出成本</p></li>
                            <li><p>实际非计费支出成本</p></li>
                            <li><p>实际非计费支出成本</p></li>
                        </ul>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年5月10日</p>
                            </li>
                            <li>
                                <p><span class="preview">所有客户的生产时间：2024年5月10日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 集成增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">适用于Experience Manager Assets的Workfront和Assets Essentials改进</a></p>
                        [！BADGE New in Preview ]{type=Negative}
                        <p>我们对Workfront进行了以下改进，以便实现Experience Manager Assets和Assets Essentials集成：</p>
                        <ul>
                            <li><p>该集成现在支持GCP作为云服务提供商。 以前支持AWS和Azure。</p></li>
                            <li><p>通过集成发送到Experience Manager的文件的大小限制已增加到30 GB。 以前，限制为5 GB。</p></li>
                        </ul>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本： 2024年6月27日</p>
                            </li>
                            <li>
                                <p>所有客户的生产：使用24.7版（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 项目增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">在标题或详细信息部分中编辑任务和问题提交日期和条件</a></p>
                        [！BADGE In Production for Fast Release ]{type=Positive}
                        <p>为了便于您更新任务和问题，我们现已添加“提交日期”和“条件”字段，作为选项，可添加到布局模板中的任务和问题标题及“详细信息”部分。 当这些字段被分配给修改后的布局模板时，用户现在可以从页面的标题或详细信息部分更新这些字段。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本： 2024年5月30日</p>
                            </li>
                            <li>
                                <p>快速发布生产：使用24.6版本（2024年6月13日）</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：使用24.7版本（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                   <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">已将更相关的分配添加到“新建任务”工作流</a></p>
                        <p>[！BADGE In Production for Fast Release ]{type=Positive}</p>
                        <p>在将任务添加到项目和项目任务列表时，我们已在“新建任务”框的“工作总揽”字段中添加了相同的功能，用于更相关的智能分配。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本： 2024年2月13日</p>
                            </li>
                            <li>
                                <p>针对快速版本的生产：24.5版（2024年5月16日）</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：随24.7版本一起发布（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">更相关的智能分配</a></p>
                        <p>[！BADGE for Fast Release ]{type=Positive}</p>
                        <p>我们更改了Workfront用于计算和建议智能任务分配的算法。 新算法适用于Workfront中分配任务的以下区域：任务列表、任务标题中的“工作总揽”区域、“主页”和“摘要”面板。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年12月21日</p>
                            </li>
                            <li>
                                <p>针对快速版本的生产：24.5版（2024年5月16日）</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：随24.7版本一起发布（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                 </tr>
           </tbody>
        </table>

### 校样增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-proofing-enhancements.md" class="MCXref xref" xrefformat="{para}">桌面校对查看器的安全更新</a></p>
                        <p>Workfront Proof Desktop Proofing Viewer 2.1.35安全更新为以前版本中发现的漏洞提供了安全错误修复。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年7月</p>
                            </li>
                            <li>
                                <p><span class="preview">适用于所有客户的生产： 2024年7月4日</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>             
           </tbody>
        </table>

### 资源管理增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-resource-mgmt-enhancements.md">空闲时间现在反映在工作负载均衡器中</a></p>
                        <p>为了在任务的主要被分配人已计划休息时间时无缝地调整工作，工作负载均衡器现在在重新计算项目时间表时重新分配小时数给主要用户和次要用户。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年6月6日</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：随24.7版本一起发布（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
           </tbody>
        </table>

### 其他增强功能

<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">功能</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">发行日期</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">更多Workfront组织现在可使用Adobe统一体验</a></p>
                        <p>为了让企业可以享用Adobe统一体验的好处，我们已经开始向现有Workfront客户提供。 </p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年6月20日</p>
                            </li>
                            <li>
                                <p>特定客户的生产：随24.7版（2024年7月18日）一起提供</p>
                            </li>
                         </ul>
                         <span style="color: #ff0000;">AdobeUnified Shell正在分阶段推出。 其他组织将登记到AdobeUnified Shell 24.10和25.1版本。 </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">帮助按钮已从主导航栏中移除</a></p>
                        <p>为了统一不在Unified Shell上的用户的体验，已删除主导航栏上的“帮助”按钮。 此按钮未向Unified Shell上的用户提供，已链接到Workfront文档，并且与主菜单中所有用户都可用的类似“帮助”按钮一起冗余。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本： 2024年6月6日</p>
                            </li>
                            <li>
                                <p>适用于所有客户的生产版本：使用24.7版本（2024年7月18日）</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">改进了具有有限对象访问权限的用户的UI体验</a></p>
                        [！BADGE for Fast Release ]{type=Positive}
                        <p>当用户无权访问某个对象时，该对象名称在Workfront中显示的任何位置都将显示“无访问权限”。 这种改进的体验也适用于Workfront API。</p>
                    </td>
                    <td><p><b>在以下日期提供：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2024年3月27日</p>
                            </li>
                            <li>
                                <p>针对快速版本的生产：24.5版（2024年5月16日）</p>
                            </li>
                            <li>
                                <p>季度版本生产：随24.7版（2024年7月18日）一起发布</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-look-and-feel-updates.md" class="MCXref xref" xrefformat="{para}">在2024年第三季度时间范围内的外观更新</a></p>
                        <p>在2024年第三季度内，将对Adobe Workfront应用程序各个方面的外观和感觉进行小幅更新。 查看特定发行日期的个人发行说明。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：整个2024年第三季度发布时间范围</p>
                            </li>
                            <li>
                                <p><span class="preview">生产版本：查看特定日期的发行说明</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>                
           </tbody>
        </table>

## 公告

### Workfront Fusion增强

Workfront Fusion中的新增功能在2024年第三季度发布计划之外的“生产”环境中以一定节奏提供。 有关最新功能的更多信息，请参阅 [Adobe Workfront Fusion发布活动](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Workfront Scenario Planner增强

此版本中目前没有Scenario Planner更新。 在有可用更新时，将更新此区域。

### Workfront Proof增强功能

此版本中此时没有Workfront Proof更新。 在有更新可用时，将更新此区域。

### Workfront Goals增强

此版本中目前没有Workfront Goals更新。 在有更新可用时，将更新此区域。

### API版本18

对于API版本18，我们修改了一些资源和端点。 某些更改支持新功能，而其他更改使您更容易使用通过API获得的信息。

有关新增功能和更新的信息，请参阅 [API版本18的新增功能](/help/quicksilver/wf-api/api/new-api-version-18.md).

有关API版本的信息，请参阅 [API版本控制和支持计划](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront 维护更新

有关2024年第三季度版本中所做维护更新的信息，请参阅 [Workfront维护更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

### 培训更新

探索每个Adobe Workfront产品版本对学习计划、学习路径、视频和指南的最新更新。 有关更多信息，请参阅 [“WorkfrontTutorials”页面](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html).
