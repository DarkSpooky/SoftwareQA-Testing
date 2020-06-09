---
title: \vspace{2in} 场景测试报告
subtitle: "软件质量保障与测试课程Lab9课程作业（第9组）"
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

date: "2020年6月9日"
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
\textbf{\emph{软件质量保障与测试课程Lab9课程作业}}
\end{center}

# 摘要 {-}

本次作业为软件质量保障与测试课程的Lab9课程作业，需要我们以小组为单位完成对出题系统的场景测试。本文档分为五小节。第一小节介绍了本小组进行测试计划设计的情况；第二小节介绍了本小组设计测试范围的情况；第三小节整理了本小组进行测试的结果；第四小节介绍了本小组对bug等级的评估情况；第五小节介绍了本小组对本次场景测试的测试总结。

# 关键词 {-}

系统与软件工程; 系统与软件质量要求和评价; 测试文档

\normalsize

\newpage

\tableofcontents

\newpage

# 测试简介

## 目的

编写该测试总结报告主要有以下几个目的

1．	记录测试的主要过程和测试结果

2．	评估测试测试执行和测试计划是否符合，以及测试退出准则是否满足

3．	分析系统存在的缺陷，为修复和预防缺陷提供建议

4．	对本次测试进行总结和评价，并给出改进的建议

## 用户群

1．	项目测试人员

2．	项目测试经理和管理人员

3．	其他项目相关人员

## 测试对象

目标系统及其版本

## 测试阶段

系统测试

## 测试工具

xx 测试（缺陷）管理系统

## 参考资料

1．	需求和设计说明书

2．	系统测试计划

3．	系统测试用例

#	测试概要

## 测试范围和计划

被测模块，测试方法，测试用例等等。

## 测试进度

实际测试进度


## 测试覆盖
是否完成所有的测试。
如有未完成的测试，指明原因以及何时测试。



#	测试环境

## 软件环境

## 硬件环境

## 网络环境

## 数据环境


#	测试结果分析

## 缺陷趋势

分析缺陷的趋势来确定测试是否充分。

## 缺陷优先级分析

缺陷的优先级也可以帮助分析测试是否充分，以及开发的质量。为今后开发测试的改进提供数据支持。



## 缺陷引入阶段分析

缺陷引入阶段的分析能够告诉我们在整个开发测试生命周期里，那些阶段是做的不够好的，以及今后需要如何改进。



## 缺陷引入原因分析

为改进提供数据支持


## 遗留缺陷分析

记录遗留未修复缺陷的描述，推迟原因，影响，以及修复计划。

#	测试总结

## 功能测试

总结系统的主要功能性缺陷以及修复情况。
是否满足测试的退出准则，能否上线。

## 性能测试

## 其他测试

#	测试建议

针对测试计划，执行，结果分析中出现的问题，提出改进的建议。
譬如：
针对测试流程：

1．	发布版本的时候，正确布置测试环境，减少因为测试环境，测试数据的问题而出现的无效缺陷。

2．	开发人员解决缺陷的时候，需要填写缺陷原因以及解决方式，方便缺陷的跟踪和方便测试人员今后做缺陷原因分析。

3．	开发人员在开发版本上发现缺陷，可以通知测试人员，因为开发人员发现的缺陷很有可能在测试版本上出现，而测试人员和开发人员的思路不同，有可能测试人员没有发现该缺陷，而且，这样可以保证发现的缺陷都能够被跟踪。开发人员必须使用缺陷管理工具记录单元测试的缺陷来方便共享缺陷信息。




\pagebreak

# 参考文献 {-}
