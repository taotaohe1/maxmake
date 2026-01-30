# MaxmakeLab HiMill D1/D1S 无法通过WiFi连接软件

---

## 🔌 连接问题

### ❓ 可能原因
- 设备未正确重启或回零
- WiFi账号或密码输入错误
- 电脑IP地址配置错误
- 路由器设置异常
- 设备天线连接不良


### ✅ 解决方法

1. **🔄 重启设备**
   - 关闭设备电源
   - 等待10秒后重新启动设备
   - 重启后确保设备回零，再进入设置界面
   - 尝试重新连接WiFi网络


2. **🔑 检查WiFi账号密码**
   - 确认WiFi账号和密码输入无误
   - 注意密码大小写和特殊字符
   - 重新输入密码

3. **🌐 检查IP地址配置**
   - 在「本地IP地址」下拉菜单中选择电脑的IP地址（通常只有一个选项，如有多个可在电脑网络设置中查看无线网卡IP地址）
   - 在下方输入框中输入设备IP地址

4. **📡 检查路由器设置**
   - 检查路由器是否屏蔽了设备
   - 查看路由器的MAC地址过滤配置
   - 确认路由器的WiFi频段（2.4GHz）配置【本设备只支持2.4GHz频段】
   - 重启路由器

5. **📱 测试设备热点功能**
   - 将设备切换至热点模式（具体操作流程参考 [HiMill D1/D1S 网络配置](/zh/himill-d1-d1s/hmd1s-network-configuration.md) 中的「切换至热点模式」部分）
   - 使用电脑搜索并连接设备热点
   - 若电脑能连接到热点，说明设备WiFi模块工作正常

6. **📡 检查设备天线连接**
   - 拆卸后盖，检查主控板上的天线是否脱落或松动
   - 拆卸后盖步骤请参考更换主控板的视频 [HiMill D1/D1S 更换器件仓部件](/zh/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
   - （如曾拆卸过顶盖，拆卸过程中可能将天线带落）
   - 打开顶盖检查天线连接状态
   - 打开顶盖步骤请参考更换移动轴电机的视频 [HiMill D1/D1S 更换移动轴电机](/zh/himill-d1-d1s/hmd1s-replace-moving-axis-motor.md)中的更换Z轴电机部分

> ⚠️ **重要注意事项**：
> - 打开顶盖时，注意一定不要牵扯到天线！！！
> 
> {.is-warning}

**天线在主控板上的位置：**

<img src="/zh/himill-d1-d1s/media/hmd1s-cannot-connect-software-via-wifi/主控板.jpg" alt="天线未插" style="width: 50%; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/zh/himill-d1-d1s/media/hmd1s-cannot-connect-software-via-wifi/wifi天线.png" alt="天线已插" style="width: 50%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

7. **📧 如问题仍未解决，请联系 support@maxmake.com**

---

## 📶 干扰问题

### ❓ 可能原因
- 周围存在强电磁干扰源
- WiFi信号被遮挡或衰减
- 设备距离路由器过远

### ✅ 解决方法
1. 将设备远离强电磁干扰源（如微波炉、无线路由器、蓝牙设备等）
2. 减少WiFi信号遮挡物，确保设备与路由器之间无金属障碍物
3. 将设备靠近路由器，或使用WiFi信号放大器
4. 尝试更换WiFi频段（2.4GHz），本设备只支持2.4GHz频段，如果用5GHz频段只能使用热点连接
5. 重启路由器和设备后重试连接
6. 如问题仍未解决，请联系 support@maxmake.com
