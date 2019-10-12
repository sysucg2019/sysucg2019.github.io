---
layout: page
title: Assignment
permalink: /assignment/
---

## 作业说明
-  每次作业统一使用QT模板<a href="https://github.com/sysucg2019/sysucg2019.github.io/raw/master/CGTemplate.zip">CGTemplate</a>。
-  评分细则：完成度及正确性(50%) + 编程规范(20%) + 书面报告(30%)。编程规范见<a href="https://github.com/sysucg2019/sysucg2019.github.io/raw/master/slides/CG-01-Introduction.pdf">CG-01-Introduction.pdf</a>。
-  允许讨论代码，但作业代码和报告的编写和提交应独立完成。严禁任何形式的抄袭，否则将无法通过本课程。
-  缓交作业：迟交作业不得分，但同学们可在作业截止前向TA：liuj285@mail2.sysu.edu.cn提出使用3天的slip days(包括周末节假日，且不适用于期末现场报告)，并在slip days结束前补交作业。

## 作业列表
### 作业1 （2019.10.12 ~ 2019.11.3 23:59）[Assignment1.pdf](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/Assignment1.pdf)
### 使用自行编写的代码重现场景

在作业模板中的`scene_0()`函数使用了`OpenGL`函数（如，`glBegin(GL_LINE_STRIP)`，`glTranslatef()`及`glRotatef()`等）绘制一个三角形及一个四边形的场景。同学们需要在`不使用`以上函数的情况下重现同样场景（在模板中的`scene_1()`函数汇总实现）。

#### 1.1 实现平移Translation及旋转Rotation变换
实现平移及旋转函数，计算点经过平移、旋转等变换后，于屏幕中所处的位置。  
-  不能使用`glTranslate()`, `glRotate()`, `glMultMatrix()`等函数。  
-  可选：通过矩阵乘法及四元数两种方式实现旋转。  

#### 1.2 实现直线绘制算法
使用`OpenGL`实现你的直线光栅化算法。  
-  输入：两个二维平面上的点（由1.1中计算得到）。  
-  输出：在屏幕上输出一条直线。  
-  只能使用整数运算，并且只能使用`GL_POINTS`作为基本元素。  
-  可选：使用抗锯齿算法或机制对绘制直线进行平滑。

#### 1.3 其他注意事项
- 在报告中写下主要算法，说明多个变换之间的顺序关系对结果的影响，并附上运行结果截图。  
- `scene_1()` 函数中已经提供一个基本模板，用于对每个坐标对应的像素点着色。  
- `scene_0()` 及 `scene_1()` 的绘制可通过键盘的"0","1"按键进行切换。  
- 在窗口resize过程中，需要保持 `scene_1()` 绘制结果与 `scene_0()` 一致。  

#### 1.4 Qt相关链接
Qt 5.13.0 下载：https://download.qt.io/official_releases/qt/5.13/5.13.0/  
Qt镜像列表（exe for windows）：https://download.qt.io/archive/qt/5.13/5.13.0/qt-opensource-windows-x86-5.13.0.exe.mirrorlist  
Qt .pro项目文件变量说明：https://doc.qt.io/qt-5/qmake-variable-reference.html

## 提交格式
#### 请将你的作业发送至作业邮箱sysucg2019@163.com，邮件标题应与你的附件(.zip文件)名一致。你的压缩文件夹应有如下的组织形式：

学号\_姓名\_作业#\_版本#/  
　　|— src/  
　　|— doc/  
- 学号：你的8位数学号。
- 姓名：你的中文姓名。
- 作业#: 表明第几次作业。
- 版本#：表明你提交的作业版本，从版本0开始。只有最后一版的作业会被评分。
- src/：包含你的项目代码文件(.pro/.h/.cpp文件)。
- doc/：包含你的作业报告(report.pdf文件)。

例如，学号为12345678的艾伦同学首次提交作业1，那么他提交的附件应为：  
　　12345678\_艾伦\_作业1\_版本0.zip  
  　　　　|— 12345678\_艾伦\_作业1\_版本0/  
  　　　　  　　｜—src/  
  　　　　  　　｜—doc/
