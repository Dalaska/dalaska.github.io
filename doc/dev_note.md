# 开发笔记

*2020-03-22*
- [动态类型](https://www.zhihu.com/question/30072490)

- [汽车软件](https://zhuanlan.zhihu.com/c_1039090669892902912)


- 一流供应商从来没有一个项目完全遵循了aSPICE和ISO26262 part6流程

- 做项目和做产品有很大不同

- [Matlab向量化编程](https://www.zhihu.com/question/50423550)


- [python dict 嵌套](https://anjingwd.github.io/AnJingwd.github.io/2017/08/19/%E5%A6%82%E4%BD%95%E4%BC%98%E9%9B%85%E7%9A%84%E7%94%9F%E6%88%90python%E5%B5%8C%E5%A5%97%E5%AD%97%E5%85%B8/
)

- [AI人工智能图片放大](http://bigjpg.com)

- [开机启动](https://blog.csdn.net/sinat_38682860/article/details/93776792)
[开机启动2](https://zhuanlan.zhihu.com/p/62258128)

- [python 调用 bash](https://blog.csdn.net/u010429424/article/details/76896918)


- 软件测试
1. 软件很容易升级，有了 Bug ，起码后台数据库的数据一般不会损坏，打个电话，让客服帮忙弄一下。

2. 软件是有测试的。写测试，也就是去写一些能有验证代码的代码，往往也会模拟一些输入和输出情况的。

3. 形式化验证是超豪华版的测试，用严格的数学论证，保证逻辑没有死角。

4. 对于区块链领域，代码即法律，可不是给客服打电话就能解决的。交给黑盒测试团队，去覆盖百分之九十九的可能，这是远远不够的。我们需要不计成本的去提高软件的可靠性。

- ADAS 难点
    1. 信号验证
    2. 防止突变
    3. 问题，track 为什么断了
    4. 单雷达追踪

- [Nginx](https://zhuanlan.zhihu.com/p/34943332)

*2020-03-21*

- 软件破解：程序验证可以多种多样，可以是电脑的注册表，也可以是系统时间，还可以是版本号。程序的功能是完全的，只是因为一些原因被关闭了而已。而cracker要做的，就是强行启动这些被关闭的功能。cracker常见的破解手法就是硬性修改程序的机器码。通过ollydbg这样的软件来将验证的逻辑修改掉，

- 游戏修改器
1. 修改文件数据：就是修改游戏过程中存在本地的数据。特别对于单机游戏而言，玩家的金币数、等级啥的，肯定得存在硬盘上的某个地方。
2. 修改内存数据:程序运行过程中，数据都是在内存里的。通过搜内存，即可直接修改游戏数据（金山游侠）。
3. 截包:对于网游来说，数据都是封装在一个一个数据包里，发送到服务器的。只要截取从你电脑发出去的游戏包，找到对应的数据，修改即可。但实际上，这是最困难的修改方式, 数据包通常用的是非对称加密算法，

- [fsm](https://blog.csdn.net/jgftyfc/article/details/83935200)
[fsm2](https://zhuanlan.zhihu.com/p/32743628)


- [图片转字符串](https://blog.csdn.net/mieleizhi0522/article/details/81908217)
[图片转字符串2](https://www.zhihu.com/question/275611095/answer/383461376)


- 开发成本不在于项目复杂度..在于你所用的框架的坑有多少

- C语言一切皆内存

- 技术选型是一个政治决定

- 言Python做胶水语语言，与C语言交互，只需要按要求写好C的API，再写个Python的setup脚本，就能将C代码编译成库文件

- Go语言可直接编译成机器码，不依赖其他库,静态类型语言，但是有动态语言的感觉，

- [pytgame flappy bird](https://zhuanlan.zhihu.com/p/106591651)

- [有限状态机]()https://zhuanlan.zhihu.com/p/32743628


*2020-03-20*

- 描图用sai钢笔曲线工具
- [google drive 变外链](https://wzfou.com/goindex/)
- [通过网络控制aduino](http://www.yeelink.net/)
- [aduino传感器](https://zhuanlan.zhihu.com/p/64861157)

- 惯导陀螺仪
[惯导](https://zhuanlan.zhihu.com/p/82854981)
[惯导](https://zhuanlan.zhihu.com/p/24280315)

- gps 地图
[地图](https://zhuanlan.zhihu.com/p/109965742)
[地图](https://www.zhihu.com/question/33783546)

- 手机录制gps
[gsp](https://www.zhihu.com/question/30478842)

*2020-03-20 CI continous integration*

- 改完代码要做代码检查，保证可以运行。如控制器不能有float64型变量。matlab不定义变量类型。代码生成会自动生成float 64
- 生成的autosar代码中matlab函数的输入输出都变成C代码的输入。
 ```
C代码
/* Function for MATLAB Function: '<S23>/ListJoint' */
static void SortIgnoreZero(float32 x[52], uint8 id[52])

Matlab代码
id = SortIgnoreZero(x)
```

*2020-03-19 游戏人工智能*

- 搜索技巧 -csdn.net

- automata自动机的话主要是编译器有用

- python game of life
 [link](https://www.geeksforgeeks.org/conways-game-life-python-implementation/)

- finite state machine
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
[sensor](runoob.com/python/python-date-time.html)
- 弹出框
[]
https://blog.csdn.net/lsxht95/article/details/79995112
https://www.cnblogs.com/leaf1117/p/3419640.html
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




