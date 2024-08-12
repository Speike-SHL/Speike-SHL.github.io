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


<!-- 这是一个锚点，用于在页面中定位 -->
<span class='anchor' id='about-me'></span>

我将硕士毕业于[华中科技大学](https://www.hust.edu.cn/) [机械科学与工程学院](https://mse.hust.edu.cn/) [智能制造装备与技术全国重点实验室](https://dmet.hust.edu.cn/)，我的导师是[李益群教授](https://mse.hust.edu.cn/info/1142/1360.htm)。
<!-- ，大导师是[熊有伦院士](https://www.hust.edu.cn/info/1133/9445.htm) -->
 <!-- <a href='https://scholar.google.com/citations?user=WMkMTb4AAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=引用"></a>。 -->

我的研究领域包括: 
- 视觉SLAM
- 多传感器融合
- 状态估计
- 机器人的定位与导航

我目前正在**求职中**，欢迎随时通过 [shao-haoluo@foxmail.com]() 联系我


<span class='anchor' id='-xl'></span>

# 🎓 学历
- *2022.09 - 2025.06*, <a href="https://www.hust.edu.cn/"><img class="svg" src="/images/HUST_logo.svg" width="23pt"></a> 华中科技大学 机械科学与工程学院 智能制造装备与技术全国重点实验室, 推免硕士
- *2018.09 - 2022.06*, <a href="http://www.whut.edu.cn/"><img class="svg" src="/images/WHUT_logo.png" width="23pt"></a> 武汉理工大学 汽车工程学院, 本科
 
<span class='anchor' id='-kyjl'></span>

# 📝 科研经历

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Manuscript is complete, tutor reviewing</div><img src='images\500x300.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**轮腿混合式机器人状态估计与高程地图构建**

**成果:**  `Haoluo Shao`, Kai Chen, Yiqun Li\*. VIEW: Visual Inertial Legged-Wheeled Odometry for Probabilistic Elevation Mapping. 
<!-- [[预览]]() -->

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">JFR (Minor Revision)</div><img src='images\ShaoHaoluo\火星无人机.gif' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**星表旋翼飞行机器人几何非线性控制与状态估计**

**成果:** Siyuan Qiao, `Haoluo Shao`, Yiqun Li, Zhouping Yin\*. Geometric adaptive neural controller and optical flow based invariant extended Kalman filter for Mars quadrotor under disturbance. *Journal of Field Robotics*. (JCR:Q2; IF: 4.599)  
<!-- [[预览]]() -->

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images\ShaoHaoluo\环视拼接.gif' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**自动泊车场景中的AVM环视系统构建**

本项目针对自动泊车场景，采用**4台森云**SG2-IMX390**环视相机**，依次进行相机内参标定、去畸变、四路相机联合标定、投影变换、鸟瞰图拼接与融合等步骤，成功构建出全景环视系统（AVM）。此外，通过对鸟瞰图的细节优化，极大程度上减轻了边缘伪影和色差。并先后在一台全尺寸四驱四轮转向金属3D打印电车底盘和一台**领克09**上进行了**实验验证**。

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><img src='images\ShaoHaoluo\第十六届智能车.gif' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**第十六届全国大学生智能车竞赛航天智慧物流组比赛**

主要负责阿克曼移动机器人的**感知与定位**。包括使用Cartographer算法进行**2D栅格地图**的构建、结合ROS中的**Navigation**框架实现机器人的精准定位与导航；使用**OpenCV**进行车道线的识别等功能。此外，作为队长还协助硬件组队员完成Jetson Nano与**STM32通信算法**的编写，全面把控比赛方案，包括任务分配，进度跟踪和难题探讨，确保团队高效协作达成目标。

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



<span class='anchor' id='-sxjl'></span>

# 💻 实习经历
- *2019.07 - 2019.09*, 泛亚汽车技术中心有限公司, 上海 [[实习成果]](pdf\ShaoHaoluo\泛亚实习成果.pdf) [[实习证明]](pdf\ShaoHaoluo\泛亚实习证明.pdf)
