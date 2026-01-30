# MaxmakeLab HiMill D1/D1S 安全门设置

## 📋 安全门功能说明

- 安全门功能可在设备设置中启用
- 启用安全门功能后，加工过程中打开前盖，加工会自动暂停。关上门后，长按按键2s后，才能继续加工
- 关闭安全门功能后，加工过程中打开前盖，不会影响加工

## ⚠️ 注意事项

> - 即使启用安全门功能，在前盖打开的情况下，仍能开始加工。若关门后再开门，才会触发暂停
> - 暂停过程中，主轴仍保持转动，注意安全
>
> {.is-warning}

---

## 📝 设置步骤

### 步骤 1：打开设备设置界面

在连接设备后，点击设备设置按钮，打开设备设置界面。

<img src="/zh/himill-d1-d1s/media/hmd1s-safe-door-setting/1.png" alt="设备设置界面" style="max-width: 800px;">

### 步骤 2：设置安全门功能

进入此界面后，安全门的开关会显示当前的开关状态。根据需要开启或关闭即可。

<img src="/zh/himill-d1-d1s/media/hmd1s-safe-door-setting/2.png" alt="安全门开关设置" style="max-width: 800px;">

### 步骤 3：查看安全门状态指示灯

在workflow状态栏中的安全门指示灯，只表示前盖的状态。可以通过此指示灯观察前盖是否正常关闭。

<img src="/zh/himill-d1-d1s/media/hmd1s-safe-door-setting/3.png" alt="安全门状态指示灯" style="max-width: 800px;">

- **指示灯亮起**：表示安全门关闭了
- **指示灯变灰**：表示未检测到前盖门关闭