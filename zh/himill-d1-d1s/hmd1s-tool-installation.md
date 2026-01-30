# HiMill D1S 刀具安装指南

本文档详细介绍HiMill D1S设备的刀具安装方法，确保安全、准确的刀具更换操作。

---

## 1. 软件换刀准备

安装刀具前，需要在软件中点击换刀按钮。

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/1软件中点击换刀.gif" alt="软件中点击换刀按钮" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **换刀准备要点**：
> 
> - 确保软件界面正常显示
> - 检查设备连接状态
> - 确认当前无加工任务进行
> 
> {.is-info}

---

## 2. 设备换刀状态

设备进入换刀状态，主轴移动至方便换刀的位置（X140,Y0），等待换刀，此时指示灯显示黄色跳动灯效。

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/2主轴移动至换刀位置.webp" alt="主轴移动至换刀位置" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/2指示灯黄色跳动.webp" alt="指示灯黄色跳动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📱 **设备状态确认**：
> 
> - 主轴已移动到换刀位置
> - 指示灯显示黄色跳动，表示可换刀
> - 确保换刀区域无障碍物
> 
> {.is-info}

---

## 3. 刀具安装

拉下把手，放入刀具，刀具夹持需≥15mm。慢慢松开把手。

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/3拉下把手_放入刀具.webp" alt="拉下把手放入刀具" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/3刀具夹持大于等于15mm.webp" alt="刀具夹持大于等于15mm" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **刀具安装安全要求**：
> 
> - 刀具夹持深度建议≥15mm
> - 确保刀具安装牢固
> - 避免刀具偏移或松动
> 
> {.is-warning}

---

## 4. 刀具测高

确认安装无误后，单击按键（内外部均可），主轴会移动到测高器上方，完成测高。

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/4内外部均可.webp" alt="内外部按键均可" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/4单击按键.webp" alt="单击按键触发测高" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **刀具测高注意事项**：
> 
> - 只要文件代码中有T*M6，系统就会执行换刀步骤。此步骤前的刀具如果未测高，执行完T*M6后，刀具补偿会出错
> - 加工前的第一把刀具，一定要完成测高，才能设置Z0。避免后续换其他刀具后刀具补偿出错
> - 如果仅有一把刀具，也应先换刀测高后，再去设置Z0。以防止代码中有T1M6代码导致补偿出错
> 
> {.is-warning}

---

## 5. 夹头与刀具匹配

D1S如果选配了6mm夹头，应安装6mm刀具。

<img src="/zh/himill-d1-d1s/media/hmd1s-tool-installation/5夹头与刀具匹配.webp" alt="夹头与刀具匹配" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📏 **刀具规格说明**：
> 
> - 如果要更换4mm刀具，应先将刀具放入4mm变径套中，再塞入6mm夹头中
> - 如果要更换3.175mm刀具，应先将刀具放入3.175mm变径套中，再塞入6mm夹头中
> - 注意不能混用
> 
> {.is-info}

---

## 📋 刀具安装安全总结

> 🚨 **刀具安装安全要点**：
> 
> - 刀具夹持深度必须符合要求
> - 每次换刀后必须完成测高
> - 检查刀具安装牢固性
> - 遵守刀具规格匹配原则
> 
> {.is-warning}

---

