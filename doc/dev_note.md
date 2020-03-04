# 开发笔记

## 供应商审核进入车厂供应商体系步骤：
1. 技术认可：考察配套经验、供货能力、审厂，技术考察包含了各种特殊场景；
2. 报价招标：综合考虑价格、品质、技术的过程；
3. 定点：确认车厂与供应商之间的合作关系；
4. 发RFQ文件，制定产品开发进度：样件要提供A、B、C三个阶段的测试。A样件称为功能样件，用于验证功能，B样件用于环境测试。环境测试包括高低温、电磁兼容、盐雾、沙尘、振动等等。C阶段是和量产一样的样件。

## 采购流程
- 院技术委员会评审供应公司考察，入库招标，签合同，验收

## 汇报材料
- 总结做了贡献，经验，kpi
- 立项与中体规划的联系
- 问题汇报时把感知边界情况说清楚

## 软件需求
- 功能性，非功能性
- 软件系统 = 软件+硬件+使用环境：software intensive system = software + hardware + context 

## debug 方法
- 从后往前想：reproduce, simplify, find origionsomething impossible ocurred,the only solid infomation is it did ocurredso we must think backward from the result

## 价值创造
搬砖，技能，人脉，资源，聚焦，信息，圈子，投资

## 网关
- 网关不具体特指一类产品，只要连接两个不同的网络的设备都可以叫网关；

## IP 地址
- 路由A，地址192.168.1.1
- 子网掩码255.255.255.0
- port, 程序入口
- 典型计算机B，地址192.168.1.129

## CAN总线
- 高低差分信号
- 终端电阻减少信号抖动
- 接口db9
- DBC， 信号矩阵 data base

# Vector Canoe， 
- 用于刷标定了，观测量
- 可以看值，通信会有延时
- 才数据看报文用analyzer

## autosar编程规范
- 代码生成
- a2l文件定义变量及标定观测量

## 功能安全
- ASIL: B,D(D高), PM

## 接口
感知的量里给控制bypasssensor can, body cansenor can直接通控制器，两路can都要进数采。
