# HiMill D1 Basic Operation & Safety Guide: Power, Connection & Machining Safety

Learn essential safety procedures for HiMill D1 CNC machine operation. This guide covers voltage settings, USB connection, clamping safety, safety door requirements, and power-off maintenance procedures.

---

## 🔌 Electrical Safety

### 1. Voltage Check
Before using the equipment, determine whether the equipment's power voltage value complies with local voltage values. The power interface label will indicate the current equipment power voltage.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-贴纸-110v.webp" alt="Voltage Label 1" style="width: 150px; height: auto; margin-bottom: 8px; border-radius: 0px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-贴纸-230v.webp" alt="Voltage Label 2" style="width: 150px; height: auto; margin-bottom: 8px; border-radius: 0px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-贴纸-英文.webp" alt="Voltage Label 3" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 0px;" />

If it doesn't comply, please adjust before powering on. The adjustment position is as follows.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/电压调节位置.jpg" alt="Voltage Adjustment Position" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 8px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/电压调节位置内部.jpg" alt="Internal Voltage Adjustment Position" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 8px;" />

### 2. Voltage Switching
Slide to the left to switch to 230V, slide to the right to switch to 110V.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-1.webp" alt="Voltage Switch 1" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-2.webp" alt="Voltage Switch 2" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-3.webp" alt="Voltage Switch 3" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 3. Power Connection Operation
Remove the power interface label, insert the power cord, and turn on the power switch.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-4.webp" alt="Remove Label" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/1-用电安全-5.webp" alt="Insert Power Cord" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## 🔗 Data Cable Connection

### 1. USB Connection Steps
Take out the USB-B data cable, insert one end into the equipment's USB port and the other end into the computer's USB port.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/2-连接数据线-1.webp" alt="Equipment USB Port" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/2-连接数据线-2.webp" alt="Computer USB Port" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚡ **USB Connection Precautions**:
> 
> - Ensure complete insertion
> - Use good USB interfaces, avoid rust or looseness
> - If using a USB hub, ensure hub quality to avoid affecting data transmission, causing data errors or disconnections
> 
> {.is-warning}

---

## 🔧 Clamping Safety

### 1. Clamping Method Selection
According to workpiece size and tool path, reasonably select clamping methods such as clamping plate clamping, jaw vise clamping, or side push clamp clamping.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/3-装夹安全-1.webp" alt="Fixture Types" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. Clamping Requirements
Clamping should be firm. Loose clamping may cause the workpiece to be lifted by the spindle, potentially causing tool breakage.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/3-装夹安全-2.webp" alt="Proper Clamping" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📏 **Clamping Safety Precautions**:
> 
> - The total height of clamped workpieces should not exceed 80mm to avoid collision with equipment components
> - If the workpiece is too tall or when using rotary axis processing, the spindle height needs to be adjusted
> 
> {.is-info}

---

## ⚠️ Machining Safety

### 1. Safety Door Requirements
Keep the safety door closed during machining, do not approach the moving spindle!

### 2. Safety Door Function Description
Note that even when the safety door function is enabled, machining can still be started in the software when the door is not closed. After the first door closing, opening the door again will pause machining. After closing the door, long-press the button for 2s to resume machining.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/4-加工安全-1-安全门.jpg" alt="Safety Door 1" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1-basic-operation-and-usage-safety/4-加工安全-2-打开安全门会暂停加工.webp" alt="Safety Door 2" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1-basic-operation-and-usage-safety/4-加工安全-3-恢复加工.webp" alt="Safety Door 3" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 🚨 **Safety Door Important Reminder**:
> 
> When the door is open and the program is paused, the spindle will still rotate. DO NOT APPROACH!!!{.is-danger}

### 3. Hand Safety
Do not operate with gloves on to avoid entanglement with tools.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/4-加工安全-4.webp" alt="No Gloves" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## 🚫 Strictly Prohibit Disassembly Under Power

### 1. Safe Operation Requirements
If accessories or electrical components need to be replaced, please disconnect power and unplug the power cord before operation. Avoid disassembling under power.

<img src="/eng/himill-d1-d1s/media/basic-operation-and-usage-safety/5-严禁带电拆机.webp" alt="Power Off Operation" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚡ **Electrical Safety Warning**:
> 
> - Disassembly under power is extremely dangerous and may cause electric shock accidents
> - Power must be cut off before any electrical maintenance
> - Operate only after unplugging the power cord
> 
> {.is-danger}