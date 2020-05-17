---
title: \vspace{2in} 黑盒测试设计与执行
subtitle: "软件质量保障与测试课程Lab5课程作业（第9组）"
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

date: "2020年5月2日"
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
\textbf{黑盒测试设计与执行}
\end{center}

\large
\begin{center}
\textbf{\emph{软件质量保障与测试课程Lab5课程作业}}
\end{center}

# 摘要 {-}

本次作业为软件质量保障与测试课程的Lab5课程作业，需要我们以小组为单位完成对出题系统的黑盒测试。本文档分为三小节。第一小节介绍了本小组设计的黑盒测试整体框架以及测试流程；第二小节介绍了黑盒测试中的关键字以及测试数据设计；第三小节介绍了本小组对黑盒测试任务的具体脚本实现以及运行情况介绍。

# 关键词 {-}

系统与软件工程; 系统与软件质量要求和评价; 测试文档

\normalsize

\newpage

\tableofcontents

\newpage

# 测试框架设计

## 黑盒测试框架图

在本节内容中，将会通过两个图对本小组设计的黑盒测试框架进行描述。

其中程序流程图将整个黑盒测试的各个步骤进行了分解，展现了整个测试过程中不同动作执行的先后顺序以及之间的关联关系。而UML类图将黑盒测试的框架组成进行了分解，说明了测试框架中各个模块之间的关系。

\begin{figure}
  \centering
  \includegraphics[scale=0.5]{./FlowChart.pdf}
  \caption{黑盒测试流程图}\label{1}
\end{figure}

\begin{figure}
  \centering
  \includegraphics[scale=0.75]{./ClassDiagram.pdf}
  \caption{黑盒测试整体框架图}\label{2}
\end{figure}

\begin{figure}
  \centering
  \includegraphics[scale=0.85]{./KeywordsDiagram.pdf}
  \caption{黑盒测试关键词设计框架图}\label{3}
\end{figure}

\begin{figure}
  \centering
  \includegraphics[scale=0.85]{./ActionEngineDiagram.pdf}
  \caption{黑盒测试用例执行组件框架图}\label{4}
\end{figure}

\pagebreak

## 黑盒测试框架图说明

# 关键字及测试数据设计

## 测试关键字
### 登录
### 创建考题
创建考题需要完成考题的相关设定。这些设定包括选择章节、选择知识点、设置作者、设置评审
、设置质管、设置类型、设置语言、设置出题日期、设置评审日期。而创建考题作为一个独立的UI测试，登录是一个基础环节。于是我们针对上述的关键步骤设计了以下关键字：
+ loginActions 登录系统
+ navigateToAddQuestion 页面导航
+ showEditQuestion 选择添加考题
+ chooseChapter 选择章节
+ chooseKnowledgePoint 选择知识点
+ chooseAuthor 设置作者
+ chooseReviewer 设置评审
+ chooseQA 设置质管
+ chooseType 设置题目类型
+ startDate 设置出题开始日期
+ finishDate 设置出题结束日期
+ reviewStartDate 设置评审开始日期
+ reviewFinishDate 设置评审结束日期
+ chooseLanguage 选择语言
+ saveQuestion 保存考题

其中我们没有将登录拆分为更加细致的行为，这是因为登录对于创建考题环节而言是比较基础和简单的。它不是本黑盒测试的考察内容。

## 测试数据
### 登录
####等价类划分与边界值分析

####测试数据

### 创建考题
#### 等价类划分

创建考题的UI测试具备多个输入参数，并且这些参数的取值也多种多样。我们对输入参数进行等价类划分:

\begin{table}[!htbp]
  \caption{等价类划分}
  \label{Tab:bookRWCal}
  \centering
  \begin{tabular}{|p{3.5cm}|p{5.0cm}|p{4.0cm}|}
  \hline
  \textbf{输入参数} &\textbf{有效等价类果} &\textbf{无效等价类 }\\
  \hline
  Chapter     & [1]任何章节 	& [2]为空 \\
  \hline
  Knowledge point  & [3]章节下任意知识点 	& [4]为空  \\
  \hline
  Author   & [5]任意用户  	& [6]为空 \\
  \hline
  Reviewer    & [7]除author外用户   	& [8]author \newline [9]为空 \\
  \hline
  QA     & [10]除author，reviewer外用户    	& [11]author或reviewer
\newline [12]为空 \\
  \hline
  Type     & [13]任意类型    	& [14]为空  \\
  \hline
  Start date   & [15]任意日期    	& 16]为空  \\
  \hline
  Finish date      & [17]在开始日期及之后的日期  	& [18]为空 \\
  \hline
  Review start date    & [19]出题开始日期及之后日期    	& [20]为空 \newline [21]出题开始日期之前 \\
  \hline
  Review finish date   & [22]评审开始日期及之后的日期，且不早于出题结束日期  	& [23]为空 \newline  [24]出题结束日期之前 \\
  \hline
  Language    & [25]任意语言  	& [26]为空 \\
  \hline
  \end{tabular}
\end{table}

表7是根据等价类划分设计的测试用例，其中c0表示第一个章节，k0表示该章节第一个知识点，u0表示成员1，u1表示成员2，u2表示成员3，t0表示类型为情景题，l0表示语言为中文。

\begin{table}[!htbp]
  \caption{等价类划分测试数据}
  \centering
  \begin{tabular}{|p{0.35cm}|p{1.2cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.9cm}|p{0.9cm}|p{0.9cm}|p{0.9cm}|p{0.22cm}|p{0.8cm}|}
  \hline
  \textbf{ID} & \textbf{类} & \multicolumn{11}{c|}{\textbf{输入参数}} & \textbf{预期}  \\ 
  \hline
1   & 1,3,5,7, 10,13,15, 17,19,22, 25 & c0  & k0 & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-03 & 2020-05-03 & 2020-05-03 & l0 & 成功   \\
  \hline
2   & 2  & 空 & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-03  
& 2020-05-03 & 2020-05-03 & l0 & 失败   \\
  \hline
3   & 4  & c0 & 空 & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
4   & 6  & c0 & k0  & 空 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
5   & 8  & c0 & k0  & u0 & u0 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
6   & 9  & c0 & k0  & u0 & 空 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
7   & 11 & c0 & k0  & u0 & u1 & u1 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & 0  & 失败   \\
  \hline
8   & 12 & c0 & k0  & u0 & u1 & 空 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
9   & 14 & c0 & k0  & u0 & u1 & u2 & 空  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline 
10  & 16 & c0 & k0  & u0 & u1 & u2 & t0  & 空         & 2020-05-04  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
11  & 18 & c0 & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 空  
& 2020-05-03 & 2020-05-04 & l0 & 失败   \\
  \hline
12  & 20 & c0 & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 空         & 2020-05-04 & l0 & 失败   \\
  \hline
13  & 21 & c0 & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-04-30 & 2020-05-04 & l0 & 失败   \\
  \hline
14  & 23 & c0 & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 空         & l0 & 失败   \\
  \hline
15  & 24 & c0 & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-03 & l0 & 失败   \\
  \hline
16  & 26 & 0  & 0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04  
& 2020-05-03 & 2020-05-04 & 空 & 失败   \\

  \hline
  \end{tabular}
\end{table}

\pagebreak

#### 边界值分析

边界值分析适用于具有连续取值的参数分析，题目中具有连续取值的只有出题日期与评审日期。
其中出题开始日期不存在边界限定，故不考虑。而对于评审结束日期，它的边界值与评审开始日期和出题结束日期相关。由于这两个日期不存在约束关系，
故它的多个边界值条件可以同时成立。对于不存在连续取值的参数，此处边界值分析不再进行罗列，在测试数据中会使用固定的取值。

\begin{table}[!htbp]
  \caption{边界值分析}
  \label{Tab:bookRWCal}
  \centering
  \begin{tabular}{|p{6.0cm}|p{6.5cm}|}
  \hline
  \textbf{输入参数} &\textbf{边界值} \\
  \hline
  Finish date     & [27]与start date相同 	\newline [28] start date后一天 \\
  \hline
  Review start date     & [29]Start date前一天 	\newline [30]与Start date相同  \newline  [31]Start date后一天 \\
  \hline
  Review finish date     & [32]与Review start date相同 	\newline [33]Review start date后一天 \newline [34]Finish date前一天 \newline [35]与Finish date相同  \newline  [36]Finish date后一天\\
  \hline
  \end{tabular}
\end{table}

表9是根据边界值分析设计的测试数据。

\begin{table}[!htbp]
  \caption{边界值分析测试数据}
  \centering
  \begin{tabular}{|p{0.35cm}|p{1.2cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.22cm}|p{0.9cm}|p{0.9cm}|p{0.9cm}|p{0.9cm}|p{0.22cm}|p{0.8cm}|}
  \hline
  \textbf{ID} & \textbf{类} & \multicolumn{11}{c|}{\textbf{输入参数}} & \textbf{预期}  \\ 
  \hline
17   & 27,30, 32,35 & c0  & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-03 & 2020-05-03 & 2020-05-03 & l0 & 成功   \\
  \hline
18   & 28,31, 33,36 & c0  & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04 & 2020-05-04 & 2020-05-05 & l0 & 成功   \\
  \hline
19   & 29           & c0  & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04 & 2020-05-02 & 2020-05-04 & l0 & 失败   \\
  \hline
20   & 34           & c0  & k0  & u0 & u1 & u2 & t0  & 2020-05-03 & 2020-05-04 & 2020-05-03 & 2020-05-03 & l0 & 失败   \\
  \hline
  \end{tabular}
\end{table}

\pagebreak

# 测试脚本实现及运行

## 脚本实现方式
脚本的实现主要参照https://my.oschina.net/hellotest/blog/531932 中，通过java反射机制，使用poi包操作excel关键字表，使用selenium的jar包进行自动化录制测试操作，以完成自动化测试框架。

### 出题测试脚本实现

#### 执行流程
  - 登陆
  - 导航到添加题目
  - 显示添加题目对话框
  - 选择章节
  - 选择知识点
  - 选择作者
  - 选择审核者
  - 选择质量审核
  - 选择种类
  - 填写开始日期
  - 填写结束日期
  - 填写审核开始日期
  - 填写审核结束日期
  - 选择语言
  - 保存问题

## 运行截图及说明
### 运行说明
\begin{figure}
  \centering
  \includegraphics[scale=0.7]{./screenshots/result.jpg}
  \caption{运行结果说明截图}\label{4}
\end{figure}
测试用例2和测试用例3保存题目预期结果应该是失败，但由于系统存在bug，并不会对章节和知识点的缺失进行检查，所以实际UI测试的结果并不是失败。

\pagebreak

### 运行过程截图

图6-图9展示的是测试运行过程中浏览器的情况。

\begin{figure}
  \centering
  \includegraphics[scale=0.1]{./screenshots/login.jpg}
  \caption{登录测试截图}\label{6}
\end{figure}

\begin{figure}
  \centering
  \includegraphics[scale=0.1]{./screenshots/CreateQ1.jpg}
  \caption{创建考题测试截图1}\label{7}
\end{figure}

\begin{figure}
  \centering
  \includegraphics[scale=0.1]{./screenshots/CreateQ2.jpg}
  \caption{创建考题测试截图2}\label{8}
\end{figure}

\begin{figure}
  \centering
  \includegraphics[scale=0.1]{./screenshots/CreateQ3.jpg}
  \caption{创建考题测试截图3}\label{9}
\end{figure}

\pagebreak

### 控制台截图

图10展示的为运行完测试之后的控制台日志输出情况

\begin{figure}
  \centering
  \includegraphics[scale=0.5]{./screenshots/console.jpg}
  \caption{控制台说明截图}\label{5}
\end{figure}



\pagebreak

# 参考文献 {-}
