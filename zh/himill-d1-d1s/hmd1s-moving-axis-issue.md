# HiMill D1/D1S 移动轴运行异常

## 注意事项
>- **紧急情况处理**：如遇轴不停撞击或卡顿情况，应立即停止设备运行并断电，避免进一步损坏机械部件
>- **安全操作**：进行检查或维修前，请确保设备已完全断电
>- **操作规范**：手动调整轴位置时，应缓慢操作
>- **防护措施**：处理机械部件时，建议佩戴防护手套，防止划伤
> {.is-warning}
---

## 可能现象
- **上电未锁紧**：设备通电后，轴未处于锁紧状态，可能自由移动
- **轴不移动**：操作控制器时，轴无任何移动反应
- **轴移动卡顿**：轴在移动过程中出现卡顿、抖动或异常噪音

## 可能原因
### 电气故障
- 电机驱动器故障或损坏
- 电机连接线松动、接触不良或断线
- 电机本身故障

### 机械故障
- 机械传动部分（如丝杠、导轨）故障或有异物卡住
- 导轨或丝杠润滑不足导致摩擦增大

### 控制系统问题
- 限位开关被触发或损坏
- 参数设置错误
- 控制器软件异常

## 解决方法

### 1. 排除限位开关异常
- 开机后尝试回零操作，检查是否能正常移动
- 若回零失败，参考[限位开关异常文档](/zh/himill-d1-d1s/hmd1s-limit-switch-issue.md)进行排查

### 2. 检查机械传动部分
- 仔细检查传动路径是否有异物卡住
- 若发现卡顿，立即断电并移除异物

### 3. 检查电机连接线

#### X电机连接线
需要将主轴移动至右侧进行检查,尝试重新拔插
<img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/x电机.jpg" alt="X电机" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/x电机线.jpg" alt="X电机线" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### Y电机连接线
需要将设备侧放进行检查,尝试重新拔插
<img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/y电机线.jpg" alt="Y电机线" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### Z电机连接线
检查位置如下,尝试重新拔插
<img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/z电机线.jpg" alt="Z电机线" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 4. 检查润滑情况
- 检查导轨和丝杠是否润滑不足
- 若长期未润滑，移动时会产生噪音和卡顿

### 5. 重启设备
- 关闭设备电源，等待30秒后重新开机
- 观察轴移动是否恢复正常

### 6. 恢复参数设置
- 若移动仍然卡顿且声音异常，尝试恢复设备出厂参数。连接设备后，尝试在回零后点击恢复按键
<img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/恢复参数.png" alt="恢复参数" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 7. 恢复参数设置
- 检查主控板上的电机连接线是否松动或接触不良，拆后盖步骤请参考更换主控板的视频 [HiMill D1/D1S 更换器件仓部件](/zh/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/主控板未插线电机.jpg" alt="主控板未插线电机" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/chi/himill-d1-d1s/media/hmd1s-moving-axis-issue/主控板插线电机.jpg" alt="主控板插线电机" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />     

### 8. 联系技术支持
若以上方法均无效，请联系 support@maxmake.com 获取进一步帮助