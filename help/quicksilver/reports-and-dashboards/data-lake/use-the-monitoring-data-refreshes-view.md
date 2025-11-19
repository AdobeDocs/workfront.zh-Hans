---
product-area: reports and dashboards
navigation-topic: data-connect
title: 在Data Connect中使用监控数据刷新视图
description: 借助Data Connect，Workfront管理员可以访问最近刷新期间对数据湖日期所做的最新更新的详细记录。
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# 在Data Connect中使用监控数据刷新视图

监控数据刷新视图显示最近刷新期间对数据湖日期所做的最新更新。 每次成功完成数据加载后，此视图的数据都会更新。

由于数据量大和聚合的复杂性，监控数据刷新视图仅显示最近2周内更新的对象视图。 如果此视图中没有特定记录类型，则可能是由于该时间范围内缺少活动。

>[!NOTE]
>
>此视图显示应用程序和刷新活动提供的数据的详细集合，而不是显示刷新活动历史记录的每日历史记录或事件视图。 要获取历史刷新活动详细信息，您可以使用<code>DL_LOAD_TIMESTAMP</code> 日期对象。

## 监控数据刷新视图列

“监视数据刷新”视图列包含以下信息：

<table>
    <tr>
        <td><b>列名称</b></td>
        <td><b>类型</b></td>
        <td><b>描述</b></td>
    </tr>
    <tr>
        <td>对象类型</td>
        <td>Varchar
        </td>
        <td> 
      与发送到数据湖的Workfront记录关联的对象类型。 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>日期</td>
        <td>
   在OBJ_TYPE列中显示的对象类型上次成功刷新数据的日期。 </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 在OBJ_TYPE列中显示的对象类型的最新数据刷新日期和时间。  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       在OBJ_TYPE列中显示的对象类型第二次刷新数据的日期和时间。 </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>数值</td>
        <td>
     自上次刷新对象类型数据以来经过的时间（以分钟为单位）。 </td>
    </tr>
            <tr>
        <td>已创建 </td>
        <td>数值 </td>
        <td>在对象类型的前次和最新数据刷新之间捕获的CREATE记录事件的计数。  </td>
    </tr>
                <tr>
        <td>已更新</td>
        <td>数值 </td>
        <td>在对象类型的前次和最新数据刷新之间捕获的UPDATE记录事件的计数。</td>
    </tr>
                <tr>
        <td>已删除</td>
        <td>数值 </td>
        <td>在对象类型的前次和最新数据刷新之间捕获的DELETE记录事件计数。 </td>
    </tr>
                <tr>
        <td>总计</td>
        <td>数值 </td>
        <td>对象类型在上一次和最近一次数据刷新之间发生的事件总数。 
        <br> 
        <br><b>注意</b>：这与受CREATE、UPDATE或DELETE事件影响的记录总数不同，因为在两次刷新间隔内，同一记录可能会被多次创建和更新。  </td>
    </tr>
   </table>

