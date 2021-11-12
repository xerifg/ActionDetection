# 动作捕捉平台

能负担的起的动作捕捉平台简介，[视频](https://www.youtube.com/watch?v=cggrDnjdUwI)

马克斯普朗克3Dpose识别的研究实验室结果，[地址](https://vcai.mpi-inf.mpg.de/GVV_Projects.html)

## 基于传感器的

### 1. iPi soft

包含ipi recorder,ipimocap studio两个软件，一个采集数据，一个3D动画的动作展示

 iPi soft兼容的摄像头

1. Sony PlaystationEye
2. Microsoft Kinectfor Windows / Kinect XBOX 360
3. ASUS Xtion / XtionLive
4. PrimeSense Carmine1.08
5. Any DirectShowcompatible web cameras

### 2. VDMocap

超次元推出的虚拟动力动捕软件，需要搭配虚拟动力VDSuit Full全功能动作捕捉设备使用，设备拥有27个高精度感应器，360度姿态不好做范围，单POSE校准

### 3. NoKov(度量)

国内的基于mark点的运动捕捉系统

## 基于纯视觉的

### 1. VNect（单目RGB）

VNect既可以实时预测人物的三维姿态，也可以定位图人物的位置。这允许系统避免在不包含人类的图像区域上浪费计算。在机器学习过程中，系统的神经网络通过数万个注释图像进行训练。系统根据关节角度提供三维姿态信息，而这可以轻松用于控制虚拟角色.

但VNect仍然存在局限性。姿态估计的准确度比多相机系统或基于标记的姿态估计系统更低。如果人脸被遮挡，运动速度太快，或者出现没有训练过的姿势，系统将出现问题。另外，多用户场景也是一个问题。

[Real-time 3D Human Pose Estimation with a Single RGB Camera](https://vcai.mpi-inf.mpg.de/projects/VNect/)

### 2. XNect（单目、多人）

多人识别，相关解读[博客](https://www.cnblogs.com/zhongzhaoxie/p/14299143.html)，[博客2](https://aijishu.com/a/1060000000180901)

### 3. Openpose（单目、开源）

[Github地址](https://github.com/CMU-Perceptual-Computing-Lab/openpose)

开源，2D+3D的姿态估计，且在unity有插件

### 4. DeepCap

[youtube视频](https://www.youtube.com/watch?v=C4eDrvJ9aBs)

### 5. DeepPose（单目）

只需要上传普通的视频，就可以生成3D动作动画甚至还有脸部动作跟踪，还可以将动作数据应用到自己制作的3D人物上。其运动数据会以fbx的格式存储下载，具体的操作过程可以看[这里](https://www.youtube.com/watch?v=hPIO7DPLnUs)

### 6. DeepMotion（单目）

[主页](https://www.deepmotion.com/)

上传视频，自己可以像搭积木似的制作自己的3D模型，支持多种格式输出

### 7. Getrad（单目）

与DeepMotion类似

### 8. Radical studio（单目）

[地址](https://getrad.co/studio-product/) 

[直接地址](https://getrad.co/dashboard/)

上传视频，生成3D动画，以fbx格式保存，收费的

### 9. EasyMocap（开源）

多视角检测

### 10. ThreeDPoseUnityBarracuda（单目、开源）

[Github地址](https://github.com/digital-standard/ThreeDPoseUnityBarracuda)

利用Unity自带的Barracuda库去运行神经网络进而对2D视频进行实时动作捕捉

### 11. Physics-based Human Motion（单目）

[论文](https://arxiv.org/abs/2109.09913)

[项目主页](https://nv-tlabs.github.io/physics-pose-estimation-project-page/)

**lntel**提出的基于训练好的人体运动模型进行约束，外加姿态估计.

可以进行地面力反馈，可实现脚由于重力而与地面的附着效果

### 12. freemocap（多目、开源）

[Github地址](https://github.com/jonmatthis/freemocap)

### 13. I2L-MeshNet

[论文](https://arxiv.org/abs/2008.03713)

[Github地址](https://github.com/mks0601/I2L-MeshNet_RELEASE)

实现了论文中的模型训练，用Pytorch进行的训练

### 14. 3D-pose-baseline（单目、开源）

[论文](https://arxiv.org/pdf/1705.03098.pdf)

[Github地址](https://github.com/una-dinosauria/3d-pose-baseline)

由单目RGB估计3Dpose，且解决了光照影响问题

### 15. Lifting from the Deep（单目、开源）

[论文](https://openaccess.thecvf.com/content_cvpr_2017/papers/Tome_Lifting_From_the_CVPR_2017_paper.pdf)

[Github地址](https://github.com/DenisTome/Lifting-from-the-Deep-release)

采用一种综合方法，将 3D 人体姿势的概率知识与多级 CNN 架构相融合，并使用合理的 3D 地标位置的知识来优化 2D 位置的搜索

### 16. [ArashHosseini/3d-pose-baseline](https://github.com/ArashHosseini/3d-pose-baseline)

根据 OpenPose 检测到的人体骨骼结构生成 3D 人体模型。

# 密集模型搭建

### 1. DensePose

[Youtube](https://www.youtube.com/watch?v=Dhkd_bAwwMc)
