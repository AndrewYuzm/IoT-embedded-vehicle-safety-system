# IoT-embedded-vehicle-safety-system

本系统可用于车内婴幼儿遗留状态情况监测并做出相关反应措施，车内环境监测包括温湿度情况，若出现不适宜情况立即报警。
车辆落水安全监测及自动破窗设施。同时搭载北斗导航系统将行驶信息转递到制作的APP上，实现安全追踪。
危险驾驶行为监测可以检测到驾驶员的驾驶情况并进行警示。

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/0e360420-ee3d-47a7-a8ef-b6f7900bf387)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/9bd05356-1e1d-4941-9881-fe1275fbee7d)

一、滞留儿童监测
车辆熄火后，系统主动通过摄像头结合深度学习算法做图像识别判断车内有无滞留人员及婴幼儿；
并通过温湿度等传感器自动监测车内的环境数据，当车内儿童有窒息或者脱水的危险时，本系统会通过降低车窗等一系列措施主动解救车内被困儿童；
同时通过4G模组自动向车辆联系人发送求救信息并通过鸣笛报警寻求帮助，挽救被困儿童的生命。
所用模块：OPENMV摄像头、温湿度传感器、步进电机、4G模组

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/6ea7ae6d-f2a3-4080-ac37-2d71713d53ea)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/549311fc-5aa3-445f-9d31-89c322a54f51)

二、车辆落水自救
当驾车入水时，车内人员可以通过按下车内控制按钮使系统将车窗击碎，便于人员逃生，在车内人员无法主动按下控制按钮的情况下，水压检测器同时监测到长时间水压达到一定阈值后，向主板传递信息，系统也可自动将车窗击碎。
所用模块：车窗破碎器、水压传感器

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/43f922ba-9da0-4fa4-9dd8-9b5deb538cda)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/5fc462bc-3040-4452-9dba-607af3e0498e)

三、AI驾驶员危险行为监测
通过OPENMV做图像识别驾驶者驾驶状况，当驾驶者出现危险行为状态时，向主板传递信息，系统主动向驾驶员报警提醒。
我们的驾驶员危险行为检测采用了深度学习方法，考虑到模型压缩的问题，采用五层卷积层加三层最大池化层的方式，作为我们的神经网络框架，并使用了ReLU激活函数和动量法随机梯度下降，在数据集方面，我们使用了随机剪切等三种数据增强方法，经过我们的反复测试，最终达到测试集准确度为92.85%
所用模块：OPENMV摄像头，深度学习平台

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/c6b7c132-49fb-48c9-bf18-fb71f6bc6f9d)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/14f6f6a1-9c0c-4d9e-bb81-01bb9ca7c91a)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/25cae4be-0bd9-43c4-bdd4-ce35e46ccca2)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/a53cb3a0-7f4a-4be9-a3b2-81f256e5777b)

![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/5e4e1b6d-f2f7-4efe-bb88-28bc749fc54e)

四、制作APP，将搭载北斗导航系统的行驶信息转递到APP上，实现安全追踪。
1. 历史轨迹可以查看车辆行驶路线；
2. 定位功能可以展示车辆实时位置
3. 电子围栏可以限制车辆行驶范围，车辆超出范围后报警。
![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/626ba976-70e0-4b01-ba74-9a459c7ccdd7)
![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/d8fe3943-6926-451e-986e-f0c75d83932e)
![image](https://github.com/AndrewYuzm/IoT-embedded-vehicle-safety-system/assets/118711557/2f462c43-164e-4c6b-806f-18cb44fab78c)







