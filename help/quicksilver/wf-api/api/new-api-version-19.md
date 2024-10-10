---
content-type: api
navigation-topic: api-navigation-topic
title: API版本19中的新增功能
description: Adobe Workfront于2022年4月6日发布了API版本19。 API版本19具有来自版本18的以下更改。
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 13910328903744aa9bf619e8b4c376520c21b89e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# API版本19中的新增功能

Adobe Workfront于2024年4月8日发布了API版本19。 API版本19具有来自版本18的以下更改。

## 已添加资源

没有为API版本19添加资源。

## 已删除资源

没有为API版本19删除资源

## 已修改的资源

### 访问级别(ACSLVL)

AccessLevel对象与用户相关联，并描述确定用户可以访问的AccessLevelPermissions集。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>添加了以下可能值：
            </p>
            <ul>
              <li>
                <p>禁用Workfront AI助手(AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 分配(ASSGN)

Assignment对象表示工作项与分派处理该工作项的用户、团队或组之间的连接。

任务对象添加了标志&#x200B;**DATA_EXTENDIBLE**。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下直接字段：
        <ul>
          <li>
            <p><b>类别ID</b><p>类别是自定义表单。 此字段支持向分配添加自定义表单的功能。
            </p>
          </li>
          <li>
            <p><b>优先次序</b><p>此字段允许使用以下值：
            <ul>
              <li>0（无）</li>
              <li>1（低）</li>
              <li>2（正常）</li>
              <li>3（高）</li>
              <li>4（紧急）</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>添加了以下参考字段：
        <ul>
          <li>
            <p><b>类别</b><p>类别是自定义表单。 此字段支持向分配添加自定义表单的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>添加了以下收藏集字段：
        <ul>
          <li>
            <p><b>对象类别</b><p>类别是自定义表单。 此字段支持向分配添加自定义表单的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### 类别(CTGY)

Category对象是自定义表单。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下字段以支持向分配添加自定义表单的功能。
        <ul>
          <li>
            <p><b>catObjCode</b><p>添加了以下可能值：
            </p>
            <ul>
              <li>
                <p>分配(ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>对象类型</b><p>添加了以下可能值：
            </p>
            <ul>
              <li>
                <p>分配(ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 分类器(CLSF)

分类器是一个位置。

<table>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>添加了以下操作：
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 客户

Customer对象表示一个使用Workfront实例的组织。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumType</b><p>添加了以下可能值：
            </p>
            <ul>
              <li>
                <p>分配优先级(PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>CustomEnum对象有助于将状态代码转换为人类可读的文本。</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 客户首选项(CUSTPR)

CustomerPreferences对象表示客户为其Workfront实例设置的首选项集。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>删除了以下可能值：
            </p>
            <ul>
              <li>
                <p>在更新流中启用缩放集成（密码：zoomIntegrationEnabled）
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 文档(DOCU)

Document对象表示文件（如书面材料、图像或其他形式的信息）。

<table>
  <tbody>
    <tr>
      <td role="rowheader">操作</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>已添加字段<code>folderID</code>。</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>已添加。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### 汇率（汇率）

ExchangeRate对象表示在Workfront中设置的货币汇率。 ExchangeRate对象不是动态的。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
      <ul>
      <li>以下字段已添加验证器<code>REQUIRED</code>：
        <ul>
          <li><p><b>货币</b></li>
          <li><p><b>费率</b></li></ul>
      <li>添加了以下字段：
        <ul>
          <li><p><b>enteredById</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
      <ul>
        <li>添加了以下字段：
        <ul>
          <li><p><b>输入者</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 组（组）

组对象表示一组用户和团队。 组通常代表部门结构。

组对象添加了标志&#x200B;**可共享**。

### Hour (HOUR)

Hour对象表示用户在时间表上记录的小时。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
      添加了以下字段：
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submittedById</b></li>
          </ul>
          <p>对<b>小时</b>字段进行了以下更改。</p>
          <ul> 
          <li> 已删除验证器<b>GREATER_THAN</b></li>
          <li> 已添加验证器<b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">操作</td>
      <td>
      已添加以下操作：
        <ul>
          <li><p><b>批准</b></li>
          <li><p><b>取消批准</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### 日志条目(JRNLE)

JournalEntry对象可以设置为在修改特定对象字段时记录这些字段的相关信息。 将某个字段设置为记录为日志条目对象的一部分时，每次修改该字段时将创建相应的日志条目。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>标志</b><p>添加了以下可能值：
            </p>
            <ul>
              <li>
                <p>为成本率(CR)
                </p>
              </li>
              <li>
                <p>记帐费率(BR)
                </p>
              </li>
              <li>
                <p>为一般财务(GF)
                </p>
              </li>
              <li>
                <p>为组合财务(CF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### 参数（参数）

Parameter对象是一个自定义字段。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
        <ul>
          <li>
            <p><b>数据类型</b></p><p>添加了以下可能值：
            <ul>
            <li>持续时间(DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>显示类型</b></p><p>为了创建更便于用户使用且更灵活的系统，<b>小组件（小组件）</b>字段类型已被弃用，并被拆分为以下字段类型：
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>图像(IMAGE)</li>
            <li>PDF(PDF)</li>
            <li>视频（视频）</li>
            <li>外部查找(EXTRNL)</li>
            <li>多选外部查找(MULTEXTRNL)</li>
            <li>本机字段(WFNATIVE)</li>
            <li>计划字段(WFPLANNING)</li>
            <li>时间分段KPI（按时间分段）</li>
            <li>汇总（汇总）</li>
            <li>文档（文档）</li>
           </ul>
          </li>
          <li>
            <p><b>配置</b><p>已添加。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### 角色(ROLE)

角色对象（工作角色）表示用户可能填充的功能能力或技能集，如Designer或产品经理。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
    添加了以下字段：
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>
        添加了以下字段：
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### 记分卡问题 {#scorecardquestion}

ScoreCardQuestion对象表示已添加到记分卡的问题。 这些问题通常由Portfolio经理决定，这些问题的答案让经理能够了解项目与项目组合目标的符合程度。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>
            <p><b>显示类型</b></p><p>为了创建更便于用户使用且更灵活的系统，<b>小组件（小组件）</b>字段类型已被弃用，并被拆分为以下字段类型：
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>图像(IMAGE)</li>
            <li>PDF(PDF)</li>
            <li>视频（视频）</li>
            <li>外部查找(EXTRNL)</li>
            <li>多选外部查找(MULTEXTRNL)</li>
            <li>本机字段(WFNATIVE)</li>
            <li>计划字段(WFPLANNING)</li>
            <li>时间分段KPI（按时间分段）</li>
            <li>汇总（汇总）</li>
            <li>文档（文档）</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TASSGN)

TemplateAssignment对象表示模板任务与分配给其工作的用户、团队或组之间的连接。 当模板用于项目时，该用户、团队或组会被分配给任务。

TemplateAssignment对象添加了标志&#x200B;**DATA_EXTENDIBLE**。

<table>
  <tbody>
    <tr>
      <td role="rowheader">直接字段</td>
      <td>添加了以下直接字段：
        <ul>
          <li>
            <p><b>类别ID</b><p>类别是自定义表单。 此字段支持向分配添加自定义表单的功能。
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">引用字段</td>
      <td>添加了以下参考字段：
        <ul>
          <li>
            <p><b>类别</b><p>类别是自定义表单。 此字段支持向分配添加自定义表单的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">收藏集字段</td>
      <td>添加了以下收藏集字段：
        <ul>
          <li>
            <p><b>对象类别</b><p>类别是自定义表单。 此字段支持向分配添加自定义表单的功能。
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### 时间表(TSHET)

工时表对象表示一个虚拟工时表，允许用户输入任务、项目和管理费用小时类型的实际工作小时数。

<table>
  <tbody>
    <tr>
      <td role="rowheader">核心字段</td>
      <td>
        <ul>
          <li>
            <p><b>对象代码</b></p><p>已删除。</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


