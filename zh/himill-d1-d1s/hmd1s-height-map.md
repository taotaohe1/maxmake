# 📏 MaxmakeLAB 3D测头高度图功能

## 🌟 功能介绍

MaxmakeLAB的3D测头高度图功能允许您通过3D测头自动探测工件表面的高度变化，并根据探测结果调整加工路径，从而获得更精准的加工效果。此功能特别适用于表面不平整的工件加工。

---

## 📋 准备工作

在使用高度图功能前，请注意以下几点：

1. **熟悉3D测头使用**：建议先熟悉并掌握3D测头的基本使用方法
2. **安装并测高**：确保已经先点击换刀，安装3D测头，并完成3D测头的自动测高
3. **设置加工原点**：建议先设置好加工原点（XY零点），并自动探测并设置Z零点
4. **连接稳定性**：建议使用USB连接设备时使用此功能。如果使用WIFI连接，请确保WiFi连接通畅，避免通信错误

> ℹ️ 提示：在开始使用高度图功能前，请确保您已经熟悉3D测头的基本操作流程。
> 
> {.is-info}

---

## 🛠️ 使用流程

### 步骤1：安装3D测头并完成测高

1. 在主页面中，点击换刀按钮
2. 安装3D测头
3. 完成自动测高

<img src="/chi/himill-d1-d1s/media/height-map/1.换测头并测高.webp" alt="1.换测头并测高" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤2：完成加工原点的自动探测

1. 切换到Probe页面
2. 完成加工原点的自动探测，包括XYZ零点

<img src="/chi/himill-d1-d1s/media/height-map/2.probe页面.webp" alt="2.probe页面" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤3：切换到高度图页面并导入加工文件

1. 切换到高度图页面
2. 导入加工文件（也可一开始导入）

<img src="/chi/himill-d1-d1s/media/height-map/3.切换并导入文件.webp" alt="3.切换并导入文件" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤4：创建并编辑探测点位

1. 点击Create按钮，自动打开Edit界面
2. 创建并编辑探测点位

<img src="/chi/himill-d1-d1s/media/height-map/4.编辑探测点.webp" alt="4.编辑探测点" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 编辑参数说明

- **Border**：
  - XY：探测范围的坐标信息
  - WH：探测范围的宽度高度
  - 点击自动按钮可以将探测范围设置为导入的文件的加工范围

- **Probe Grid**：
  - XY：横向纵向的探测点数（探测点位越多越精准，但耗费的时间更多）
  - Zt：探测的安全高度
  - Zb：探测的下探距离

- **Interpolation**：
  此功能暂未实现，现在只能更改数值但无实际效果。后续更新会补充此功能

### 步骤5：开始探测

1. 点击Grid Probe开始探测
2. 开始时，会在XY0处先自动探测一次，找到的位置作为基准平面
3. 后续的探测会以此点计算Z坐标差值
4. 可以点击Gcode列表查看探测的差值

<img src="/chi/himill-d1-d1s/media/height-map/5.点击开始探测.webp" alt="5.点击开始探测" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤6：应用高度图

1. 探测结束后，点击Edit按钮，退出探测界面
2. 点击Use Height Map，应用刚刚的探测值
3. 可观察到路径发生了变化

<img src="/chi/himill-d1-d1s/media/height-map/6.点击使用.webp" alt="6.点击使用" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤7：更换刀具并开始加工

1. 切换到主界面点击换刀按钮
2. 换成要加工的刀具
3. 点击开始加工

---

## ⚠️ 注意事项

> ⚠️ **Gcode文件导入要求**：
> - 使用高度图功能一定要先导入Gcode文件，才能点击Create，编辑探测点，之后才能点击Grid Probe
> - 如果中途切换了文件，或者先进入高度图再导入文件，会出现点击Grid Probe后直接加工了导入的文件
> - 遇到上述情况，需要取消Edit再点击Create重新进入编辑界面
> - 此问题在后续版本中会更新解决
>
> {.is-warning}

> ℹ️ **探测时间**：
> - 探测点位越多，精度越高，但耗费的时间也会相应增加
> - 请根据实际加工需求平衡精度和时间
> 
> {.is-info}

> ⚠️ **安全高度**：
> - 请确保设置合适的安全高度（Zt），避免碰撞
> 
> {.is-warning}

> ℹ️ **通信稳定性**：
> - 使用WiFi连接时，请确保网络稳定，避免探测过程中因通信错误导致失败
> 
> {.is-info}

---

## ❓ 常见问题

### Q: 探测过程中出现通信错误怎么办？
A: 检查网络连接，确保USB连接稳定或WiFi信号良好，然后重新开始探测流程。

### Q: 探测结果不准确怎么办？
A: 增加探测点位数量，确保探测范围覆盖整个加工区域，同时检查3D测头是否正确安装。

---

## 📅 后续更新

- **Interpolation功能**：后续版本将实现插值功能，进一步提高高度图的精度
- **Gcode文件导入流程优化**：优化Gcode文件导入与高度图功能的交互流程，避免点击Grid Probe后直接加工的问题
- **操作优化**：简化探测流程，减少用户操作步骤

---

> ⚠️ 注意：使用高度图功能时，请确保3D测头已正确安装并完成测高，避免因操作不当导致设备损坏。
> 
> {.is-warning}