# HiMill D1 Tool Installation Guide

This document details tool installation methods for HiMill D1 equipment, ensuring safe and accurate tool change operations.

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

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/1-移动到合适的地方换刀.webp" alt="Spindle moves to tool change position" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

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

Loosen the collet with a wrench

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/2-用扳手拧松筒夹.webp" alt="Loosen collet with wrench" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Unscrew the collet by hand

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/3-用手拧下筒夹.webp" alt="Unscrew collet by hand" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Insert the tool into the collet and tighten it initially by hand

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/4-将刀具插入筒夹.webp" alt="Insert tool into collet" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Tighten the collet with a wrench

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/5-用扳手将筒夹拧紧.webp" alt="Tighten collet with wrench" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/6-建议夹取长度大于15mm.webp" alt="Tool clamping greater than or equal to 15mm" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Tool Installation Safety Requirements**:
> 
> - Tool clamping depth should be ≥15mm
> - Ensure tool installation is firm
> - Avoid tool misalignment or loosening
> 
> {.is-warning}

---

## 4. Tool Height Measurement

After confirming correct installation, click the button (either internal or external), the spindle will move above the height measurer to complete height measurement.

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/4内外部均可.webp" alt="Internal and external buttons both available" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1-tool-installation/7-自动测高.webp" alt="Click button to trigger height measurement" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **Tool Height Measurement Precautions**:
> 
> - As long as there is T*M6 in the file code, the system will execute the tool change step. If the tool before this step has not been measured for height, after executing T*M6, the tool compensation will be wrong
> - The first tool before machining must complete height measurement before setting Z0. This avoids tool compensation errors after changing to other tools
> - If there is only one tool, you should also first change tool and measure height before setting Z0. This prevents compensation errors caused by T1M6 code in the program
> 
> {.is-warning}

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