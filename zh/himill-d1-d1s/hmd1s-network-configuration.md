# 📡 MaxmakeLab HiMill D1/D1S 网络配置

## 🌟 功能介绍

HiMill设备内置WiFi模块，支持无线控制功能。通过网络配置连接设备后，在网络通畅的情况下，可获得与数据线连接控制一致的操作体验。以下是两种WiFi连接方法的详细说明：

---

## 🏠 局域网连接

局域网连接是让HiMill设备直接连接到家庭或办公室路由器，同一局域网络下的电脑可直接访问设备（电脑需同时连接到该路由器）。

### 步骤1：USB连接设备并完成复位

1. 启动MaxmakeLab软件
2. 使用USB数据线连接设备与电脑
3. 等待设备完成自动复位，确保设备状态正常后再进行下一步操作

<img src="/zh/himill-d1-d1s/media/network-configuration/usb连接.webp" alt="USB连接设备" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤2：选择STA模式并配置WiFi参数

1. 点击软件界面中的「设备设置」按钮
2. 在设置界面中选择「STA模式」
3. 输入路由器的WiFi名称（SSID）和密码

> ⚠️ **重要注意事项**：
> - 请务必确保WiFi名称和密码输入正确，此过程会直接将配置信息写入设备的WiFi模块，输入错误将导致连接失败
> 
> {.is-warning}

<img src="/zh/himill-d1-d1s/media/network-configuration/切换sta.webp" alt="选择STA模式并配置WiFi" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤3：点击Config按钮进行配置

1. 点击「Config」按钮开始配置过程
2. 软件会将配置信息逐条传输到设备中，请耐心等待配置完成
3. 配置成功后，软件会弹出「正在重启网络模块」的提示
4. 点击「确认」后，等待15-30秒让设备完成网络模块重启

<img src="/zh/himill-d1-d1s/media/network-configuration/点击config.webp" alt="点击Config进行配置" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤4：查看设备IP地址

1. 等待15-30秒后，重新打开「设备设置」界面
2. 如果设备成功连接到路由器，界面中会显示设备获取到的IP地址
3. 记录下此IP地址，后续连接需要使用
4. 关闭软件，断电重启设备以完成配网过程

> ⚠️ **重要注意事项**：
> - 设备重启前请拔掉USB数据线
> - 无线控制过程中，请保持USB数据线断开状态
> 
> {.is-warning}

<img src="/zh/himill-d1-d1s/media/network-configuration/查看sta_ip地址.webp" alt="查看IP地址" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤5：通过IP地址连接设备

1. 重新启动MaxmakeLab软件
2. 点击「连接」按钮，选择「IP连接」模式
3. 在「本地IP地址」下拉菜单中选择电脑的IP地址（通常只有一个选项，如有多个可在电脑网络设置中查看无线网卡IP地址）
4. 在「设备IP」输入框中输入刚才记录的设备IP地址
5. 点击「连接」按钮，成功连接后会弹出连接成功的提示框

> ⚠️ **连接提示**：
> - 如果首次连接失败，请断开后再次尝试连接
> - 连接成功后，建议点击进入「workflow」界面，执行「回零」操作，确认设备是否正常响应
> 
> {.is-warning}

<img src="/zh/himill-d1-d1s/media/network-configuration/通过sta连接设备.webp" alt="通过IP地址连接" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

---

## 📱 热点连接

如果家中没有网络环境，或局域网连接时设备响应延迟过高，可以尝试使用设备热点进行连接。

### 热点默认信息

- **热点名称**：HiMill-AP
- **热点密码**：12345678
- **默认IP地址**：192.168.0.1

### 切换为热点模式的操作步骤

如果设备已配置过网络，可按照以下步骤切换为热点模式：

### 步骤1：USB连接设备并完成复位

1. 启动MaxmakeLab软件
2. 使用USB数据线连接设备与电脑
3. 等待设备完成自动复位，确保设备状态正常

<img src="/zh/himill-d1-d1s/media/network-configuration/usb连接.webp" alt="USB连接设备" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤2：选择AP模式并准备配置

1. 点击软件界面中的「设备设置」按钮
2. 在设置界面中选择「AP模式」

> ℹ️ **功能说明**：
> - 当前AP模式与STA模式存在配置冲突，必须输入名称和密码才能点击配置按钮（可随意输入，后续版本将修复此问题）
> 
> {.is-info}

<img src="/zh/himill-d1-d1s/media/network-configuration/切换ap.webp" alt="选择AP模式并点击配置" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤3：点击Config按钮进行配置

1. 点击「Config」按钮开始配置过程
2. 等待软件完成配置传输
3. 配置成功后，软件会弹出「正在重启网络模块」的提示
4. 点击「确认」后，等待15-30秒让设备完成网络模块重启

<img src="/zh/himill-d1-d1s/media/network-configuration/点击config2.webp" alt="点击Config进行配置" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤4：重启设备并确认热点模式

1. 关闭软件，断电重启设备
2. 设备重启后会自动进入热点模式，热点名称为「HiMill-AP」

> ⚠️ **重要注意事项**：
> - 设备重启前请拔掉USB数据线
> - 无线控制过程中，请保持USB数据线断开状态
> 
> {.is-warning}

<img src="/zh/himill-d1-d1s/media/network-configuration/通过ap连接设备.webp" alt="查看IP地址" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### 步骤5：电脑连接设备热点

1. 在电脑的WiFi设置中找到并连接「HiMill-AP」热点
2. 输入热点密码：12345678

> ⚠️ **连接提示**：
> - 连接设备热点后，电脑将暂时断开互联网连接
> 
> {.is-warning}

### 步骤6：通过IP地址连接设备

1. 启动MaxmakeLab软件
2. 点击「连接」按钮，选择「IP连接」模式
3. 在「本地IP地址」下拉菜单中选择电脑的IP地址
4. 在「设备IP」输入框中输入默认IP地址：192.168.0.1
5. 点击「连接」按钮，成功连接后会弹出连接成功的提示框

> ⚠️ **连接提示**：
> - 如果首次连接失败，请断开后再次尝试连接
> - 连接成功后，建议点击进入「workflow」界面，执行「回零」操作，确认设备是否正常响应
> 
> {.is-warning}

<img src="/zh/himill-d1-d1s/media/network-configuration/通过ap连接设备.webp" alt="通过IP地址连接" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

---

## 📋 功能说明

> ℹ️ **当前功能状态**：
> - 目前仅支持IP网络连接功能
> - 其他网络相关功能正在开发中
> - 请持续关注此页面，我们会及时更新功能信息
> 
> {.is-info}

---

