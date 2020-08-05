#### 配置
将已经配置好的盒子Client账号关联到云组态平台，快速完成设备与平台的对接。

**1、配置盒子账户**  

在设备中心选择配置，填写盒子账号的用户名密码完成账号绑定。注意： 绑定账号后，绑定到云组态的盒子会自动关联到该账号下，而且该账号下的盒子可以直接绑定到云组态的设备中。

![Alt text](images\device_center\setting\account_setting.png)

**2、删除盒子账户**  
可以将配置的账户删除，但是已经被绑定的盒子不会被删除，进入该设备的监控页面会提示“该盒子目前不在您配置的账号下”：

![Alt text](images\device_center\setting\non_existent.png)


**3、更换盒子账户**

更换盒子账户，已经被绑定的盒子就会被迁移到新的账户中。

**4、修改密码**
如果在盒子client中更改了账号的密码，云组态没有随之修改的话，就会有相应的提示，在此处重新更改账户密码就可以了。

![Alt text](images\device_center\setting\modify_password.png)

在账号有“配置”权限的时候，系统会有如下提示：

![Alt text](images\device_center\setting\peizhi_quanxian.png)

在账号没有“配置”权限的时候，系统会有如下提示：

![Alt text](images\device_center\setting\unpeizhi_quanxian.png)


**5、重新连接**

当云组态与盒子服务器连接异常，会有如下提示，盒子服务器恢复正常时，手动点击“重新连接”，可以使云组态重新与盒子服务器恢复正常连接。

**萤石云账号配置**  

在此处可以绑定萤石云账号，在设备管理列表中绑定萤石云摄像头，可以在监控中心中查看到绑定的摄像头的情况。
![Alt text](images\device_center\setting\yingshi_cloud.png)

**注意：**

- 如果有绑定的摄像头，不能直接解绑萤石云账号，需要将绑定的摄像头全部解绑后，才能将账号解绑。
- 一个摄像头只能被一个设备绑定，但是一个设备可以绑定多个摄像头。