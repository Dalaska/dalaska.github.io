# ADAS感知架构

自动驾驶的商业化还有些遥远，而高级辅助驾驶（ADAS）已经装备量产。甚至8万元的车型都配备了自适应巡航（ACC）,自动辅助刹车(AEB)功能。
环境感知是决策和控制的前提。下面对ADAS中感知的架构和模块做一个介绍。

## 1.传感器融合架构分为
因为不同的传感器有各自的优缺点，所以需要将传感器融合来扬长避短。
在ADAS中最普遍的传感器是摄像头与毫米波雷达的。
摄像头优势目标识别，对目标分类车辆，自行车，行人等目标。劣势距离信息不是直接测量得到的，不准确。特别是在恶劣环境和光照不足的环境下。
毫米波雷达优势直接测量目标的位置和速度。并且受到天气及环境的影响小。
劣势在于雷达的信号较为稀疏，不便通过雷达进行目标识别。这些性质正好与摄像头形成互补。
信息融合又可分为目标级融合和信号级融合。
目标级融合，每个传感器先各自处理原始信号生成目标。在目标的基础上进行融合。优点是对控制器的算力和通信传输要求低。缺点是传感器在独立处理信号时会有信息丢失。
数据级融合，在原始数据级就进行融合优点是信息丢失少，精度高，缺点是对控制器的算力和通信传输要求高。
在设计架构时需要找到精度和算力分布的平衡点。

一个摄像头和雷达目标级的传感器融合。雷达输出target信号，摄像头为类似mobileye的智能摄像头输出track信号
架构分为数据有效性验证，时间补偿，雷达聚类，目标匹配，新目标生成，航迹追踪，目标管理等子模块
下面将对雷达聚类，目标匹配，航迹追踪进行介绍

## 1.雷达聚类 
毫米波雷达原理
雷达之前步骤, 处理硬件实现
一般输出的信号，target，object，track
将target目标转化为 object list.


回波，噪音其实是，隧道，旁边有道路的情况下
与其说是噪音，


目标过滤，静止目标，对象面车
基于距离，基于密度

eclidean clustering
介绍

dbscan
介绍

## 2.目标匹配
目标匹配的目的是传感器与航机匹配。
gating，
gating 方法，
1. 每个track gate，会出现多对一的情况

一配多，一一匹配，多配一

2. linear assignment
jpda，gnn,马氏距离,卡方分布
joint covance
 pda， mht, multi hypothesis tracking
Note: if assignment was always unambiguous, we could turn MTT into independent single-target tracking problems. However, when the association is ambiguous (multiple observations in one gating region; common observations in multiple gating regions ), then the assignment decisions become coupled and much harder to solve.
匹配讲义

## 3. 航迹追踪
卡尔曼kf 相机
ekf, 雷达， 
1.雷达的观测矩阵
1.相机激光雷达的观测矩阵
（如果用到更复杂的模型 ufk
 如果用到多轨迹假设 pf）
管理，航迹合并，丢失几帧删除

## 4. 难点
1. 目标个旁边障碍物区分，速度最为gate
2. 并行目标区分
3. 遮挡障碍物，雷达可以穿透
4. 误报警，单雷达存在误报警，相机确认
5. 漏报警，雨天相机漏报，
误报，漏报存在权衡
