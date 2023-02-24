---
title: 23.2版本概述
description: 23.2版本概述
author: Courtney
draft: Probably
feature: Product Announcements
source-git-commit: 10c7e95f542cb3e05de62cff24f24439af140c0c
workflow-type: tm+mt
source-wordcount: '1454'
ht-degree: 0%

---


# 23.2版本概述

本页介绍了计划于2023年4月发布的23.2版中包含的功能信息。

在“预览”环境中，提供了此页面上的增强功能。 当23.2版本接近其计划的生产版本时，本页面将进行更新，并提供其他增强功能。

有关为即将发布的版本做准备的提示，请参阅 [为Adobe Workfront季度版本做准备](/help/quicksilver/product-announcements/product-releases/release-readiness.md).

<!-- The 23.2 release webinar will be held on ___. You can [register for the webinar here](link). -->

<span class="preview">非周期功能（在23.2发行日期之前发布到生产环境的功能）以黄色突出显示。</span>

## Adobe Workfront增强功能

* [管理员增强功能](#administrator-enhancements)
* [灵活的增强功能](#agile-enhancements)
* [项目管理增强功能](#project-management-enhancements)
* [资源管理增强](#resource-management-enhancements)
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-6.md" class="MCXref xref" xrefformat="{para}">重命名布局模板中的管脚</span></a>
                        </span></a><p>您现在可以重命名布局模板中的针脚，以便对用户更有意义，而不是使用固定页面的默认名称。 管理员创建的管脚将针对分配给布局模板的所有用户显示，用户无法重命名这些管脚。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月9日<br /></p>
                            </li>
                            <li>
                                 <p>生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### 灵活的增强功能

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-20.md" class="MCXref xref" xrefformat="{para}">在主板上的连接卡上记录小时</a><span style="color: #ff0000;"> 预览中的新增功能！</span></p>
                        <p>现在，您可以在连接的卡上登录数小时，这与在任务或问题上的登录方式相同。 您必须拥有正确的任务或问题权限才能记录时间。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月23日<br /></p>
                            </li>
                            <li>
                                 <p>提前选择加入的生产版本：2023年3月2日 <span style="color: #ff0000;"> 此功能仅在此日期通过为Workfront主板提前选择加入功能在生产环境中提供。</span></p>
                                <p>适用于所有客户的生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
              <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">自定义信息卡中字段的显示</a></p>
                        <p>现在，可进行自定义，以配置在信息卡上显示的字段（在信息卡打开时的完整视图中）和展示板上的压缩信息卡视图中。 禁用字段时，这两个视图中都不显示字段。 您还可以在完整视图中启用字段，并在压缩视图中隐藏该字段。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月16日<br /></p>
                            </li>
                            <li>
                                 <p>提前选择加入的生产版本：2023年2月23日 <span style="color: #ff0000;"> 此功能仅在此日期通过为Workfront主板提前选择加入功能在生产环境中提供。</span></p>
                                <p>适用于所有客户的生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">为移入展示板列的信息卡定义默认状态</a></p>
                        <p>您现在可以通过在列策略中选择自定义状态和系统状态，将默认状态设置为应用于移动到特定列中的卡。 将信息卡移入列时，Workfront会首先尝试应用自定义状态（例如，等待反馈）。 如果自定义状态不适用于该卡，则Workfront将应用系统状态（例如，暂挂）。 此外，如果连接任务或问题的状态更改为列策略中设置的自定义或系统状态，则卡会自动移至列。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月16日<br /></p>
                            </li>
                            <li>
                                 <p>提前选择加入的生产版本：2023年2月23日 <span style="color: #ff0000;"> 此功能仅在此日期通过为Workfront主板提前选择加入功能在生产环境中提供。</span></p>
                                <p>适用于所有客户的生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                 <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">收藏集现在在Adobe Workfront展示板中可用</a></p>
                        <p>您现在可以在展示板仪表板上创建收藏集。 收藏集是一组用于协作工作的委员会。 命名收藏集后，您可以使用一组提供预定义设置（如列名称）的模板将展示板添加到收藏集。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月16日<br /></p>
                            </li>
                            <li>
                                 <p>提前选择加入的生产版本：2023年2月23日 <span style="color: #ff0000;"> 此功能仅在此日期通过为Workfront主板提前选择加入功能在生产环境中提供。</span></p>
                                <p>适用于所有客户的生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-1-jan-23.md" class="MCXref xref" xrefformat="{para}">连接卡上的估计字段映射到Workfront对象上的“文章点”字段</a></p>
                        <p>Workfront展示板中连接的信息卡上的“估计”字段现在映射到关联的Workfront对象的“文章点”字段。 </p>
                        <p>新的“文章点”字段是一个可编辑的自由表单字段，您可以将该字段添加到列表或报表中的视图，以了解任务或问题。 它不与计划小时数或团队分配绑定。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年1月26日<br /></p>
                            </li>
                            <li>
                                 <p>提前选择加入的生产版本：这项功能推迟了，将于2月9日发布。 <span style="color: #ff0000;">此功能仅在此日期通过为Workfront主板提前选择加入功能在生产环境中提供。</span></p>
                                <p>适用于所有客户的生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-1-jan-23.md" class="MCXref xref" xrefformat="{para}">进气列中的预览卡</a></p>
                        <p>现在，您可以单击进入列中的连接卡，以查看其内容的仅查看版本。 在信息卡从进入列移出到展示板上的另一列之前，您无法编辑信息卡内容。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年1月26日<br /></p>
                            </li>
                            <li>
                                 <p>提前选择加入的生产版本：2023年2月2日 <span style="color: #ff0000;"> 此功能仅在此日期通过为Workfront主板提前选择加入功能在生产环境中提供。</span></p>
                                <p>适用于所有客户的生产版本：在23.2版本中</p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### 项目管理增强功能

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">复制项目时复制预算小时数</a>
                        <p>现在，您可以在复制项目时，选择复制在“业务案例”或“资源计划员”的“资源预算”区域中预算的小时数。 在此增强之前，项目预算的小时数未转移到复制的项目。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月16日<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">生产版本：2023年3月2日（非周期）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

### 资源管理增强

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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-13.md" class="MCXref xref" xrefformat="{para}">引入“工作时间”字段以准确计算用户容量</a>
                        <p>为了让资源经理能够准确计算其用户的可用性并考虑用户投入实际项目相关工作的时间，我们将工作时间概念引入Adobe Workfront。</p>
                        <p>在创建或编辑每个用户的配置文件时，您可以为其定义“工作时间”字段的值。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：2023年2月16日<br /></p>
                            </li>
                            <li>
                                 <p><span class="preview">生产版本：2023年3月2日（非周期）</span></p>
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
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-feb-6.md" class="MCXref xref" xrefformat="{para}">在Adobe Workfront for XD中将画板导出为单个PDF或多个PDF文件</span></a>
                        </span></a><p>在Adobe Workfront for XD插件中，您现在可以选择将画板导出为单个PDF文件或多个PDF文件。</p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：不适用<br /></p>
                            </li>
                            <li>
                                 <p>生产版本：2023年2月6日</p>
                            </li>
                        </ul>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-look-and-feel.md" class="MCXref xref" xrefformat="{para}">23.2版本时间段内的观感更新</a></p>
                        <p>在23.2版本期限内，将对Adobe Workfront应用程序各个区域的外观进行细微更新。 在发布到“预览”后，生产环境中将至少在2周内提供这些增强功能。 </p>
                    </td>
                    <td><p><b>在以下日期可用：</b></p>
                        <ul>
                            <li>
                                <p>预览版本：在23.2版本发布的整个时间范围内<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">生产版本：发布到“预览”后至少2周（除非另有指定）</span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>

## 公告

### Workfront Fusion增强功能

在23.2版本计划之外，Workfront Fusion的新增功能在生产环境中以一定频率提供。 有关最新功能的更多信息，请参阅 [Adobe Workfront Fusion版本活动](/help/quicksilver/product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

### Workfront Scenario Planner增强功能

此时版本中没有方案计划员更新。 此区域将在更新可用时进行更新。

### Workfront Proof增强功能

此时，版本中没有Workfront校样更新。 此区域将在更新可用时进行更新。

### Workfront目标增强功能

此时，版本中没有Workfront Target目标更新。 此区域将在更新可用时进行更新。

### API版本15

对于API版本15，我们修改了一些资源和端点。 某些更改支持新功能，而其他更改则使您能够更轻松地使用通过API提供的信息。

有关新增功能和更新功能的信息，请参阅 [API版本15的新增功能](/help/quicksilver/wf-api/api/new-api-version-15.md).

有关API版本的信息，请参阅 [API版本控制和支持计划](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

### Workfront 维护更新

有关23.2版本期间进行的维护更新的信息，请参阅 [Workfront维护更新](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

### 培训更新

浏览每个Adobe Workfront产品版本的学习计划、学习路径、视频和指南的最新更新。 有关更多信息，请参阅 [培训版本更新页面](https://one.workfront.com/s/training-release-updates).

### 即将从Workfront中删除功能

以下功能即将从Workfront中删除：

#### **对Workfront默认API的更改**

为确保API调用能够利用最新的Workfront API功能，我们正在更新默认API。 当API调用未指定API版本时，将对默认API进行调用。

现在，默认API将反映API的最新版本。 今后，我们将在每次发布新API版本时更新默认API，以便对默认API的调用始终使用最新版本的API。

以前，默认API使用的是Workfront API版本2.0，该版本已弃用。

如果贵组织当前使用的是已弃用的默认API，则Workfront管理员已收到公告中心消息，其中包含有关默认API的进一步说明。

有关更多信息，请参阅 [更新使用默认API版本控制的集成](/help/quicksilver/wf-api/api/update-default-api-versioning.md).


<!--
<table>
            <col style="width: 50%;" />
            <col style="width: 50%;" />
            <tbody>
                <tr>
                    <td>
                        <p><span class="bold">Feature</span>
                        </p>
                    </td>
                    <td>
                        <p><span class="bold">Release dates</span>
                        </p>
                    </td>
                </tr>
                <tr>
                    <td>
                        <a href="ADD LINK" class="MCXref xref" xrefformat="{para}">Title</a><span style="color: #ff0000;"> New in Preview!</span></p>
                        <p>Body</p>
                    </td>
                    <td><p><b>Available on these dates:</b></p>
                        <ul>
                            <li>
                                <p>Preview release:<br /></p>
                            </li>
                            <li>
                                <p><span class="preview">Production release: </span></p>
                            </li>
                        </ul>
                    </td>
                </tr>
            </tbody>
        </table>  

        -->