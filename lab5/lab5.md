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

本次作业为软件质量保障与测试课程的Lab5课程作业，需要我们以小组为单位撰写在线出题考试系统的IEEE829测试文档.

# 关键词 {-}

系统与软件工程; 系统与软件质量要求和评价; 测试文档

\normalsize

\newpage

\tableofcontents

\newpage

# 测试框架设计

## 黑盒测试框架图

## 黑盒测试框架图说明

# 关键字及测试数据设计

## 测试关键字

## 测试数据
<table>
    <tr>
        <td>ID</td>
        <td>覆盖的类</td>
        <td colspan="11">input</td>
        <td>预期输出</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>chapter</td>
        <td>knowledge point</td>
        <td>author</td>
        <td>reviewer</td>
        <td>QA</td>
        <td>type</td>
        <td>start date</td>
        <td>finish date</td>
        <td>review start date</td>
        <td>review finish date</td>
        <td>language</td>
        <td></td>
    </tr>
    <tr>
        <td>1</td>
        <td>1,3,5,7,10,13,15,17,19,22,25</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-03</td>
        <td>2020-05-03</td>
        <td>2020-05-03</td>
        <td>中文</td>
        <td>成功</td>
    </tr>
    <tr>
        <td>2</td>
        <td>1,3,5,7,10,13,15,17,19,22,25</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>jmeter002</td>
        <td>jmeter003</td>
        <td>jmeter004</td>
        <td>视频题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>英文</td>
        <td>成功</td>
    </tr>
    <tr>
        <td>3</td>
        <td>2</td>
        <td>空</td>
        <td>空</td>
        <td>jmeter002</td>
        <td>jmeter003</td>
        <td>jmeter004</td>
        <td>视频题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>英文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>4</td>
        <td>4</td>
        <td>1</td>
        <td>空</td>
        <td>jmeter002</td>
        <td>jmeter003</td>
        <td>jmeter004</td>
        <td>视频题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>英文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>5</td>
        <td>6</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>空</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-04-29</td>
        <td>2020-04-30</td>
        <td>2020-04-29</td>
        <td>2020-04-30</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>6</td>
        <td>9</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>空</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>7</td>
        <td>8</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>testadmin</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>8</td>
        <td>12</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>空</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>9</td>
        <td>11</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter022</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>10</td>
        <td>14</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>空</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>11</td>
        <td>16</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>空</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>12</td>
        <td>18</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>空</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>13</td>
        <td>20</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>空</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>14</td>
        <td>23</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>空</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>15</td>
        <td>26</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>空</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>16</td>
        <td>21</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-04-30</td>
        <td>2020-05-04</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
    <tr>
        <td>17</td>
        <td>24</td>
        <td>1</td>
        <td>1.2.1</td>
        <td>testadmin</td>
        <td>jmeter022</td>
        <td>jmeter023</td>
        <td>情景题</td>
        <td>2020-05-03</td>
        <td>2020-05-04</td>
        <td>2020-05-03</td>
        <td>2020-05-03</td>
        <td>中文</td>
        <td>失败</td>
    </tr>
</table>
<table>
<tr>
        <td>ID</td>
        <td>覆盖的类</td>
        <td colspan="11">input</td>
        <td>预期输出</td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td>chapter</td>
        <td>knowledge point</td>
        <td>author</td>
        <td>reviewer</td>
        <td>QA</td>
        <td>type</td>
        <td>start date</td>
        <td>finish date</td>
        <td>review start date</td>
        <td>review finish date</td>
        <td>language</td>
        <td></td>
    </tr>
    <tr>
            <td>18</td>
            <td>27,29,31</td>
            <td>1</td>
            <td>1.2.1</td>
            <td>testadmin</td>
            <td>jmeter022</td>
            <td>jmeter023</td>
            <td>情景题</td>
            <td>2020-05-03</td>
            <td>2020-05-03</td>
            <td>2020-05-03</td>
            <td>2020-05-03</td>
            <td>中文</td>
            <td>成功</td>
        </tr>
        <tr>
            <td>19</td>
            <td>28,30,32</td>
            <td>1</td>
            <td>1.2.1</td>
            <td>jmeter002</td>
            <td>jmeter003</td>
            <td>jmeter004</td>
            <td>视频题</td>
            <td>2020-05-03</td>
            <td>2020-05-04</td>
            <td>2020-05-04</td>
            <td>2020-05-05</td>
            <td>英文</td>
            <td>成功</td>
        </tr>
</table>

# 测试脚本实现及运行

## 脚本实现方式

## 运行截图及说明



\pagebreak

# 参考文献 {-}
