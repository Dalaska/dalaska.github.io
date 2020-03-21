# 开发笔记

*2020-03-29 CI continous integration*

改代码，要做监测，保证可以运行。
做代码检查，控制器不能有float64。
matlab不定义变量类型。代码生成会自动生成float 64
autosar规范.

/* Function for MATLAB Function: '<S23>/ListJoint' */
static void SortIgnoreZero(float32 x[52], uint8 id[52])

 id = SortIgnoreZero(x)
 生成的autosar代码中，后面输出
 找到对应simulink模块

*2020-03-19 游戏人工智能*

- 搜索技巧 -csdn.net

- automata自动机的话主要是编译器有用

- python game of life

- finite state machine
 [link](https://www.geeksforgeeks.org/conways-game-life-python-implementation/)
[link](https://www.infoq.cn/article/uzc9lOyLT9*36HvjMu4A)

*2020-03-18 软件*

- 将70个ECU减少到3个域控制器：
    1. 驾驶舱
    2. 自动驾驶和安全域
    3. 高性能的车身控制器。
- OTA方式进行更新，软硬分离
- AGL（汽车级linux）开发联盟，
- 过去软件集成委托给了一级供应商。黑盒。

*2020-03-16 python获得时间*

- 时间元组
- 获取格式化的时间
runoob.com/python/python-date-time.html
[link](runoob.com/python/python-date-time.html)

*2020-03-158 供应商入库步骤*

1. 技术认可：考察配套经验、供货能力、审厂，技术考察包含了各种特殊场景；
2. 报价招标：综合考虑价格、品质、技术的过程；
3. 定点：确认车厂与供应商之间的合作关系；
4. 发RFQ文件，制定产品开发进度：样件要提供A、B、C样件：
    - A样件称为功能样件，用于验证功能；
    - B样件用于环境测试。环境测试包括高低温、电磁兼容、盐雾、沙尘、振动等等。
    - C阶段是和量产一样的样件。

*2020-03-05 采购流程*

- 院技术委员会评审供应公司考察，入库招标，签合同，验收

*2020-02-22 汇报材料* 
- 总结做了贡献，经验，kpi
- 立项与中体规划的联系
- 问题汇报时把感知边界情况说清楚

*2020-02-11 软件需求* 
- 功能性，非功能性
- 软件系统 = 软件+硬件+使用环境：software intensive system = software + hardware + context 

*2020-01-28 debug 方法* 
- 从后往前想：reproduce, simplify, find origionsomething impossible ocurred,the only solid infomation is it did ocurredso we must think backward from the result

*2020-01-12价值创造* 
搬砖，技能，人脉，资源，聚焦，信息，圈子，投资

*2020-01-04 网关* 
- 网关不具体特指一类产品，只要连接两个不同的网络的设备都可以叫网关；

*2019-12-10 IP地址* 
- 路由A，地址192.168.1.1
- 子网掩码255.255.255.0
- port, 程序入口
- 典型计算机B，地址192.168.1.129

*2019-11-27 CAN总线* 
- 高低差分信号
- 终端电阻减少信号抖动
- 接口db9
- DBC， 信号矩阵 data base

*2019-11-02 Vector Canoe*  
- 用于刷标定了，观测量
- 可以看值，通信会有延时
- 才数据看报文用analyzer

*2019-10-12 autosar编程规范* 
- 代码生成
- a2l文件定义变量及标定观测量

*2019-09-17功能安全* 
- ASIL: B,D(D高), PM

*2019-08-10 接口*

- 感知的量里给控制bypasssensor can, body cansenor can直接通控制器，两路can都要进数采。




