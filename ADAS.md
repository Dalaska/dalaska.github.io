ADASPerception
# L2传感器融合架构方法和常见问题
L2传感器融合架构分为
1.雷达聚类，匹配，追踪，管理
fig
##1.雷达 聚类 
雷达之前步骤, 处理硬件实现
将target目标转化为 object list.
回波，噪音其实是，隧道，旁边有道路的情况下
与其说是噪音，
目标过滤，静止目标，对象面车
基于距离，基于密度
eclidean clustering
http://www.pointclouds.org/documentation/tutorials/cluster_extraction.php
https://github.com/cse481sp17/cse481c/wiki/Lab-32:-Euclidean-clustering
dbscan
https://www.mathworks.com/matlabcentral/fileexchange/52905-dbscan-clustering-algorithm
##2.匹配
gating
gating 方法，
1. 每个track gate，会出现多对一的情况
2. linear assignment
jpda，gnn,马氏距离,卡方分布
joint covance
https://www.mathworks.com/matlabcentral/fileexchange/6543-functions-for-the-rectangular-assignment-problem
 pda， mht, multi hypothesis tracking
https://www.mathworks.com/help/fusion/examples/track-simulated-vehicles-using-gnn-and-jpda-trackers-in-simulink.html
http://www.cse.psu.edu/~rtc12/CSE598C/datassocPart1.pdf
Note: if assignment was always unambiguous, we could turn MTT into independent single-target tracking problems. However, when the association is ambiguous (multiple observations in one gating region; common observations in multiple gating regions ), then the assignment decisions become coupled and much harder to solve.
匹配讲义http://www.cse.psu.edu/~rtc12/CSE598C/datassocPart2.pdf


### 3 追踪
卡尔曼kf 相机
ekf, 雷达， 
1.雷达的观测矩阵
1.相机激光雷达的观测矩阵
（ ufk, pf）
管理，航迹合并，丢失几帧删除

4 难点
1. 目标个旁边障碍物区分，速度最为gate
2. 并行目标区分
3. 遮挡障碍物，雷达可以穿透
4. 误报警，单雷达存在误报警，相机确认
5. 漏报警，雨天相机漏报，
误报，漏报存在权衡
