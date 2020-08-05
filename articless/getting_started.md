### 快速入门
#### 第一步：配置BOX账号
在设备中心选择配置，填写盒子账号的用户名密码完成账号绑定。

![Alt text](images\getting_start\account_setting.gif)

#### 第二步：新建模板
在设备中心选择设备模板，添加设备模板。

![Alt text](images\getting_start\create_model.gif)

#### 第三步：导入BOX变量
进入新创建的模板组态，切换到“配置数据源”页面，新增数据源，然后从盒子导入变量，输入盒子账号的用户名、密码、盒子序列号。
![Alt text](images\getting_start\import_variables.gif)

#### 第四步：设计组态
导入变量后，通过拖拽不同元件，设置大小颜色等属性，关联导入的数据变量，完成自定义的监控界面设计。
#### 第五步：发布
组态设计好后，需要点击“发布“按钮，配置信息将保存并下发到使用该模板的设备上。
![Alt text](images\getting_start\release.gif)

#### 第六步：新建设备
在设备中心，设备管理页面，点击添加设备，选择新建的设备模板，填写基本信息，定位，完成设备创建。
![Alt text](images\getting_start\create_device.png)

#### 第七步：绑定BOX
设备创建完成后，点击绑定解绑数据源，将创建的设备正式关联现场的设备。模板中创建的数据源都展示在列表中，可以绑定多个BOX使用。（如果该盒子已经在关联的盒子账号下，密码可为任意值）
![Alt text](images\getting_start\bind_box.png)

#### 第八步：查看监控中心
点击设备名的超链接进入监控中心，就可以查看设备关联的设备模板中的组态元件和此设备的报警、历史数据、设备信息、维保档案等信息。