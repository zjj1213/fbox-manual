运营中心主要为设备总体概览，添加到云平台的设备将在运营中心统一展示。运营中心分为“地图监控”和“集中监控”，地图监控展示的是有位置的设备的位置分布，集中监控展示的是添加的设备缩略图。
#### 地图监控
地图中相近的设备会叠到一块，展示叠加的设备的数量，鼠标点击相聚点，设备会分散开，同时地图会放大一定比例。鼠标点击设备图标可直接查看设备基本信息，点击“监控详情”可以直接进入设备监控页面，点击“设备管理”可以进入该设备的设备管理列表。

![Alt text](images\operation_center\device_distribution.gif)

设备不同状态以不同图标标识，标识的含义如下：
图标  | 名称  | 含义
--- | ---  | ---
![Alt text](images\operation_center\online.png)  | 在线 | 所有绑定的盒子都在线设备状态即为在线
![Alt text](images\operation_center\offline.png)  | 离线 | 任何绑定的盒子，其中一个有离线（无报警），设备状态即为离线
![Alt text](images\operation_center\unbind.png)  | 未绑定 | 所有数据源都未绑定，设备状态即为未绑定
![Alt text](images\operation_center\alarm.gif)  | 报警 | 任何绑定的盒子，其中一个有报警，设备状态即为报警
![Alt text](images\operation_center\bluetooth.png)  | 蓝牙  | 设备类型为蓝牙的设备
  
地图中有筛选人员和设备功能，勾选“设备”，在选框中选择设备关联的设备模板和设备分配的客户条件，地图中会展示出符合条件的设备，取消勾选，地图中只展示人员定位。客户可根据自己的需要查看想要的设备分布。

![Alt text](images\operation_center\map_filter.gif)
