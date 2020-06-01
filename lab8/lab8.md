---
title: \vspace{2in} 场景测试报告
subtitle: "软件质量保障与测试课程Lab8课程作业（第9组）"
author:
  - Tian, Jiahe^[Equal Contribution, Fudan University, 17307130313 (tianjh17@fudan.edu.cn)]
  - Hu, Xiaoxiao^[Equal Contribution, Fudan University, 17302010077 (xxhu17@fudan.edu.cn)]
  - Huang, Jiani^[Equal Contribution, Fudan University, 17302010063 (huangjn17@fudan.edu.cn)]
  - Liu, Jiaxing^[Equal Contribution, Fudan University, 17302010049 (jiaxingliu17@fudan.edu.cn)]
  - Shi, Ruixin^[Equal Contribution, Fudan University, 17302010065 (rxshi17@fudan.edu.cn)]
  - Wu, Chenning^[Equal Contribution, Fudan University, 17302010066 (cnwu17@fudan.edu.cn)]
  - Zhang, Cenyuan^[Equal Contribution, Fudan University, 17302010068 (cenyuanzhang17@fudan.edu.cn)]
  - Zhang, Yihan^[Equal Contribution, Fudan University, 17302010076 (zhangyihan17@fudan.edu.cn)]
  - Wang, Chen^[Equal Contribution, Fudan University, 16307110064 (wangc16@fudan.edu.cn)]

date: "2020年5月31日"
documentclass: ctexart
output:
  rticles::ctex:
    fig_caption: yes
    number_sections: yes
    keep_md: yes
    keep_tex: yes
classoption: "hyperref, a4paper"
nocite: |
  @innovativeInternationalisation, @innovative1, @innovative2, @innovative3, @innovative4, @innovative5, @innovative6, @innovative7, @innovative8, @innovative9, @innovative10, @innovative11, @innovative12, @innovative13, @innovative14, @innovative15, @innovative16
references:
- id: innovativeInternationalisation
  title: "Systems and software engineering — Systems and software Quality Requirements and Evaluation (SQuaRE) — Guide to SQuaRE"
  author:
  - family: International Organization for Standardization
  container-title: International Organization for Standardization
  volume: 2014
  URL: 'https://www.iso.org/standard/64764.html'
  issue: 2
  #publisher: Kluwer Academic Publishers
  #page: 249-275
  type: book
  issued:
    year: 2014
    month: 3

- id: innovative1
  title: "GB/T 25000.51-2016《系统与软件工程系统与软件质量要求和评价 (SQuaRE) 第 51 部分 : 就绪可用软件产品 (RUSP) 的质量要求和测试细则》"
  author:
  - family: 中国国家标准化管理委员会
  container-title: 系统与软件工程系统与软件质量要求和评价 (SQuaRE)
  volume: 51
  URL: 'http://openstd.samr.gov.cn'
  publisher: 中国国家标准化管理委员会
  type: book
  issued:
    year: 2016
    month: 1
    
- id: innovative2
  title: "GB/T 25000.23-2019《系统与软件工程 系统与软件质量要求和评价(SQuaRE) 第23部分：系统与软件产品质量测量》"
  author:
  - family: 中国国家标准化管理委员会
  container-title: 系统与软件工程系统与软件质量要求和评价 (SQuaRE)
  volume: 23
  URL: 'http://openstd.samr.gov.cn'
  publisher: 中国国家标准化管理委员会
  type: book
  issued:
    year: 2019
    month: 8
    
- id: innovative3
  title: "GB/T 25000.12-2017《系统与软件工程 系统与软件质量要求和评价(SQuaRE) 第12部分：数据质量模型》"
  author:
  - family: 中国国家标准化管理委员会
  container-title: 系统与软件工程系统与软件质量要求和评价 (SQuaRE)
  volume: 12
  URL: 'http://openstd.samr.gov.cn'
  publisher: 中国国家标准化管理委员会
  type: book
  issued:
    year: 2017
    month: 11
    
- id: innovative4
  title: "GB/T 25000.24-2017《系统与软件工程 系统与软件质量要求和评价(SQuaRE) 第24部分：数据质量测量》"
  author:
  - family: 中国国家标准化管理委员会
  container-title: 系统与软件工程系统与软件质量要求和评价 (SQuaRE)
  volume: 24
  URL: 'http://openstd.samr.gov.cn'
  publisher: 中国国家标准化管理委员会
  type: book
  issued:
    year: 2017
    month: 11
    
- id: innovative5
  title: "GB/T 25000.40-201《系统与软件工程 系统与软件质量要求和评价(SQuaRE) 第40部分：评价过程》"
  author:
  - family: 中国国家标准化管理委员会
  container-title: 系统与软件工程系统与软件质量要求和评价 (SQuaRE)
  volume: 40
  URL: 'http://openstd.samr.gov.cn'
  publisher: 中国国家标准化管理委员会
  type: book
  issued:
    year: 2018
    month: 12
    
---



\newpage

\LARGE

\begin{center}
\textbf{场景测试报告}
\end{center}

\large
\begin{center}
\textbf{\emph{软件质量保障与测试课程Lab8课程作业}}
\end{center}

# 摘要 {-}

本次作业为软件质量保障与测试课程的Lab8课程作业，需要我们以小组为单位完成对出题系统的场景测试。本文档分为五小节。第一小节介绍了本小组进行测试计划设计的情况；第二小节介绍了本小组设计测试范围的情况；第三小节整理了本小组进行测试的结果；第四小节介绍了本小组对bug等级的评估情况；第五小节介绍了本小组对本次场景测试的测试总结。

# 关键词 {-}

系统与软件工程; 系统与软件质量要求和评价; 测试文档

\normalsize

\newpage

\tableofcontents

\newpage

# 测试计划
## 登录及个人信息
### 登录

* 输入正确的用户名和密码
* 输入错误的用户名和密码 

### 修改个人信息

* 登录状态下对用户名进行修改
* 登录状态下对密码进行修改
* 非登录状态下访问修改个人信息页面

## 建立新项目

### 创建项目

* 主持人登录后创建项目，确定项目名称，项目规划

### 新建考题

* 主持人创建新考题
* 主持人设置考题状态为“开始”
* 开始状态下为考题设置题目属性
* 开始状态下为考题设置相关管理人员

## 开始启动项目

### 设置期限

* 主持人为开始状态下的考题分配知识点
* 主持人设定编写考题与评审考题的时间限制

### 修改状态

* 主持人在开始状态下完成了对题目属性的设置、知识点的分配、作者、 评审员和质管员的设置后，将题目状态改为 “编写”
* 主持人在未完成相应设置时修改题目状态为编写

## 编写考题

### 设置多类型考题

* 作者编写纯文字考题
* 作者编写带有表格的考题
* 作者编写带有图形的考题
* 作者以Excel形式将考题导入出题系统
* 作者以XML形式将考题导入出题系统

### 修改状态

* 作者在编写过程中设置题目状态为“评审”
* 作者在完成编写后把题目状态设置为“评审”

## 评审考题

### 评审可接受

* 评审员设置评审结果为“可接受”

### 评审被拒绝

* 评审员设置评审结果为“被拒绝”

### 评审需修改

* 评审员设置评审结果为“需修改”

### 评审权限控制

* 评审员阅读分配属于自己评审的考题
* 评审员对属于自己评审的考题编写评审意见和建议
* 评审员改变属于自己评审的考题的状态
* 主持人阅读该考题
* 主持人修改和操作该考题

## 再审考题

### 再审可发布

* 评审员设置题目状态为“发布”

### 再审需修改

* 评审员设置评审结果为“修改”

### 再审需作废

* 评审员设置评审结果为“作废”

### 再审权限控制

* 主持人修改考题
* 主持人改变考题状态

## 修改考题

### 修改考题

* 作者阅读意见并修改考题
* 作者改变考题状态为“评审”

### 修改权限控制

* 主持人修改考题
* 主持人改变考题状态

## 发布考题

### 导出发布考题

* 主持人在考题处于“发布”状态下导出考题
* 主持人在考题处于“发布”状态下修改考题

### 导入题库

* 题库系统管理员将已发布并且由主持人导出的考题文件导入题库

## 作废考题

### 废除作废考题

* 主持人查看作废考题
* 主持人修改考题或改变状态

### 重启出题流程

* 主持人查看作废考题后重新启动项目

## 生成考卷

### 填写考试名称
* 输入合法的考试名称
* 输入非法的考试名称

### 设置题目总数
* 输入范围为1~5的数字

### 选择试卷难度
* 选择简单
* 选择一般
* 选择困难

### 填写开始时间
* 填写格式正确的时间
* 填写格式错误的时间

### 填写结束时间
* 填写格式正确的时间
* 填写格式错误的时间

### 选择章节
* 选择具体的章节

### 选择考试学生
* 选择本次考试的学生

## 考试

### 查看考卷
* 点击侧边栏查看考卷

### 参加考试
* 点击图标开始开始
* 点击考题答案的单选框进行选择

### 提交考卷
* 回答完所有题目提交考卷
* 没有答完所有题目提交考卷

### 查看分数
* 点击查看成绩
* 没有参加考试时点击查看成绩



# 测试范围制定

## 出题场景

### 登录及个人信息
* 登录
* 修改个人信息

### 建立新项目
* 创建项目
* 新建考题

### 开始启动项目
* 设置期限
* 修改状态

### 编写考题
* 设置多类型考题
* 修改状态

### 评审考题
* 评审可接受
* 评审被拒绝
* 评审需修改
* 评审权限控制

### 再审考题
* 再审可接受
* 再审被拒绝
* 再审需修改
* 再审权限控制

### 发布考题
* 导出发布考题
* 导入题库

### 作废考题
* 废除作废考题
* 重启出题流程

## 创建试卷与考试场景

### 登录及个人信息
* 登录
* 修改个人信息

### 生成考卷
* 填写考试名称
* 设置题目总数
* 选择试卷难度
* 填写开始时间
* 填写结束时间
* 选择章节
* 选择考试学生

## 参加考试场景

### 登录
* 登录

### 查看考卷
* 查看考卷

### 参加考试
* 参加考试
* 开始考试

### 提交考卷
* 提交考卷

### 查看分数
* 查看分数


# 测试结果整理

# bug等级评估

# 总结陈词

##组卷部分
对于组卷部分，管理员在登录后，点击查看考卷进入到组卷页面。然后依次输入考试名称，选择题目总数、试卷难度，输入开始和结束时间，选择章节以及选择参与这场考试的学生，这些是完成一次成功的组卷所必须经过的步骤。在这部分操作之外，登录及个人信息部分测试了错误的用户名密码的输入，以及修改个人信息。组卷部分对输入非法名称，格式错误的开始和结束时间这两个容易发生的错误操作进行了测试。
首先，对于组卷功能涉及的一系列操作都已经实现，可以完成一次成功的组卷。对于输入的非法的考试名称（此处使用的是为空的名称进行测试），系统能够给出提示。所以系统在正确使用的前提下可以正常工作，对于操作过程中可能出现的错误，系统也进行了一定的错误处理。但个人信息修改因为功能包含在出题系统中，所以同样没有实现，以及在输入格式错误的时间时，系统给出的提示是http的状态500，对于用户来说可能无法立刻明白出错的原因，但通过修改为正确的格式可以完成组卷。所以系统中还包含了一些未实现的需求以及用户不友好的部分，但并不是致命性的错误。
系统其他可能存在的风险包括其他的非法输入以及安全性方面的风险。对于非法名称，只测试了为空，而没有测试重复的名称和过长的名称。对于章节和学生选择的多选框如果没有进行选择的情况没有进行测试，以及在没有登录的情况下是否能进入这一界面没有测试。

##考试部分
考试部分的必经流程包括，学生登录，查看自己参加的所有考试，开始考试并获取试卷，点击单选框选择答案，提交考卷，最后查看自己分数。除了以上的步骤外，包括了使用错误的用户名和密码登录，在没有答完所有题目的情况下提交试卷，以及在没有参加考试时查看分数。
在操作正确的前提下，参加考试并获取分数这一系列的步骤可以正常完成。对于没有参加的考试，查看到的分数为零分。但在没有答完所有题目的情况下提交试卷，系统会给出错误提示，这与一般的处理方法并不一致。所以系统对于基本的操作流程，大体实现了相关功能，但对于一些特殊情况，系统的处理可能与常理不同，应当加以说明。
没有覆盖的风险包括与考试时间相关的错误操作以及安全性相关的风险，如在考试未开始或结束后试图开始考试，在考试结束前查看成绩，在没有登录的情况下进行除了登录以外的操作，以及尝试获取自己没有参加的考试的试卷。


\pagebreak

# 参考文献 {-}
