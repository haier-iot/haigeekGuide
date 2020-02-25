**海极网**   

海尔智家开发者平台（简称“平台”），是海尔面向IoT、AI等领域的开放平台。 
针对硬件开发者、APP开发者、服务开发者、内容开发者，提供不同的自助开发服务，满足不同开发者的开发需求。  

-网站: http://www.haigeek.com



**开发者及开发者账号**    
开发者指注册并使用海极网开发者平台的企业或个人。

开发者需使用海尔账号注册海极网账号，所注册用的账号即为开发者账号。


**海尔智能模组**   
海尔智能模组是由海尔研发的、为设备提供Wi-Fi或蓝牙连接能力的芯片模组。当前有Wi-Fi单模模组、Wi-Fi蓝牙双模模组、蓝牙单模模组。


**海尔设备开发板**  
海尔设备开发板中嵌有海尔智能模组，可供开发者模拟设备接入平台，进行平台熟悉及功能试用。

**产品、产品功能集及typeid、产品型号**  
产品是开发者在平台注册创建的智能硬件，比如“海尔天禧空调”就是一款产品。

产品功能集是在注册创建产品时定义的设备功能模型集合，是开发者在设备开发中管理的重要参数，typeid是产品功能集在平台的唯一标识，由平台分配。

产品型号是用户购买设备能够查看到的设备描述，由开发者在产品下创建产品型号，并定义产品型号功能（从产品功能集中选择）

>注1：如果两款硬件在用户可见的硬件整体外观上存在差异（比如颜色、形状等），但在软件部分完全相同，开发者可在平台创建一个产品，在产品下创建2个型号。

>注2：平台要求产品在升级过程中必须做到向下兼容，即新的版本必须支持过去版本功能的正常使用。如果一款硬件在后续的生产批次中发生无法向下兼容的变更（如替换模组），则需要为后续批次注册创建新的产品型号版本。


**IoT设备协议规范**
- 标准模型  
标准模型是海尔IoT设备模型规范，所有设备功能建模由海尔标准团队与开发者一同定义完成；

- E++协议  
是海尔定义电脑版与WIFI模组的协议规范；

- 设备  
是一个独立的有意义的设备，比如：灯泡、插座、风扇

- 属性  
设备的每个功能参数可以定义为设备的一个属性。以彩光灯为例，属性包括开关、亮度、颜色等

- 操作（组命令）
若一个有意义的操作，需要对多个属性进行读写，可以用方法来实现

- 告警  
事件的一种，对设备产生的故障的单独定义，上报给用户或售后；

- 事件  
简单的变化，用属性的上报来通知用户。复杂的变化，需要用事件来表达

!>注：产品功能定义是产品研发过程中必须的环节之一，是产品能够正常运行的基础，也是产品检验过程中的重要检验项之一，需开发者认真定义。


**设备及DeviceID**  
设备是指某一个智能硬件，如一台海尔空调。
DeviceID是设备在平台中的唯一标识，由平台分配。

>对于已使用海尔智能模组的设备，模组中具备DeviceID；  
>对于BLE设备，DeviceID由海尔智家APP添加设备时传给设备；  
>对于Android或Linux的设备，根据设备生产情况确定。  

**用户及UserID**  
用户指添加并使用已接入海尔开发者平台的设备的人。
UserID即为用户的海尔账号，是用户在平台中的唯一标识。

**应用**  
应用是指开发者拥有的、用于查看／控制已接入海尔开发者平台的智能硬件的程序，其形态可以是APP、Web、AI程序等等。  