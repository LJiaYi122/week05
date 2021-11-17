# week05
 Typora
 - 课程：数字媒体技术
- 记录人：李嘉谊
- 时间：2021-11-10
- week11





## 本周任务：

>
>
>>
>>
>>>
>>>
>>>

```
<!DOCTYPE html>
<html>
<head>
   <meta charset="ut" f-8>
   <title>INFINI|映纷创意</title>
   <style>
    h1 {
        text-align: center;
        color:white;
        line-height: 75px;
        background: dimgrey;
        margin: 0;
      }
      
      
      </style>
</head>
<body>
    <div>
   <h1>INFINI</h1>
   </div>
   </body>
</html>


```

2.流程图

>
>
>2.1显示方向

- TB/TD（ top bottom/top down）表示从上到下

- BT（bottom top）表示从下到上

- RL（right left）表示从右到左

- LR（left right）表示从左到右

  

> 
>
> 2.2节点类型

>- 默认节点： A
>- 矩形节点： B[矩形]
>- 圆角矩形节点： C(圆角矩形)
>- 圆形节点： D((圆形))
>- 非对称节点： E>非对称]
>- 菱形节点： F{菱形}
>
>> 
>>
>> 2.3节点连线样式
>
>* 箭头连接 A1- ->B1
>* 开放连接 A2- - -B2
>* 虚线箭头连接 A3.->B3 或者 A3-.->B3
>* 虚线连接 A4.-B4 或者 A4-.-B4
>* 粗线箭头连接 A5==>B5
>* 粗线开放连接 A6===B6
>* 标签虚线箭头连接 A7-.text.->B7
>* 标签开放连接 A8- -text- - -B8
>  
>
>

 

```mermaid
graph TB
A[Apple]-->B{Boy}
A---C(Cat)
B.->D((Dog))
C==喵==>D
style A fill:#2fff,fill-opacity:0.1,stroke:#faa,stroke-width:3px
style D stroke:#000,stroke-width:8px

```

>
>
>3.甘特图
>
>
>
>>```mermaid
>>gantt
>>dateFormat YYYY-MM-DD
>>TITLE 产品计划表
>>section 阶段一
>>产品原型图:2021-11-11,2021-12-20
>>section 阶段二
>>产品交互界面:2021-12-22,2022-01-10
>>section 阶段三
>>前段开发:2022-11-21,2022-01-01
>>```
>
>>```mermaid
>>gantt
>>dateFormat YYYY-MM-DD
>>TITLE 产品计划表
>>section S1
>>T1: done,2014-01-01, 9d
>>section S2
>>T2: crit,active,2014-01-11, 9d
>>section S3
>>T3: 2014-01-02, 9d
>>```
>
>
>
>>```mermaid
>>gantt
>>dateformat HH:mm
>>Title 24-Hour Day
>>Whole day: done, 00:00, 1440m
>>睡觉:crit, sleep2,after 00:00, 450m <--! 00:00-7:30 -->
>>起床: get_up,after sleep2, 30m  <--! 7:30-8:00 -->
>>通勤(公交车)/早餐: commute1,after get_up, 60m <--! 8:00-9:00 -->
>>工作 :active,work1,after commute1,180m <--! 9:00-12:00 -->
>>吃饭 /休息 : rest,after work1,90m <--! 12:00-13:30 -->
>>工作 :active,work2,after rest,330m <--! 13:30-19:00 -->
>>通勤(步行) : commute2,after work2,90m  <--! 19:00-20:30 -->
>>学习:crit, study,after commute2,120m <--! 20:30-22:30 -->
>>准备睡觉: pre_sleep,after study,30m <--! 22:30-23:00 -->
>>睡觉 : crit,sleep1,after pre_sleep,60m <--! 23:00-00:00 -->
>>```
>
>>```mermaid
>>gantt         
>>       dateFormat  YYYY-MM-DD   
>>       title 使用mermaid语言定制甘特图
>
>>       section 任务1
>>       已完成的任务           :done,    des1, 2014-01-06,2014-01-08
>>       正在进行的任务               :active,  des2, 2014-01-09, 3d
>>       待完成任务1               :         des3, after des2, 5d
>>       待完成任务2              :         des4, after des3, 5d
>
>>       section 关键任务
>>       已完成的关键任务 :   crit, done, 2014-01-06,24h
>>       已完成的关键任务2         :crit, done, after des1, 2d
>>       正在进行的关键任务             :crit, active, 3d
>>       待完成的关键任务        :crit, 5d
>>       待完成任务           :2d
>>       待完成任务2                      :1d
>
>>       section 文档编写
>>       描述甘特图语法               :active, a1, after des1, 3d
>>       完成甘特图实例1      :after a1  , 20h
>>       完成甘特图实例2    :doc1, after a1  , 48h
>
>>       ```
>
>
>
>>>4.数学公式
>
>
>
>
>
>
>
>作业：
>
>### 实践1：
>
>```mermaid
>graph LR
>A[TREE]==>B{融合新闻学}
>A[TREE]==>C{网页设计与制作}
>A[TREE]==>D{数字媒体技术}
>B{融合新闻学}-->E[新闻传播与研究方法]
>B{融合新闻学}-->F[数字多媒体作品创造]
>C{网页设计与制作}-->G[电子商务基础与应用]
>C{网页设计与制作}.->Q[H5互动技术与应用]
>D{数字媒体技术}-->H[Python语言]
>E[新闻传播与研究方法]-->I[大数据]
>G[电子商务基础与应用]-->I[大数据]
>H[Python语言]-->J[API,机器学习与人工智能]
>H[Python语言]-->K[网络舆情监测与研判]
>I[大数据].->L[交互设计]
>I[大数据].->M[网站运营与管理]
>I[大数据].->N[新媒体产品设计与项目管理]
>I[大数据].->O[信息可视化]
>H[Python语言].->P[Web数据挖掘]
>L[交互设计].->R[用户研究]
>M[网站运营与管理].->S[产品经理能力培养]
>N[新媒体产品设计与项目管理].->S[产品经理能力培养]
>S[产品经理能力培养].->T[写作能力]
>P[Web数据挖掘].->U[Python数据分析]
>Q[H5互动技术与应用].->V[移动互联网开发]
>Q[H5互动技术与应用].->W[前端开发框架]
>W[前端开发框架].->X[新媒体数据分析与应用]
>U[Python数据分析].->X[新媒体数据分析与应用]
>V[移动互联网开发].->Y[交互设计与前端设计]
>V[移动互联网开发].->X[新媒体数据分析与应用]
>U[Python数据分析].->Z[用户研究与数据分析]
>X[新媒体数据分析与应用].->T[写作能力]
>T[写作能力].->a[文献总数与写作]
>T[写作能力].->b[实践社群与自我策划]
>R[用户研究].->c[产品策划/运营]
>R[用户研究].->d[社会数据科学]
>Y[交互设计与前端设计].->e[微信小程序开发与运营]
>Z[用户研究与数据分析].->f[数据产品经理/平台型产品经理/产品体验设计]
>style A fill:#2fff,fill-opacity:0.1,stroke:#faa,stroke-width:8px
>style B fill:#2fff,fill-opacity:0.1,stroke:#faa,stroke-width:6px
>style C fill:#2fff,fill-opacity:0.1,stroke:#faa,stroke-width:6px
>style D fill:#2fff,fill-opacity:0.1,stroke:#faa,stroke-width:6px
>
>
>
>
>
>
>```
>
>
>
>
>
>
>
>





