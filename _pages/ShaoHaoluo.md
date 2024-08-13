---
permalink: /ShaoHaoluo
title: "邵浩洛"         # 有title选项会显示上面导航栏
author: ShaoHaoluo      # 在_data/authors中
excerpt: ""             # 摘要
author_profile: true    # 是否显示左侧个人介绍
layout: "default"
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}


<!-- 这是一个锚点, 用于在页面中定位 -->
<span class='anchor' id='about-me'></span>

我将硕士毕业于[华中科技大学](https://www.hust.edu.cn/) [机械科学与工程学院](https://mse.hust.edu.cn/) [智能制造装备与技术全国重点实验室](https://dmet.hust.edu.cn/)。
<!--, 我的导师是[李益群教授](https://mse.hust.edu.cn/info/1142/1360.htm) , 大导师是[熊有伦院士](https://www.hust.edu.cn/info/1133/9445.htm) -->
 <!-- <a href='https://scholar.google.com/citations?user=WMkMTb4AAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=引用"></a>。 -->

我的研究领域包括: 
- 视觉SLAM
- 多传感器融合
- 状态估计
- 机器人的定位与导航

我目前正在**求职中**, 欢迎随时通过 [shao-haoluo@foxmail.com]() 联系我


<span class='anchor' id='-xl'></span>

# 🎓 学历
- *2022.09 - 2025.06*, <a href="https://www.hust.edu.cn/"><img class="svg" src="/images/HUST_logo.svg" width="23pt"></a> 华中科技大学 机械科学与工程学院 智能制造装备与技术全国重点实验室, 推免硕士
- *2018.09 - 2022.06*, <a href="http://www.whut.edu.cn/"><img class="svg" src="/images/WHUT_logo.png" width="23pt"></a> 武汉理工大学 汽车工程学院, 本科
 
<span class='anchor' id='-kyjl'></span>

# 📝 科研经历

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Manuscript is complete, tutor reviewing</div><img src='images\toBeUpdate.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**轮腿混合式机器人状态估计与高程地图构建**

**项目简介:** 本项目依托课题组**自研**的四足轮腿机器人平台展开。

在触地检测方面, 因轮足平台难以安装力传感器检测触地情况, 利用KF融合步态相位、足端高度以及足端力, 实现机器人准确的触地检测。在Webots中测试触地准确率达到**99%**以上, 并能识别足端初始触地时回弹造成的**假触地**现象。

在状态估计方面, **创新性**地结合Invariant-EKF与S-MSCKF算法, 深度融合**视觉、IMU、腿部编码器以及轮式里程计**, 构造为VIS和LegIS两个子系统, 实现机器人在**足式、轮式、轮足混合运动模式**下、视觉或腿部编码器可缺失的**稳健状态估计**, 并构建**2.5D高程地图**。已经基于ROS和Webots平台完成仿真验证, 正在积极筹备进行实物实验。


**成果:**  `Haoluo Shao`, Kai Chen, Yiqun Li\*. VIEW: Visual Inertial Legged-Wheeled Odometry for Probabilistic Elevation Mapping. 
<!-- [[预览]]() -->

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">JFR (Minor Revision)</div><img src='images\ShaoHaoluo\火星无人机.gif' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**星表旋翼飞行机器人几何非线性控制与状态估计**

**项目简介:** 本项目聚焦强风、稀薄空气等极端环境, 设计几何自适应控制器来提高四旋翼飞行器的飞行安全性。

本人主要**负责状态估计**部分, 考虑到不变扩展卡尔曼滤波器（Invariant-EKF）具有误差演变独立于当前状态, 具有极好的鲁棒性和一致性的特点, 采用**Invariant-EKF融合视觉和IMU**数据, 并结合**VINS-Mono**的前端, 为飞行器提供精准且稳健的实时状态估计。

在Webots中的仿真结果显示, 四旋翼飞行器在高速、强风干扰下“8”字形飞行100m, 最大轨迹误差仅为**0.34m**。


**成果:** Siyuan Qiao, `Haoluo Shao`, Yiqun Li, Zhouping Yin\*. Geometric adaptive neural controller and optical flow based invariant extended Kalman filter for Mars quadrotor under disturbance. *Journal of Field Robotics*. (JCR:Q2; IF: 4.599)  
<!-- [[预览]]() -->

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images\ShaoHaoluo\环视拼接.gif' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**自动泊车场景中的AVM环视系统构建**

本项目针对自动泊车场景, 采用**4台森云**SG2-IMX390**环视相机**, 依次进行相机内参标定、去畸变、四路相机联合标定、投影变换、鸟瞰图拼接与融合等步骤, 成功构建出全景环视系统（AVM）。此外, 通过对鸟瞰图的细节优化, 极大程度上减轻了边缘伪影和色差。并先后在一台全尺寸四驱四轮转向金属3D打印电车底盘和一台**领克09**上进行了**实验验证**。

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images\ShaoHaoluo\第十六届智能车.gif' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**第十六届全国大学生智能车竞赛航天智慧物流组比赛**

主要负责阿克曼移动机器人的**感知与定位**。包括使用Cartographer算法进行**2D栅格地图**的构建、结合ROS中的**Navigation**框架实现机器人的精准定位与导航；使用**OpenCV**进行车道线的识别等功能。此外, 作为队长还协助硬件组队员完成Jetson Nano与**STM32通信算法**的编写, 全面把控比赛方案, 包括任务分配, 进度跟踪和难题探讨, 确保团队高效协作达成目标。

**成果:** 全国总决赛国家二等奖

</div>
</div>

<span class='anchor' id='-ryjx'></span>

# 🏅 荣誉奖项
- *2023.12* 获得 华中科技大学2023-2024学年 `校二等硕士学业奖学金` [[证书]](pdf\ShaoHaoluo\邵浩洛-华科2023-2024校二等奖学金.pdf)
- *2022.12* 获得 华中科技大学2022-2023学年 `校一等硕士学业奖学金` [[证书]](pdf\ShaoHaoluo\邵浩洛-华科2022-2023校一等奖学金.pdf)
- *2022.06* 获得 武汉理工大学2022届优秀毕业生
- *2021.09* 获得 第十六届全国大学生智能汽车竞赛 航天智慧物流组 `全国总决赛国家二等奖` [[证书]](pdf\ShaoHaoluo\邵浩洛-第十六届智能车竞赛-国赛.pdf)
- *2021.07* 获得 第十六届全国大学生智能汽车竞赛 航天智慧物流组 `南部赛区一等奖` [[证书]](pdf\ShaoHaoluo\邵浩洛-第十六届智能车竞赛-省赛.pdf)
- *2020.11* 获得 武汉理工大学2019-2020学年 `校一等学业奖学金` [[证书]](pdf\ShaoHaoluo\邵浩洛-武理2019-2020校一等奖学金.pdf)
- *2020.11* 获得 武汉理工大学2019-2020学年 `校三好学生` [[证书]](pdf\ShaoHaoluo\邵浩洛-武理2018-2019校三好学生.pdf)
- *2019.11* 获得 武汉理工大学2018-2019学年 `校三等学业奖学金` [[证书]](pdf\ShaoHaoluo\邵浩洛-武理2018-2019校三等奖学金.pdf)


<span class='anchor' id='-zyjn'></span>

# 🎯 专业技能
- **语言能力:** CET4、CET6
- **编程能力:** 熟练使用C/C++、Python、Matlab以及CMake和Git进行项目构建和版本管理
- **核心技能:** 
    1. 掌握视觉SLAM与多传感器融合领域核心算法（S-MSCKF、VINS-Mono）与理论基础；
    2. 熟练使用多种滤波算法如KF、EKF、ESKF、Invariant-EKF进行机器人状态估计；
    3. 了解相关优化算法, 能够使用多种优化库如Ceres、G2O构建优化问题；
    4. 具备坚实的机器人正运动学理论基础、熟练使用ROS/ROS2联合Webots/Gazebo进行机器人项目的构建与仿真；
    5. 拥有实际机器人的项目开发与落地经验
- **其他技能:** 熟练使用SolidWorks/Fusion 360/CATIA进行三维建模；使用STM32CubeMX与嘉立创EDA进行嵌入式开发；熟练使用Office系与PS、PR等软件



<span class='anchor' id='-sxjl'></span>

# 💻 实习经历
- *2019.07 - 2019.09*, 泛亚汽车技术中心有限公司, 上海 [[实习成果]](pdf\ShaoHaoluo\泛亚实习成果.pdf) [[实习证明]](pdf\ShaoHaoluo\泛亚实习证明.pdf)
