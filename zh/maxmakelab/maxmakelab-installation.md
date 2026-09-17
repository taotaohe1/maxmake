# MaxmakeLab 软件安装

## 📖 软件简介
MaxmakeLab是一款专为HiMill系列CNC设备设计的智能控制软件，提供直观的操作界面和丰富的加工功能，帮助用户轻松完成各种创意加工任务。

## 🖥️ 系统要求

### Windows系统
- **操作系统**：Windows 10/11（64位）及以上版本
- **处理器**：Intel i3或同等性能CPU（非ARM架构）
- **内存**：4GB以上
- **存储空间**：1GB以上可用空间
- **显示器**：分辨率1920x1080及以上
- **USB端口**：USB 2.0或更高版本

### macOS系统
- **操作系统**：macOS 14（Sonoma）及以上版本
- **处理器**：Apple Silicon
- **内存**：4GB以上
- **存储空间**：1GB以上可用空间
- **显示器**：分辨率1920x1080及以上
- **USB端口**：USB 2.0或更高版本

> ⚠️ **处理器兼容性注意**：
> 只支持Apple Silicon M系列芯片，暂不支持英特尔系列芯片。
> {.is-warning}

## 📥 软件下载
您可以通过以下链接下载MaxmakeLab软件，根据您的操作系统和需要选择相应版本：

> ℹ️ **0.9.20软件版本更新内容**：
> 
> **一、Probe功能**
> 1. 对刀界面添加对刀器状态灯显示
> 2. 对刀功能应用高度图在 GCode 的 M3/M4 指令后添加 F 值
> 
> **二、刀具参数与路径**
> 1. 修复偏移轮廓铣复杂刀具路径错误问题
> 2. 刀具参数库数据库功能调整：软件更新后不再覆盖用户修改的刀具参数。默认加载 toolbase_user.db3（不存在时自动从 toolbase.db3 复制），用户参数保存在该文件中
> 3. 添加重置刀具参数库的弹窗提示
> 
> **三、图层管理**
> 1. 修复 CNC 模式添加图形后，激光模式下会出现图层的问题
> 2. 修复激光模式下，图层没有图元时仍显示图层信息的问题
> 
> **四、图元操作与渲染**
> 1. 添加图元宽高渲染，标尺宽高高亮渲染
> 2. 对齐操作支持 Shift 单选图元时作为基准图元
> 3. 新增 2D 画布移动图元时对齐吸附功能
> 4. 修复多次解组后图元消失的问题
> 5. 添加裁剪功能
> 
> **五、文字编辑**
> 1. 修复添加文字动作交互时按 ESC 键 UI 问题
> 2. 修复双击文字二次编辑时按 ESC 键渲染问题
> 3. 添加文字时所选字体不支持字符时使用候选字体（项目中的字体）加载字形
> 4. 文字交互原有按 ESC 取消功能调整为提交功能，二次编辑文字修改后按 ESC 触发提交
> 5. 节点编辑功能重新设计：当前仅支持移动控制点，后续将添加增加节点、移除节点等功能
> 
> **六、报错与稳定性**
> 1. 修复 alarm 报错里面 3、4、5、8、9 里面的回零和检测按键会导致软件崩溃的问题
> 2. alarm 弹窗显示与关于窗口显示保持一致，不单独窗口显示
> 
> **七、UI/UX 优化**
> 1. 开启软件后的用户提示默认关闭
> 2. 换刀弹窗 3 秒后自动关闭
> 3. 修复裁剪动作时切换节点编辑动作时光标问题
> 
> 有任何软件问题，可在Discord软件反馈专区内联系我们。我们会积极参考大家的建议并及时修复问题：[Discord](https://discord.gg/u9XkszV3Mj)
> {.is-info}

### 最新版本 (v0.9.20)
**[MaxmakeLab 软件下载链接(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.20.exe)**
**[MaxmakeLab 软件下载链接(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.20.dmg)**

### 历史版本 (v0.9.19)
**[MaxmakeLab 软件下载链接(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.19.exe)**
**[MaxmakeLab 软件下载链接(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.19.dmg)**

### 历史版本 (v0.9.18)
**[MaxmakeLab 软件下载链接(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.exe)**
**[MaxmakeLab 软件下载链接(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.dmg)**

> 建议：请始终下载最新版本的软件，以获得最佳的功能体验和稳定性。
{.is-info}

## 🎬 安装使用流程

### Windows系统安装使用步骤

#### 1. 双击安装包安装软件

<img src="/chi/maxmakelab/media/maxmakelab-installation/1-双击安装软件.webp" alt="双击安装包安装软件" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 2. 打开软件

<img src="/chi/maxmakelab/media/maxmakelab-installation/2-打开软件.webp" alt="打开软件" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 3. 点击自动连接查找设备，连接后点击回零

<img src="/chi/maxmakelab/media/maxmakelab-installation/3-自动连接，点击回零.webp" alt="自动连接查找设备" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 4. 也可以选择设备，手动选择串口号连接

<img src="/chi/maxmakelab/media/maxmakelab-installation/4-手动连接.webp" alt="手动连接设备" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<!-- ### macOS系统安装使用步骤

#### 1. 下载并安装软件

> 📥 **下载安装**：
> 
> - 从官网下载Mac版本的安装包
> - 双击.dmg文件打开镜像
> - 拖拽MaxmakeLab到应用程序文件夹
> - 首次运行时需在系统偏好设置中授权

#### 2. 打开软件

> 🚀 **启动软件**：
> 
> - 从启动台或应用程序文件夹打开MaxmakeLab
> - 如果出现安全提示，按住Control键点击选择"打开"
> - 等待软件完全加载

#### 3. 点击自动连接查找设备，连接后点击回零

> 🔌 **设备连接**：
> 
> - 点击"自动连接"按钮
> - 等待软件搜索设备
> - 连接成功后点击"回零"操作
> - 确认设备状态正常

#### 4. 也可以选择设备，手动选择串口号连接

> ⚙️ **手动连接**：
> 
> - 从设备列表中选择您的设备
> - 手动输入或选择串口号
> - 点击连接按钮建立连接
> - 验证连接状态 -->

## ⚠️ 注意事项

> 🔍 **设备连接问题**：
> 
> 搜索不到设备时：
> 1. 尝试重启软件
> 2. 尝试拔插USB数据线
> 3. 检查设备是否已正确通电
> 4. 确保已安装正确的驱动程序
> 
> {.is-warning}

> ⚡ **电气安全**：
> 
> - 确保USB数据线连接牢固
> - 避免在数据传输过程中断开连接
> - 检查USB端口是否正常工作
> 
> 🛡️ **系统兼容性**：
> - 确认操作系统版本符合要求
> - 以管理员权限运行软件（如需要）
> - 关闭可能冲突的同类软件
> 
> 🔧 **故障排除**：
> - 重启软件和设备后重试
> - 检查设备管理器中的驱动状态
> - 尝试不同的USB端口
> {.is-info}


## ❓ 常见问题

### Windows系统问题

### Q：安装过程中出现错误怎么办？
A：请确保您的电脑满足系统要求，关闭其他可能冲突的软件，重新下载安装包并尝试安装。

### Q：软件启动后没有反应？
A：检查电脑是否安装了最新的显卡驱动，尝试以管理员身份运行软件。

### macOS系统问题

### Q：macOS系统提示"无法打开，因为来自身份不明的开发者"？
A：按住Control键并点击应用图标，选择"打开"，然后在弹出的对话框中再次点击"打开"即可。

### Q：macOS系统下无法识别设备？
A：
1. 确保已安装最新版本的macOS系统
2. 检查USB数据线是否连接稳定，尝试更换USB端口
3. 打开"系统偏好设置" → "安全与隐私" → "通用"，确认已授权MaxmakeLab的USB访问权限
4. 尝试重启软件和设备

### 通用问题

### Q：设备连接成功但无法控制？
A：检查USB数据线是否完好，尝试更换数据线或USB端口，确保设备已正确通电。

### Q：软件界面显示异常？
A：检查电脑是否安装了最新的显卡驱动，或调整显示器分辨率至推荐值。

---