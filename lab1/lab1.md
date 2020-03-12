---
title: \vspace{2in} 出题系统需求文档
subtitle: "软件质量保障与测试课程Lab1课程作业（第9组）"
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

date: "2020年3月12日"
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
\textbf{出题系统需求文档}
\end{center}

\large
\begin{center}
\textbf{\emph{软件质量保障与测试课程Lab1课程作业}}
\end{center}

# 摘要 {-}

本次作业为软件质量保障与测试课程的Lab1课程作业，需要我们以小组为单位阅读、理解出题系统初始需求文档，进行小组讨论，结合软件质量相关属性，提出潜在存在的需求重构点，并自定义需求规范撰写需求文档，结合“禅道”平台辅助进行需求管理。

# 关键词 {-}

系统与软件工程; 系统与软件质量要求和评价; 需求文档



# 版本历史 {-}
\begin{center}
%干我的居中失败了why
\begin{tabular}{|l|l|l|}
\hline
版本 & 日期 & 说明\\
\hline
草稿 & 2014 年2 月6 日 & 建立此文档\\
\hline
Alpha 版 & 2014 年2 月8 日 & 做了修改后进行内部评审\\
\hline
Alpha 03 & 2014 年2 月9 日 & 魏X 内部评审稿\\
\hline
Alpha 04 & 2014 年2 月11 日 & 黄X 增加属性，完善评审流程\\
\hline
Alpha 05 & 2014 年2 月14 日 & 增加周X 的问题\\
\hline
Alpha 06 & 2014 年2 月17 日 & 增加T 模块考卷规则、增加分值规则\\
\hline
发布版 1.0 & 2014 年3 月10 日 & 修改后发布\\
\hline
发布版 2.0 & 2014 年3 月16 日 & 评审后，经修改后发布\\
\hline
修订版3.1 & 2014 年4 月25 日 & 与开发商和办公室讨论后收集的建议和问题\\
\hline
修订版3.2 & 2014 年5 月21 日 & 回答魏X 的问题\\
\hline
修订版3.3 & 2014 年6 月30 日 & 根据开发商反馈建议和需求细化后整理。\\
%\hline
%发布版3.0 & 2014 年7 月1 日 & %\makecell[l]{修改后发布。所有状态的描述重新编写，更加便于理解。\\加入新的考题属性“理论实践”。部分修改和完善。}\\
\hline
修订版4.0 & 2020 年3 月12 日 & 进行合理性检查和规范定义后整理。\\
\hline
\end{tabular}
\end{center}

\normalsize

\newpage

\tableofcontents

\newpage
# 在线出题考试系统概述（完整系统）{-}
“在线出题考试系统”是为组织考试的一个基于Web 的在线系统，主要由“出题系统”、“题库管理系统”、“在线报名和考生管理系统”以及“考试系统”四大模块（子系统）组成。

# 出题系统描述 {-}
出题系统是在线出题考试系统的的一个子系统。利用出题系统，出题专家们可以方便的进行网上考题编写和评审，并无缝的与在线出题考试系统进行衔接，提高考题编写的质量和效率，也便于考题的统一管理和评估。
在出题系统中，每一次的出题活动定义为一个“项目”（Project），每个项目有它的目的、内容、角色（成员）、时间（限期）和结果（输出）。例如：某一个项目可能要求出一份或几份完整的，有若干考题组成的完整“考卷”，也有可能是针对某一个或某几个“知识点”编写相应考题。在一个项目中定义了一系列“角色”，如项目的“主持人”、编写考题的“作者”和考题的“评审员”以及最后对考题把关的“质管员”等。
在出题系统中的最小单元是“考题”，“考题”包括了“考题信息”和“考题属性（辅助信息）”，“考题信息”又有“场景描述”（可有可无）、“题干”和“选项”组成；而“辅助信息”是指“考题”在它的整个生命周期中，在管理、统计、评估和自动出考卷过程所使用的一些辅助元素，在这里称为考题的“属性”，包括此考题覆盖大纲的“章节”、“知识点”和“K级（Kn）”、“状态”、“作者”、“评审员”、“质管员”、“发布时间（启用时间）”、“使用次数（使用频率）”、“答对率（每次累加）”、“答错率（每次累加）”、“出题难度（作者的预估）”、“反馈难度（学生反馈）”等（可参看考题属性描述）。这些考题经编写、评审并通过审核后可以“发布”，并以统一的格式导出和存放到题库管理系统。


# 定义（未完成，需完善）
## 基本定义
### 考卷
考卷是由若干考题组成，并按照出题规则，主要根据考卷相对应大纲的知识点（对应大纲的章/节）以及知识点的K级，可参看考卷组成规则。

### 考题
考题是组成考卷的最小单位，由属于考题本身的考题信息以及为管理考题所需的考题属性组成。考题信息又包括该考题场景、考题题干和考题选项。考题属性包含对考题管理所需的各种属性，如考题的作者、考题的ID、考题评审者、考题的状态等，可参看考题属性表。

### 知识点
考题根据大纲所覆盖的章节内容，是出题的依据和范围。且每个知识点有其对应的K级别。

### 正确选项
考题可以是正选题，例如在考题中选择哪项是正确的，也可以是反选题，例如在考题中要求选择哪个是错误或不正确的，无论是正选还是反选题，如果考生做了正确的选择，那个被选中的选项定义为正确的选项。

## 出题系统角色：
### 系统管理员
负责该系统中所有用户账户的开设，创建新项目（项目名+主持人）；对整个系统的配置
和运行负责；维护系统和系统数据（如大纲知识点的更新等）。
### 主持人
整个考题的编写和评审流程的发起人和负责人。指定此次考题对应的大纲知识点，将考
题分配给指定的作者、评审员和质管员，设定考题编写和评审时限。可以导出质管员同
意发布的考题。每题考题的评审员可以有多人。
### 作者
考题的编写者，收到由主持人指定需要出的考题对应的大纲知识点等信息后开始编写考
题，也可根据评审员的意见修改考题。
### 评审员
可对由主持人分配的，并由对应作者已编写的考题进行评审，提出评审和修改意见。
### 质管员
是最后保障考题质量的把关和负责人，由主持人指定考题的质管员，在考题通过评审后
进入“再审”状态，在“再审”状态下质管员决定是否需要返回给作者修改或者直接发
布或者作废。

## 考题的状态
### 开始状态
由主持人创建一个新的考题（考题的ID），新创建考题的状态为“开始”。主持人在开始
状态为考题建立框架，分配考题对应的知识点、时间安排、分配作者和评审员以及质管
员等，完成相关设定后主持人将考题的状态从“开始”改为“编写”状态。
### 编写状态
在“编写”状态下，作者根据被指定的章节知识点来编写考题信息内容（场景，题干，
选项），作者填写必须或应该填写的考题属性内容。作者编写考题完毕后，作者将此考题
的状态从“编写”改写为“评审”状态。
### 评审状态
在“评审”状态下，评审员对作者编写或修改的考题进行评审，每一考题的评审员由主
持人事先指定。评审员完成评审活动后，根据评审结果评审员可将此考题的状态从“评
审”改写为“再审”或“修改”状态。例如，评审结果为“可接受”或“被拒绝”，则评
审员将此考题的状态从“评审”改写为“再审”状态。如果评审结果为“需修改”，则评
审员将此考题的状态从“评审”改写为“修改”状态。
### 再审状态
当考题处于“再审”状态，质管员对考题质量进行再次审核。根据再审结果，质管员可
以将此考题的状态从“再审”改为“修改”、“发布”或“作废”状态。
*备注：评审员或质管员应该在规定时限内完成评审活动并提交评审意见，如果超出规定时限评审员没有完成评审，系统自动向相关评审员或质管员发出提示信息（Mail），并同时向主持人发出信息（Mail），收到信息后主持人根据实际情况重新进行调整，可通过多重渠道进行调整：延长时间、重新安排评审员或质管员、直至删除该题等。*
### 修改状态
当考题处于“修改”状态时，考题的作者可以对考题进行修改，作者一般是参照评审的
记录和要求对考题进行修改。修改完毕后，作者可将此题的状态从“修改”改为“评审”
状态。
### 发布状态
当考题处于“发布”状态时，表示此题已经通过编写和评审，可以被使用了。主持人可
以导出此状态下的考题。主持人可以单题导出，也可以批量导出。
### 作废状态
当考题处于“作废”状态时，表示此题由于各种原因不被接受，也不会使用，主持人对
此类考题按照规定进行处理，例如删除。

# 功能性需求

## 功能-需求名
- 关键词
- 需求描述（参考模板：作为一种<某类型的用户>,我希望<达成某些目的>,这样可以<开发的价值>)
- 验收标准
- （图）

## 功能-需求名2
- 关键词
- 需求描述（参考模板：作为一种<某类型的用户>,我希望<达成某些目的>,这样可以<开发的价值>)
- 验收标准
- （图）

# 质量需求
## 质量-需求名
- 关键词
- 需求描述
- 验收标准

## 质量-需求名2
- 关键词
- 需求描述
- 验收标准

# 约束条件
## 约束-需求名
- 关键词
- 需求描述
- 验收标准

## 约束-需求名2
- 关键词
- 需求描述
- 验收标准



\pagebreak

# 参考文献 {-}
