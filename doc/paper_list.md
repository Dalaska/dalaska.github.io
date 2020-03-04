# 感知融合精读论文

## 雷达聚类

- 雷达处理杂波滤除 CFAR (Constant False Alarm Rate):Lee, Jae-Eun, et al. "Harmonic clutter recognition and suppression for automotive radar sensors." International Journal of Distributed Sensor Networks 13.9 (2017):1550147717729793.

- 德州仪器详尽雷达资料: Tracking radar targets with multiple reflection points (Texas Instruments)

- 雷达鬼影检测: Sole, Amir, et al. "Solid or not solid: Vision for radar target validation." IEEE Intelligent Vehicles Symposium, 2004. IEEE, 2004.

## 目标匹配

- 目标级融合详细步骤 Chavez-Garcia, Ricardo Omar, and Olivier Aycard. "Multiple sensor fusion and classification for moving object detection and tracking." IEEE Transactions on Intelligent Transportation Systems 17.2 (2015): 525-534.

- 摄像头雷达融合: Darms, Michael S., Paul E. Rybski, Christopher Baker, and Chris Urmson. "Obstacle detection and tracking for the urban challenge." IEEE Transactions on intelligent transportation systems 10, no. 3 (2009): 475-485.

- 激光雷达摄像头融合: Ziguo Zhong, Stanley Liu, Manu Mathew, and Aish Dubey.“Camera Radar Fusion for Increased Reliability in
ADAS Applications”. Electronic Imaging 2018.17 (2018): 

## 自动泊车

- 同济车位识别详细步骤和数据集 Li, Linshen, et al. "Vision-based parking-slot detection: A benchmark and a learning-based approach." 2017 IEEE International Conference on Multimedia and Expo (ICME). IEEE, 2017.

- 同济深度学习角点检测算法：Zhang, Lin, et al. "Vision-based parking-slot detection: A DCNN-based approach and a large-scale benchmark dataset." IEEE Transactions on Image Processing 27.11 (2018): 5350-5364.

- 分割 Wu, Yan, et al. "VH-HFCN based Parking Slot and Lane Markings Segmentation on Panoramic Surround View." 2018 IEEE Intelligent Vehicles Symposium (IV). IEEE, 2018.

- vslam: Huang, Yewei, et al. "Vision-based Semantic Mapping and Localization for Autonomous Indoor Parking." 2018 IEEE Intelligent Vehicles Symposium (IV). IEEE, 2018

- 超声波信号处理：Shao, Yunfeng, Pengzhen Chen, and Tongtong Cao. "A Grid Projection Method Based on Ultrasonic Sensor for Parking Space Detection." IGARSS 2018-2018 IEEE International Geoscience and Remote Sensing Symposium. IEEE, 2018.

- 融合：Suhr, Jae Kyu, and Ho Gi Jung. "Sensor fusion-based vacant parking slot detection and tracking." IEEE Transactions on Intelligent Transportation Systems 15.1 (2013): 21-36.

## 车道线

- Bosch车道线识别: Klotz, Albrecht, Jan Sparbert, and Dieter Hoetzer. "Lane data fusion for driver assistance systems." Proc. 7th International Conference on Information Fusion, Stockholm, Sweden. 2004.

- 车辆与车道线关系: Nguyen, VanQuang, et al. "A study on real-time detection method of lane and vehicle for lane change assistant system using vision system on highway." Engineering science and technology, an international journal 21.5 (2018): 822-833.

- 深度学习方法lanenet: Neven, Davy, et al. "Towards end-to-end lane detection: an instance segmentation approach." 2018 IEEE intelligent vehicles symposium (IV). IEEE, 2018.

- 车道定位 Real-Time Global Localization of Robotic Cars in Lane Level via Lane Marking Detection and Shape Registration Dixiao Cui, Jianru 4 Xue, Member, IEEE, and Nanning Zheng, Fellow, IEEE

## 态势预估

- cut-in预测，通过特征工程与机器学习预测切入目标：Heinemann, Tonja. Predicting cut-ins in traffic using a neural network. MS thesis. 2017.

- Zhu, Ying, et al. "Reliable detection of overtaking vehicles using robust information fusion." IEEE Transactions on Intelligent Transportation Systems 7.4 (2006): 401-414.


### 激光雷达

- ego-motion估计自车位置: Hoang, Berntsson. "Localisation using LiDAR and Camera." MS thesis. 2017.

- 车辆检测pipeline：Du, Xinxin, et al. "A general pipeline for 3d detection of vehicles." 2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2018.

- 博士论文：Zhongzhen Luo, LiDAR Based Perception System: Pioneer Technology for Safety Driving

- 相机融合：Car Detection for Autonomous Vehicle: LIDAR and Vision Fusion Approach Through Deep Learning Framework, Xinxin Du, Marcelo H. Ang Jr. and Daniela Rus

- 标定: Improvements to Target-Based 3D LiDAR to Camera Calibration, Jiunn-Kai Huang and Jessy W. Grizzle

### 机器视觉

- SOC系统设计: Zhou, Yuteng. "Computer Vision System-On-Chip Designs for Intelligent Vehicles." (2018).

- mobiley测距单目测速测距：Stein, Gideon P., Ofer Mano, and Amnon Shashua. "Vision-based ACC with a single camera: bounds on range and range rate accuracy." IEEE IV2003 Intelligent Vehicles Symposium. Proceedings (Cat. No. 03TH8683). IEEE, 2003.

- mobileye行人检测：Pedestrian Detection for Driving Assistance Systems: Single-frame Classification
and System Level Performance

### 深度学习
- resnet: He, Kaiming, et al. "Deep residual learning for image recognition." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.

- yolo目标检测:Redmon, Joseph, et al. "You only look once: Unified, real-time object detection." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.

- feature可视化:Zeiler, Matthew D., and Rob Fergus. "Visualizing and understanding convolutional networks." European conference on computer vision. Springer, Cham, 2014.

- 速度效果trade-off:Huang, Jonathan, et al. "Speed/accuracy trade-offs for modern convolutional object detectors." Proceedings of the IEEE conference on computer vision and pattern recognition. 2017.

### 场景识别
- 场景综述:Xue, Jian-Ru, Jian-Wu Fang, and Pu Zhang. "A survey of scene understanding by event reasoning in autonomous driving." International Journal of Automation and Computing 15.3 (2018): 249-266.

- 动作识别： Simonyan K, Zisserman A. Two-stream convolutional networks for action recognition in videos. In: Proceedings of Advances in Neural Information Processing Systems. Red Hook, NY: Curran Associates, Inc., 2014. 568-576

- fcn街景分割：Zhang Y, Qiu Z, Yao T, et al. Fully convolutional adaptation networks for semantic segmentation[C]//Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2018: 6810-6818.


### 系统设计
- ADAS handbook: Hermann Winner, Stephan Hakuli, Felix Lotz, Christina Singer.
“Handbook of Driver Assistance Systems" (2016)

- 系统从需求功能到详细设计Automotive Systems Engineering, Markus Maurer, Hermann Winner


