#### 设备模板

同一类型的工业设备往往配置基本完全相同，我们可以通过创建设备模板来快速配置同类设备。
在设备中心选择设备模板，点击右侧添加设备模板按钮，输入设备名称完成创建。

**1、创建模板**

![Alt text](images\device_center\device_model\create_model.gif)

**2、模板组态设计**

在此处进行监控画面的组态。通过拖拽不同元件，设置大小颜色等属性，关联数据变量，完成自定义的监控界面设计。

**变量导入**

将设备监控的数据关联到当前模板，模板中可以导入多个盒子的变量，首先根据需要创建多个数据源，然后在每个数据源中输入盒子账号的用户名密码、盒子序列号导入该盒子中的变量，以供后期设计组态的使用。

![Alt text](images\device_center\device_model\import_variable.gif)

**组态设计**

在此处进行设备的缩略图和主页面的组态设计，拖拽不同元件设置相应的属性，关联数据变量，完成自定义的监控界面设计。

![Alt text](images\device_center\device_model\configure_design.gif)

**发布**

设备组态设计完成后，点击发布，配置信息将保存并下发到使用该模板的设备上。如没有使用该模板的设备，点击发布后，配置的信息将保存，添加设备后可直接发布。

**3、设备模板权限**

在此处可以对该模板进行权限设置。

![Alt text](images\device_center\device_model\model_power.png)

与设备权限设置相似，用户自己创建的模板，就会有对此模板的查看、组态设计权限，可以增加、删除、修改该模板的权限。

![Alt text](images\device_center\device_model\model_con.gif)

拥有设备模板权限的用户，在管理---用户---权限---设备模板权限中可以对用户进行设备模板权限进行分配。

![Alt text](images\device_center\device_model\user_modelpower.png)

**注意：**  

- 配置用户权限页面中，不勾选查看和组态设计权限，则该设备模板就会在模板列表中不展示，如果想添加回来，需要在用户权限中添加此模板的查看、组态设计权限
- 配置模板的权限时，勾选“组态设计”权限就一定会连带勾选“查看”权限
- 已经使用了某个模板的设备，取消了该用户的此模板权限，关联此模板的设备仍能正常使用，在修改设备页面该模板会有“没有权限”的标志


**4、组态画布**

组态画面分为网页端和移动端，分别Web端和移动端展示。 

**设置启动画面**    
启动画面是指展示组态的第一页。网页端默认“主画面”为启动画面，且网页端的启动画面是不能删除的，但是可以修改其他组态画面为启动画面；移动端默认没有启动画面，可以进行设置。

![Alt text](images\device_center\device_model\set_mainview.png)

**注意：**  

- 移动端在没有启动画面的情况下，展示的是网页端的组态，会以网页端的启动画面为启动画面；如果移动端有启动画面，则展示的是移动端组态。

**画布大小可调整**  
新建画布网页端大小默认为1280X720（16：9),移动端大小默认为720X1280（9:16），客户可根据需要进行调整。

![Alt text](images\device_center\device_model\set_view_size.gif)

**画布位置可调整**  
画布的位置可以根据需要进行调整，元件可以拖动在画布外展示，以便使用。画布位置的调整需要用到的快捷键如下：

alt + 拖动鼠标：移动画布  
ctrl + 鼠标滚轮：缩放画布  
ctrl + （+ 键）、（- 键）：缩放画布  
Ctrl + 0 ：恢复画布缩放

对于画布中的元件有以下快捷键： 

方向键：按1px移动 
shift+方向键：按背景网格对齐像素移动  
Del & Backspace：删除  
Ctrl-X & Shift-Del：剪切  
Ctrl-C & Ctrl-Insert ：复制  
Ctrl-V & Shift-Insert：粘贴  
Ctrl-A ：全选  
Ctrl-Z & Alt-Backspace：撤销  
Ctrl-Y & Alt-Shift-Backspace：重做  

**画布网格设置**  

组态画布中会有背景网格，为了方便客户进行组态设计，可以对画布中的网格进行设置。  
显示网格：点击显示/取消，画布中的背景网格会显示或者取消，默认的组态是显示网格的。

![Alt text](images\device_center\device_model\Background_grid.png)

网格对齐：选择后，组态中元件的位置会按照左边、上边与背景网格进行对齐。  

对齐线对齐：设计组态时，选择元件时会出现此元件与其他元件对齐的延长线，方便定位。

![Alt text](images\device_center\device_model\Alignment_line.png)

**画布背景可设置** 

画布背景可以选择“纯色”、“图片”、“图库图形”三种，客户可根据自己的需要设置画布的背景。

![Alt text](images\device_center\device_model\Canvas_background.gif)

也可以双击画布设置画布的背景。

**5、元件状态**   

元件的状态会根据此元件关联的变量状态进行判断。状态分为：未绑定、离线、加载中、数据异常、禁用五种状态。 状态图标会在元件的右上角显示，便于客户查看。  

未绑定：该元件关联的变量所在的数据源没有绑定盒子，该元件就会展示为未绑定状态。

![Alt text](images\device_center\device_model\unbind.png)

离线：该元件关联的变量所在的数据源绑定的盒子处于离线状态，该元件就会展示为离线状态。

![Alt text](images\device_center\device_model\offline.png)

加载中：该元件关联的变量数据还没有推送到云组态，该元件就会展示为加载中状态。

![Alt text](images\device_center\device_model\loading.png)

数据异常：该元件关联的变量数据错误或者超时时，该元件就会展示为加载中状态。

![Alt text](images\device_center\device_model\yichang.png)

禁用：禁用分为两种情况：  
如果该元件没有操作权限，就会展示为禁用状态，点击元件会提示“您无权限执行此操作”；  

![Alt text](images\device_center\device_model\jinyong1.png)

如果该元件有操作权限，但是逻辑控制条件不满足或者是条件中的变量数据异常，该元件也会展示禁用状态，点击原件会提示“操作条件不满足或逻辑控制变量异常”。

![Alt text](images\device_center\device_model\jinyong2.png)

