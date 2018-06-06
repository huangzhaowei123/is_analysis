# 实验6：基于GitHub的实验管理平台的分析与设计
|学号|班级|姓名|
|:-------:|:-------------: | :----------:|
|201510414112|软件(本)15-1|黄照伟|

## 1. 概述
- 基于GitHub的实验管理平台的作用是在线管理实验成绩的Web应用系统。学生和老师的实验内容均存放在GitHUB
页面上。
- 学生的功能主要有：一是设置自己的GitHub用户名，二是查询自己的实验成绩。学生的GitHub用户名是公开的，但成绩不公开。
- 老师的功能主要有：一是批改每个学生的成绩，二是查看每个学生的成绩。
- 老师和学生都能通过本系统的链接方便地跳转到学生的每个GitHUB实验目录，以便批改实验或者查看实验情况。
- 实验成绩按数字分数计算，每项实验的满分为100分，最低为0分。
- 系统自动计算每个学生的所有实验的平均分。

## 2. 系统总体结构
![flow1](系统总体结构图.png)
[界面设计](https://huangzhaowei123.github.io/is_analysis/test6/ui1/总体.html)

## 3. 用例图设计 [源码](./src/用例图设计.puml)
![](用例源代码.png)

## 4. 类图设计 [源码](./src/class.puml)
![](类图.png)

## 5. 数据库设计
- ### [参见数据库设计](./数据库设计.md)

## 6. 用例及界面详细设计

- ### [“登录”用例](./yongli/登录.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/登录.html)
- ### [“退出”用例](./yongli/退出.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/退出.html)
- ### [“查看信息”用例](./yongli/查看信息.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/查看信息.html)
- ### [“修改信息”用例](./yongli/修改信息.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/修改信息.html)
- ### [“修改密码”用例](./yongli/修改密码.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/修改密码.html)
- ### [“发布课程”用例](./yongli/发布课程.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/发布课程.html)
- ### [“选课”用例](./yongli/选课.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/选课.html)
- ### [“发布实验”用例](./yongli/发布实验.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/发布实验.html)
- ### [“修改实验”用例](./yongli/修改实验.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/修改实验.html)
- ### [“评分”用例](./yongli/评分.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/评分.html)
- ### [“查看成绩”用例](./yongli/查看成绩.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/查看成绩.html)
- ### [“学生列表”用例](./yongli/学生列表.md),[界面](https://huangzhaowei123.github.io/is_analysis/test6/ui/学生列表.html)












