# Alarm2 报错问题

## 问题描述

当设备在加工过程中出现 Alarm2 报错时，通常是由于 Z 轴行程不足导致的。本指南将详细介绍如何排查和解决这个问题。

## 排查步骤

### 第一步：连接设备

**操作步骤**：
确保设备正确连接到电脑，打开 MaxmakeLab 软件。

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/1连接设备.gif" alt="连接设备视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 第二步：点击 Workflow 进入加工界面

**操作步骤**：
1. 在 MaxmakeLab 软件中，点击顶部导航栏的 "Workflow" 按钮
2. 进入加工界面，准备进行后续操作

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/2进入加工界面.gif" alt="点击 Workflow 进入加工界面视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参考图片**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/1.jpg" alt="点击 Workflow 进入加工界面" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 第三步：执行换刀命令换上三坐标

**操作步骤**：
1. 在加工界面中，找到并点击 "换刀" 按钮
2. 等待设备到达换刀位置，换上三坐标测头
3. 确保三坐标测头安装稳固

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/3换上三坐标.gif" alt="执行换刀命令换上三坐标视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参考图片**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/2.jpg" alt="执行换刀命令换上三坐标" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 第四步：设置 XYZ 零点

**操作步骤**：
1. 使用三坐标测头探测工件表面
2. 在软件中设置 XYZ 零点坐标
3. 确认零点设置正确

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/4设置零点.gif" alt="设置 XYZ 零点视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参考图片**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/3.jpg" alt="设置 XYZ 零点" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 第五步：执行换刀命令换上加工刀具

**操作步骤**：
1. 再次点击 "换刀" 按钮
2. 等待设备自动换上加工刀具
3. 确保刀具安装稳固

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/5换上加工刀具.gif" alt="执行换刀命令换上加工刀具视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参考图片**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/4.jpg" alt="执行换刀命令换上加工刀具" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 第六步：检查换刀刀具补偿是否正确应用

**操作步骤**：
1. 调整Z轴，让刀尖靠近工件表面
2. 确认此时工件坐标是否接近零

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/6检验高度补偿.gif" alt="换刀后的检验高度补偿视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参考图片**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/5.jpg" alt="检验高度补偿" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 第七步：检查 Z 轴行程

**操作步骤**：
1. 加载您的加工文件
2. 观察 3D 预览中的 Z 行程范围
3. 确认 Z 行程范围是否在设备允许的范围内
4. 如果 Z 行程范围超出设备允许范围，那么此次加工一定会alarm2报错

**操作视频**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/7加工报错.gif" alt="加工报错视频" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参考图片**：
<img src="/chi/himill-d1-d1s/media/hmd1s-alarm2-error/6.jpg" alt="检查 Z 轴行程" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

**问题分析**：
在视频中可以看到，3D 预览中左下角的 Z 行程是 -10.5 到 5。这说明 Z 零点向上最大需要 5mm 行程，向下最大需要 10.5mm 的行程。

如果 Z 零点设置为 73mm，而设备的 Z 最大行程是 80mm，那么可用行程为 80mm - 73mm = 7mm，这远远不够加工所需的 10.5mm 向下行程，因此在加工过程中一定会报错。

## 解决方案

遇到这种情况，需要给 Z 轴行程预留足够的加工距离：

1. **调整 Z 零点位置**：将 Z 零点设置在更合适的位置，确保有足够的行程空间
2. **检查工件高度**：如果工件过低，考虑使用垫块或调整加工策略
3. **观察行程范围**：加工前一定要观察 3D 预览中的 Z 行程范围，确保在设备允许的范围内
4. **预留安全距离**：在设置零点时，建议预留至少 5-10mm 的安全距离

## 预防措施

1. **加工前检查**：每次加工前，务必检查 3D 预览中的行程范围
2. **零点设置**：合理设置零点位置，避免接近设备行程极限
3. **刀具长度**：使用合适长度的刀具，避免因刀具过长导致行程不足
4. **工件装夹**：确保工件装夹稳固且高度合适

> 💡 **提示**：如果仍然遇到 Alarm2 报错，请检查设备的限位开关是否正常工作，以及固件版本是否最新。
> {.is-info}