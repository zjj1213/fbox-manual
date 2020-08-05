设备中心模块主要有配置账号、设备模板、（非标）设备管理、设备监控四部分，下面会一一详解。

#### 设备监控

设备监控页包含设备列表，组态画面，设备详情，报警与历史数据等内容。

![Alt text](images\device_center\device_monitor\device_monitor.jpg)

**设备列表**

系统根据设备所在区域、设备分配所属客户、设备关联的模板自动生成设备树，没有定位的设备在“区域”-->"其他"中查找，没有分配的设备在“客户”-->“未分配设备”中查找，在查询栏中可以通过设备名称查询设备。

**组态画面**

显示组态设计完成的设备监控画面，设备运行状态一目了然，并且可以进行数据输入操作，权限允许情况下，可以实现远程启停设备，远程设置参数。

**设备详情**

该区域包含一些设备详细信息，除了设备名称，设备报警统计外，还包括一些设备模板、设备序列号、设备地点、备注等，这些信息是添加设备时录入的，方便用户管理。

**报警、历史数据、设备信息、维保档案**

当前报警：当前报警里表中是绑定的数据源此时此刻触发的报警，客户可根据数据源名称查询到是哪个绑定的盒子正在报警。  
历史报警：选择数据源，可以查询到该数据源下的历史触发/恢复的报警记录  
历史数据：选择数据源，可以查询该数据源中的历史数据，如果该数据源没有绑定，会提示“数据源未绑定”  
设备信息：设备信息记录了设备的基本信息和设备参与的维保计划信息  
维保档案：维保档案中记录了设备的报修工单和保修工单 


![Alt text](images\device_center\device_monitor\device_monitor2.gif)

**视频监控**（不绑定摄像头则无法使用这个功能）

**1、注册萤石云账号**

进入萤石云官网（www.ys7.com），登录个人账号（如没有先注册），进入定制服务，开发者服务。

![Alt text](images\device_center\device_monitor\register_yingshi_cloud.png)

在定制服务页面点击账户信息，根据提示填写相关信息。

![Alt text](images\device_center\device_monitor\register_info.png)

如果后期考虑升级为企业账号的请不要选择个人开发者。（企业信息请填写客户自己公司的信息）

点击我的应用，填写应用的信息。

![Alt text](images\device_center\device_monitor\establishment_registration.png)

进入应用秘钥，复制 APPKey 和 Secret 信息。

![Alt text](images\device_center\device_monitor\secret_key.png)

在我的资源---我的设备内，点击“标准流地址”设置摄像头直播。

![Alt text](images\device_center\device_monitor\view1.png)

在此处设置开启、暂停、关闭直播，如果在客户端中摄像头没有直播，需要检查这里摄像头直播是否处于“直播中”状态。

![Alt text](images\device_center\device_monitor\view2.jpg)

**注意**

- 我的资源--我的设备页面下方，有视频直播的源地址，我们只支持通道1的播放

![Alt text](images\device_center\device_monitor\view3.jpg)

- 如果视屏加密，会导致客户端的摄像头无法直播，需要在手机萤石云app登录账号，把加密关闭

![Alt text](images\device_center\device_monitor\view4.jpg)


**2、 绑定萤石云账号**

打开云组态，进入设备中心–配置—萤石云账号设置，点击绑定，输入 appkey 与 secret。

![Alt text](images\device_center\device_monitor\yingshi_cloud.png)

**3、绑定摄像头**
进入设备管理页面，点击更多—绑定摄像头，填写摄像头信息，（序列号验证码见摄像头 背面标签）

![Alt text](images\device_center\device_monitor\bind_camera.png)

添加摄像头是请确保摄像头为在线状态。 
查看摄像头。 进入设备监控页面，点击页面中下部分的视频监控（若未看到该选项表示该设备未绑定摄像 头）即可看到摄像头的实时画面。
![Alt text](images\device_center\device_monitor\video_monitor.png)

![Alt text](images\device_center\device_monitor\video.png)

**注意**

- 如果有绑定的摄像头，不能直接解绑萤石云账号，需要将绑定的摄像头全部解绑后，才能将账号解绑。

- 一个摄像头只能被一个设备绑定，但是一个设备可以绑定多个摄像头。
