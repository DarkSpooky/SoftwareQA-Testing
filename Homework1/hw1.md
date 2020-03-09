---
title: \vspace{2in} 出题系统测试计划报告
subtitle: "软件质量保障与测试课程第一次课程作业（第9组）"
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

date: "2020年3月7日"
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
\textbf{出题系统测试计划报告}
\end{center}

\large
\begin{center}
\textbf{\emph{软件质量保障与测试课程第一次课程作业}}
\end{center}

# 摘要 {-}

本次作业为软件质量保障与测试课程的第一次课程作业，需要我们以小组为单位阅读、理解出题系统初始需求文档，进行小组讨论，结合软件质量相关属性，列举测试计划，即准备对这个系统的哪些方面进行测试，并最终撰写计划报告。

此测试计划报告为对本次作业提交的测试计划。在分析测试计划时，我们以国际标准化组织（International Organization for Standardization）在2014年修订的标准ISO/IEC 25000:2014（也被称作SQuaRE，System and Software Quality Requirements and Evaluation）为基本依据，同时参照中华人民共和国国家质量监督检验检疫总局和中国国家标准化管理委员会在2016年发布的GB/T 25000-2016（系统与软件工程系统与软件质量要求和评价，SQuaRE）为具体准则，以老师和助教所提供的出题系统初始需求文档为测试完整度衡量标准与目标，分析并撰写了本次测试计划报告。

本次测试计划报告仅作为一个初步的测试计划，其测试对象的出题系统的完整测试计划报告将会在接下来的作业中进一步地完善、整理，并作为本课程中后期阶段进行具体测试时的依据。


# 关键词 {-}

系统与软件工程; 系统与软件质量要求和评价; 测试计划报告

\normalsize

\newpage

\tableofcontents

\newpage


# 功能性测试

## 登录及个人信息测试

- 用户输入正确用户名，密码登录测试
- 用户输入错误用户名，密码登录测试
- 修改个人信息测试

## 步骤一:建立一个新项目

- 对创建新的出题系统、确定主持人进行测试
- 对为项目定义唯一项目名这一功能进行测试
- 对主持人进行的项目规划和运行进行测试
- 对创建新考题进行测试
- 对"开始"状态设置以及编写考题框架进行测试
- 对确定出题相关属性进行测试
- 对作者编写考题属性进行测试
- 对主持人设置考题状态"开始"权限进行测试
- 为考题添加单个作者，评审员，质管员进行测试
- 为考题添加多个作者，评审员，质管员进行测试
- 对作者和评审员之间读取互相信息权限进行测试
- 对作者和评审员的唯一标识符进行测试

## 步骤二:开始启动项目(状态:开始;角色:主持人)

- 对主持人能够在状态为“开始”的考题内分配知识点、作者和评审员进行测试

- 对主持人能够为状态为“开始”的考题设定编写考题与评审考题的时间限期进行测试

- 对系统会对超出限期的任务报警进行测试

- 对主持人能对超出限期的任务提出警告或调整时间限期进行测试
- 对主持人能将分配了知识点、作者、评审员和限期的题目状态改为“编写”，状态改变后系统能给对应作者发送邮件的测试
- 对未完成分配任务的题目状态不能改为“编写”的测试
- 对主持人能够批量将完成分配的题目状态改为“编写”，系统会给对应作者发送邮件的测试
- 对除主持人外，系统管理员、作者、评审员没有修改题目状态的权限的测试

## 步骤三:编写考题(状态:编写;角色:作者) 

- 对作者能够看到应当由他编写的考题的相关信息进行测试
- 对作者能够编写普通考题、给出标准答案并设置相关属性进行测试
- 对作者能够编写带有表格的题目、给出标准答案并设置相关属性进行测试
- 对作者能够编写带有图形的题目、给出标准答案并设置相关属性进行测试
- 对未完成编写（如题干为空等情况），未给出标准答案或未完成相关属性设定的题目，作者不能修改其状态为“评审”的测试
- 对作者能够将编写完成、给出标准答案并设置相关属性的题目状态改为“评审”，系统会给评审员发出邮件的测试
- 对编写过程中主持人不能修改和操作的权限进行测试
- 对普通考题能以XML，Excel的形式导入出题系统的测试
- 对带有表格的题目能以XML，Excel的形式导入出题系统的测试
- 对带有图形的题目能以XML，Excel的形式导入出题系统的测试


## 步骤四:评审考题(状态:评审;角色:评审员)

- 对评审员能够查看需要自己评审的题目的权限进行测试
- 对评审员能够查看需要再次评审的题目的权限进行测试
- 对评审员设置为"可接受"评审结果与"再审"状态的考题的流程进行测试
- 对评审员设置为"需修改"评审结果与"修改"状态的考题的流程进行测试
- 对评审员设置为"被拒绝"评审结果与"再审"状态的考题的流程进行测试
- 对评审过程中主持人没有修改和操作的权限进行测试

## 步骤五:再审考题(状态:再审;角色:质管员)

- 对质管员将"可接受"评审结果的题目设置为"发布"状态的流程进行测试
- 对质管员将"被拒绝"评审结果的题目设置为"作废"状态的流程进行测试
- 对质管员将"可接受"评审结果的题目设置为"修改"状态的流程进行测试
- 对质管员阅读所有处于"再审"状态的考题的权限进行测试
- 对质管员给所有处于"再审"状态的考题编写评审意见和建议的权限进行测试
- 对质管员给所有处于"再审"状态的考题进行变更状态的权限进行测试
- 对再审过程中主持人没有修改和操作的权限进行测试

## 步骤六:修改考题(状态:修改;角色:作者)

- 对作者可以阅读到所有与本作者有关的处于“修改”状态的考题这一权限进行测试
- 对作者可以修改考题信息进行测试
- 对作者可以将考题由“修改”状态改为“评审”状态这一权限进行测试
- 对考题改为“评审”状态后,系统自动给评审员发送提示电邮这一功能进行测试
- 对修改过程中主持人只有阅读权限,没有修改和操作的权限进行测试


## 步骤七:发布考题(状态:发布;角色:主持人) 

- 对主持人可以接受处于发布状态的考题进行测试
- 对主持人可以正常导出考题进行测试
- 对导出时选择导出考题的最终版本,不带上历史数据及无关的考题属性这一情况进行测试
- 对导出时选择导出考题的所有完整内容这一情况进行测试
- 进行普通考题导出为XML，Excel格式分别测试
- 进行带表格或图片的考题导出为XML，Excel测试
- 对题库系统管理员可以正常导入由主持人导出的考题进行测试(Excel和XML格式的考题)

## 步骤八:作废考题(状态:作废;角色:主持人)

- 对主持人废除考题的操作进行测试
- 对主持人再次安排替补的考题这一流程进行测试
- 对主持人阅读处于作废状态的考题这一权限进行测试
- 对主持人没有修改和操作的权限进行测试


## 整体流程控制

- 在重新定义模型的功能实装后定义新的合法状态模型进行测试

- 测试用户作出更改后系统所产生的记录信息可否追踪

# 非功能性测试

## 性能效率

- 测试导入题库不同大小的数据耗时
- 测试从题库导出不同大小的数据耗时

## 兼容性

- 针对不同浏览器做测试
- 针对不同用户端，不同窗口大小（如不同款式手机，平板电脑）的适配性做测试

## 易用性

- 输入不符合规定格式的用户名/密码
- 对于合法值有限的下拉框，尝试抓包修改值为非法值之后发送
- 对于日期等格式固定的参数，尝试修改为不符合格式后发送
- 把不能为null的值修改为空后发送
- 测试搜索不存在的条目
- 测试不合法数据导入题库管理系统
- 测试上传图片的大小和类型限制
- 测试无效URL的图片
- 上传图片时测试上传非图片的文件
- 测试支持的图片文件大小
- 测试支持的表格行列极限大小
- 测试添加作者，评审，质管为不存在用户
- 定义新的不合法状态模型（如含有null字段，无意义权限等）进行测试

## 可靠性

- 测试编辑到一半断电/掉线后的数据恢复能力
- 测试各角色对数据修改后未保存的后果
- 测试各角色对数据修改后能否撤销
- 测试用户作出更改后系统所产生的记录信息可否追踪
- 测试同一数据重复导入题库管理系统
- 测试未登录角色导入数据
- 测试未拥有权限的角色导入数据
- 在尚未有发布考题的时候进行导出测试
- 测试无权限的角色能否导出数据
- 测试未登录能否导出数据
- 测试多个用户在线且同时对同一考题进行更改对考题产生的作用
- 测试在用户更改某个考题时，另一用户删除该考题的后果
- 测试多位教师同时上传某一相同考题的后果
- 测试多位管理员同时导入同一数据的后果
- 测试多位管理员同时删除同一考题的后果 
- 测试对网站进行DDoS攻击

## 信息安全性

- 测试在各个环节通过SQL注入/XSS注入盗取数据/cookie
- 测试通过.DS_Store，web.rar，.git等常见后缀是否能够泄露源码
- 测试网页前端注释中是否有敏感数据泄露
- 测试通过URL的越权访问
- 测试将含有XXE注入的XML数据导入题库管理系统
- 上传图片时测试上传嵌入webshell的文件
- 在登录界面用户名，密码或题目题干等处进行SQL注入，webshell插入，XSS注入

## 维护性

- 在得到网页的源代码之后对源代码进行分析，是否满足模块化、文档清晰、代码结构有组织、代码风格统一等维护必须要素

## 可移植性

- 在Mac，Windows，Linux等各个平台上独立测试


\pagebreak

# 参考文献 {-}
