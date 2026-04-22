# HiMill D1S Tool Installation Guide

This document details tool installation methods for HiMill D1S equipment, ensuring safe and accurate tool change operations.

---

## 1. Software Tool Change Preparation

Before installing tools, you need to click the tool change button in the software.

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/1软件中点击换刀.gif" alt="Click tool change button in software" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **Tool Change Preparation Key Points**:
> 
> - Ensure software interface displays normally
> - Check equipment connection status
> - Confirm no current machining tasks in progress
> 
> {.is-info}

---

## 2. Equipment Tool Change Status

The equipment enters tool change mode, the spindle moves to a convenient position for tool changing (X140,Y0), waiting for tool change. At this time, the indicator light shows yellow flashing light effect.

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/2主轴移动至换刀位置.webp" alt="Spindle moves to tool change position" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/2指示灯黄色跳动.webp" alt="Indicator light yellow flashing" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📱 **Equipment Status Confirmation**:
> 
> - Spindle has moved to tool change position
> - Indicator light shows yellow flashing, indicating tool change available
> - Ensure tool change area is obstacle-free
> 
> {.is-info}

---

## 3. Tool Installation

Pull down the handle, insert the tool, tool clamping must be ≥15mm. Slowly release the handle.

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/3拉下把手_放入刀具.webp" alt="Pull handle and insert tool" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/3刀具夹持大于等于15mm.webp" alt="Tool clamping greater than or equal to 15mm" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Tool Installation Safety Requirements**:
> 
> - Tool clamping depth should be between 15mm and 34mm (maximum insertion depth is 34mm)
> - Ensure tool installation is firm
> - Avoid tool misalignment or loosening
> 
> {.is-warning}

---

## 4. Tool Height Measurement

After confirming correct installation, click the button (either internal or external), the spindle will move above the height measurer to complete height measurement.

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/4内外部均可.webp" alt="Internal and external buttons both available" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/4单击按键.webp" alt="Click button to trigger height measurement" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Tool Height Measurement Precautions**:
> 
> - As long as there is T*M6 in the file code, the system will execute the tool change step. If the tool before this step has not been measured for height, after executing T*M6, the tool compensation will be wrong
> - The first tool before machining must complete height measurement before setting Z0. This avoids tool compensation errors after changing to other tools
> - If there is only one tool, you should also first change tool and measure height before setting Z0. This prevents compensation errors caused by T1M6 code in the program
> 
> {.is-warning}

---

## 5. Collet and Tool Matching

If D1S is equipped with a 6mm collet, 6mm tools should be installed.

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/5夹头与刀具匹配.webp" alt="Collet and tool matching" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📏 **Tool Specification Description**:
> 
> - If changing to 4mm tools, first put the tool into a 4mm reducing sleeve, then insert into the 6mm collet
> - If changing to 3.175mm tools, first put the tool into a 3.175mm reducing sleeve, then insert into the 6mm collet
> - Note that mixing is not allowed
> 
> {.is-info}

---

## 📋 Tool Installation Safety Summary

> 🚨 **Tool Installation Safety Key Points**:
> 
> - Tool clamping depth must meet requirements
> - Height measurement must be completed after each tool change
> - Check tool installation firmness
> - Follow tool specification matching principles
> 
> {.is-warning}