# HiMill D1/D1S 限位开关异常

## 限位开关位置示意图

X限位开关位置：
<img src="/chi/himill-d1-d1s/media/hmd1s-limit-switch-issue/x限位.jpg" alt="X限位开关" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Y限位开关位置：
<img src="/chi/himill-d1-d1s/media/hmd1s-limit-switch-issue/y限位.jpg" alt="Y限位开关" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z限位开关位置：
<img src="/chi/himill-d1-d1s/media/hmd1s-limit-switch-issue/z限位.jpg" alt="Z限位开关" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## XY限位开关异常

### 可能现象
- 回零时，XY轴不停撞击，已经触发限位但无信号
- 回零时，XY轴卡住不回弹，已经触发限位后无法脱离

### 可能原因
- 限位开关连接线松动或接触不良
- 限位开关损坏
- 机械结构卡死
- 润滑不足
- 限位开关被异物遮挡

### 解决方法
1. 如遇轴不停撞击情况，立即停止设备运行，避免进一步损坏
2. 检查有无物体阻挡轴运动或者限位开关
3. 手动转动丝杆调整轴位置，使限位开关脱离触发状态
4. 尝试按压限位开关，观察回弹是否正常
5. 检查限位开关连接线是否松动，尝试重新拔插，具体请参考更换XY限位的视频 [HiMill D1/D1S 更换限位开关](/zh/himill-d1-d1s/hmd1s-replace-limit-switch.md)
6. 检查主控板上的限位连接端子是否连接正常，尝试重新拔插，拆后盖步骤请参考更换主控板的视频 [HiMill D1/D1S 更换器件仓部件](/zh/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/chi/himill-d1-d1s/media/hmd1s-limit-switch-issue/主控板未插线限位.jpg" alt="主控板未插线限位" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/chi/himill-d1-d1s/media/hmd1s-limit-switch-issue/主控板插线限位.jpg" alt="主控板插线限位" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> 

7. 检查传动部件是否需要上油
8. 重启设备后重试
9. 如问题持续，联系 support@maxmake.com 

---

## Z限位开关异常

### 可能现象
- 回零时，Z轴不停向上撞击，已经触发限位但无信号
- 回零时，Z轴移动到最上方后卡住不回弹，已经触发限位后无法脱离

### 可能原因
- Z轴限位开关连接线松动
- Z轴限位开关损坏
- Z轴机械结构卡死
- 润滑不足
- 限位开关被异物遮挡

### 解决方法
1. 如遇轴不停撞击情况，立即停止设备运行，避免进一步损坏
2. 检查有无物体阻挡轴运动或者限位开关
3. 手动转动丝杆调整轴位置，使限位开关脱离触发状态
4. 尝试按压限位开关，观察回弹是否正常
5. 检查限位开关连接线是否松动，尝试重新拔插，具体请参考更换Z限位的视频
6. 检查主控板上的限位连接端子是否连接正常，尝试重新拔插
7. 检查传动部件是否需要上油
8. 重启设备后重试
9. 如问题持续，联系 support@maxmake.com 