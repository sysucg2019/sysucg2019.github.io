---
layout: page
title: Assignment
permalink: /assignment/
---

## 作业说明
-  评分细则：完成度及正确性(50%) + 编程规范(20%) + 书面报告(30%)。编程规范见<a href="https://github.com/sysucg2019/sysucg2019.github.io/raw/master/slides/CG-01-Introduction.pdf">CG-01-Introduction.pdf</a>。
-  允许讨论代码，但作业代码和报告的编写和提交应独立完成。严禁任何形式的抄袭，否则将无法通过本课程。
-  缓交作业：迟交作业不得分，但同学们可在作业截止前向TA：liuj285@mail2.sysu.edu.cn提出使用3天的slip days(包括周末节假日，且不适用于期末现场报告)，并在slip days结束前补交作业。

## 作业列表
### 期末大作业  (截止时间：2019.12.28 23:59)
### 自选题目
每个小组自行决定期末大作业选题，选题可以是实现复杂场景、动画短片、小游戏、可视化或其他。  
（注意：期末大作业不支持缓交作业，截止时间内未提交即记为0分）

#### 期末大作业提交说明
- 提交的压缩包需要包含：代码、报告和展示视频。
- 代码：  
  必要的.pro/.h/.cpp/shader文件以及支撑项目运行的图片/模型资源；
- 报告：小组报告和个人报告；  
  小组报告需要包括但不限于选题背景、小组分工、技术要点、实现效果等方面的内容；  
  个人报告需要包括但不限于个人所负责部分的详细描述、遇到的问题及解决方法、总结和感想等方面的内容。
- 视频：时长为3分钟的视频文件，用于12月30日的课堂展示（不再需要提交ppt）；  
  视频内容只需要包括技术要点和实现效果两方面，这两部分内容可以有所侧重：实现过程比较复杂的可以侧重讲技术，效果设计比较复杂的可以侧重讲效果，至于侧重哪一方面由同学们自行决定。
  
#### 期末大作业提交格式
请将期末大作业发送至作业邮箱sysucg2019@163.com，邮件标题应与附件(.zip文件)名一致。压缩文件夹应有如下的组织形式：

组长学号\_组长姓名\_题目\_版本#/  
　　|— src/  
　　　　|- .pro/.h/.cpp/.png/.obj等  
　　|— doc/    
　　　　|- 题目_小组报告.pdf  
　　　　|- 成员1学号\_成员1姓名\_个人报告.pdf  
　　　　|- 成员2学号\_成员2姓名\_个人报告.pdf  
　　　　|- ...  
　　|- vid/  
　　　　|- 题目.avi/.mp4/...  

----

### 作业3 （2019.12.09 ~ ~~2020.01.04 23:59~~ 2020.01.08 23:59）[Assignment3.pdf](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/Assignment3.pdf)  [作业3模板-CGTemplate3.zip](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/CGTemplate3.zip)
### GLSL入门
参考作业文档，编写GLSL着色器程序，绘制沿固定轨道运动的小球。

#### 3.1 使用GL_POINTS绘制沿固定轨道运动的小球
-  每个glVertex调用指明一个小球的球心位置。
-  小球大小根据离观察点距离变化（近大远小）。
-  使用Phong Shading。
-  参考[Assignment3.pdf第9页](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/Assignment3.pdf)的Vertex Shader和Fragment Shader。 

#### 3.2 （选做）使用VBO进行绘制
-  参考[Assignment3.pdf第10页](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/Assignment3.pdf) 的绘制函数。

#### 3.3 其他注意事项
-  编程规范：编程规范包括规范的函数及变量命名、函数的注释说明及其他重要语句的注释说明，编程规范见<a href="https://github.com/sysucg2019/sysucg2019.github.io/raw/master/slides/CG-01-Introduction.pdf">CG-01-Introduction.pdf</a>。
-  报告内容：在报告中写下主要算法，详细说明实现过程，并附上每个步骤的运行结果截图；总结实现过程遇到的困难及相应的解决方法。
-  作业提交：不规范的作业附件命名可能影响作业的提交，请务必严格按照提交格式命名。

----

### 作业2 （2019.11.18 ~ 2019.12.8 23:59）[Assignment2.pdf](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/Assignment2.pdf)  [作业2模板-CGTemplate2.zip](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/CGTemplate2.zip)
### 绘制一个沿固定线路运动的机器人

~~绘制过程中使用的平移、旋转函数请使用你在作业1中实现的函数，或另行实现，不能使用`glTranslate()`, `glRotate()`, `glMultMatrix()`等函数。~~
绘制过程中的平移、旋转可以使用`glTranslate()`、`glRotate()`, `glMultMatrix()`等函数。

#### 2.1 绘制你的机器人
-  使用GL_POINTS, GL_TRIANGLES, GL_QUADS, GL_POLYGON等基本图元，结合平移、旋转函数绘制一个机器人。
-  机器人应该有头、躯干、四肢等基本部分。

#### 2.2 绘制机器人的运动线路
-  使用平移、旋转函数使你的机器人沿固定线路运动。
-  线路可以是圆或任意其他闭合路径。

#### 2.3 绘制机器人的动作
-  使用平移、旋转函数绘制机器人的动作。
-  机器人在运动过程中应具有摆臂及抬腿两个基本动作。

#### 2.4 （选做）加分项-模型载入
-  使用mesh模型（如obj文件）载入机器人模型。
-  或载入其他mesh模型围绕机器人运动。

#### 2.5 其他注意事项
-  编程规范：编程规范包括规范的函数及变量命名、函数的注释说明及其他重要语句的注释说明，编程规范见<a href="https://github.com/sysucg2019/sysucg2019.github.io/raw/master/slides/CG-01-Introduction.pdf">CG-01-Introduction.pdf</a>。
-  报告内容：在报告中写下主要算法，详细说明实现过程，并附上每个步骤的运行结果截图；总结实现过程遇到的困难及相应的解决方法。
-  作业提交：不规范的作业附件命名可能影响作业的提交，请务必严格按照提交格式命名。

----

### 作业1 （2019.10.12 ~ 2019.11.3 23:59）[Assignment1.pdf](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/Assignment1.pdf)  [作业1模板-CGTemplate.zip](https://github.com/sysucg2019/sysucg2019.github.io/raw/master/CGTemplate.zip)
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
- Qt 5.13.0 下载：[https://download.qt.io/official_releases/qt/5.13/5.13.0/](https://download.qt.io/official_releases/qt/5.13/5.13.0/)  
- Qt镜像列表（exe for windows）：[https://download.qt.io/archive/qt/5.13/5.13.0/qt-opensource-windows-x86-5.13.0.exe.mirrorlist](https://download.qt.io/archive/qt/5.13/5.13.0/qt-opensource-windows-x86-5.13.0.exe.mirrorlist)  
- Qt .pro项目文件变量说明：[https://doc.qt.io/qt-5/qmake-variable-reference.html](https://doc.qt.io/qt-5/qmake-variable-reference.html)

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
