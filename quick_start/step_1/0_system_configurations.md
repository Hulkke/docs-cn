# Step 1：完成系统基础设置

<br />

## 要点概述

-   完成基础的系统设置后，即可新增或导入代码库来进行数据分析。

-   系统设置中，包含：基础设置、自定义字段设置、SMTP 设置、登录鉴权设置、LDAP 设置、周日报配置、专家系统开关、安全性设置。

<br />

## 入口导航

**设置 > 系统设置**

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/20220226104354.png" />

<br />

## 基础设置

通过基础设置，设定系统运行所必须的基本参数。点击 **基础设置** 版块处的 **应用** 按钮，保存基础设置信息。

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/Basic_Settings.png" />

### -站点地址

当前系统站点地址，以“/”结尾。

### -系统时区

周报/日报邮件发送时间和系统设置时区一致。

### -工作日

周报中的统计数据，只统计工作日相关数据，不包含非工作日数据。

### -启用站内通知

勾选此选项时，会按照【通知设置】中的设置规则给相关账户发送站内通知。

<br />

## 自定义字段

配置自定义字段，并且给团队成员账户赋予自定义字段中的值，即可在【团队表现】中使用该自定义字段值进行筛选，汇总数据。

如：添加自定义字段“岗级”，并设置该自定义字段的三个可选值：Export，Master，Professor，即可在【账户设置】处给账户配置此三个岗级。

完成自定义字段设置后，点击此版块的 **应用** 按钮，保存此处设置。

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/Custom_Fields.png" />

<br />

## SMTP 设置

配置系统发件邮箱、发件邮箱密码、SMTP 服务器地址信息，通过 SMTP 服务器发送邮件，如成员账户信息、修改密码信息、周报/日报邮件。

如果没有配置 SMTP 发件邮箱，那么启用新账户的密码和给已有账户重置密码需要在【账户管理】界面上直接输入需要的密码，而不是通过邮件发送密码。

点击 **SMTP 设置** 版块处的 **应用** 按钮，保存发件设置信息。

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/SMTP.png" />

<br />

## 登录鉴权

通过配置基于 OAuth2.0 的参数项，用户可以凭借在其他平台的账号，通过授权的方式一键登录思码逸系统。

点击 **登录鉴权** 版块处的 **应用** 按钮，保存登录鉴权信息。

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/OAuth.png" />

<br />

## LDAP 设置

通过设置 LDAP 参数，可以接入企业内部的 LDAP 服务器，实现单点登录。

点击 **LDAP 设置** 版块处的 **应用** 按钮，保存 LDAP 设置信息。

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/LDAP.png" />

<br />

### -LDAP 地址

LDAP 服务器地址

### -Bind DN

绑定 DN 信息：用户名，域名

### -Bind Credentials

绑定密码

### -CA Certificate

CA 认证信息

### -Search Base

LDAP 服务器域名信息

### -Search Filter

LDAP 服务器用户名查找定位

### -Email attribute

Email 属性信息

<br />

## 周日报配置

可以设置全部代码库定时自动分析时间，分析数据可以以周报或日报的的形式发送，报告类型、接收范围、发送时间都可以灵活配置。

点击 **周日报配置** 版块处的 **应用** 按钮，保存周日报配置信息。

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/Reports_Settings.png" />

<br />

### -管理者报告

管理者报告内容主要为研发情况数据汇总和概况总览。为了保证信息安全，报告接收者只会收到其有权限访问的项目数据汇总。

可以通过勾选 **日报** 和/或 **周报**，配置 **接收范围** 指定某些角色的账户可以收到管理者日报和/或周报。

请注意，选择日报时，分析引擎会每日启动分析，需要确认资源足够支持在当天完成分析。

<br />

### -开发者报告

开发者报告内容主要为程序员个人工作汇总。

可以通过勾选 **日报** 和/或 **周报**，配置 **接收范围** 指定某些角色的账户可以收到开发者日报和/或周报。

请注意，选择日报时，分析引擎会每日启动分析，需要确认资源足够支持在当天完成分析。

<br />

### -报告发送时间

报告发送时间可以选择 **快速配置** 和 **高级配置** 两种模式进行配置。选择 **快速配置** 模式时，仅需选择周报和日报发送时间，系统会根据报告发送时间相应调整全部代码库定时启动分析时间。选择 **高级配置** 模式时，可以使用 **Cron 表达式** 精细配置不同报告发送时间和全部代码库定时启动分析时间。

**系统维护窗口：** 系统维护将在指定的时间窗口期每日自动进行，清理过期报告和已删除的代码库数据。维护完成后将显著缩短数据加载时间。整个维护过程大约持续 2 小时，在维护窗口期内系统响应速度可能会有所下降，请根据实际情况设置合理的系统维护时间。

**重新计算时间：** 当调整了问题忽略规则设置后，需要重新统计相关质量问题数据。此处设置用于设置在每天系统维护时（上一条系统维护窗口设置时间），花多长时间重新生成质量数据统计。为 0 时关闭本功能，为 5 小时时，每天花 5 小时重新生成质量数据统计。

<br />

### -启用在职人员白名单

勾选白名单选项，报告数据中仅包含在职人员，不包含已离职人员数据。

<br />

## 专家系统

勾选是否打开专家系统功能，打开此功能开关后，在 **项目表现、团队表现** 等模块会对数据表现给出分析和建议。

<br />

## 安全性

选择代码预览模式，控制产品里各代码展示模块里可见代码范围。

<br />

<img style="border-radius: 0.3125em;
    box-shadow: 0 2px 4px 0 rgba(34,36,38,.12),0 2px 10px 0 rgba(34,36,38,.08);" src="https://release-note.oss-cn-hongkong.aliyuncs.com/img/Expert_Security.png" />
