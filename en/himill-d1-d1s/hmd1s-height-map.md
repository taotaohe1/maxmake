# HiMill D1S 3D Probe Height Map Guide: Uneven Surface Compensation Tutorial

Learn how to use the height map feature with [3D probe](https://maxmake.com/products/3d-probe) on [MAXMAKE HiMill D1S](https://www.maxmake.com/products/himill-d1s) CNC machine. This guide covers surface detection point setup, grid probing, and precise machining for uneven workpiece surfaces.

## 🌟 Feature Introduction

The 3D probe height map feature in MaxmakeLAB allows you to automatically detect height variations on the workpiece surface using the 3D probe, and adjust the machining path based on the detection results for more precise machining. This feature is particularly suitable for machining workpieces with uneven surfaces.

---

## 📋 Preparation

Before using the height map feature, please note the following:

1. **Familiarity with 3D Probe**：It is recommended to first familiarize yourself with the basic usage of the 3D probe
2. **Installation and Height Measurement**：Ensure you have clicked the tool change button, installed the 3D probe, and completed the automatic height measurement of the 3D probe
3. **Set Machining Origin**：It is recommended to first set the machining origin (XY zero point) and automatically detect and set the Z zero point
4. **Connection Stability**：It is recommended to use this feature when connected via USB. If using WiFi connection, ensure the WiFi connection is stable to avoid communication errors

> ℹ️ Tip: Before using the height map feature, please ensure you are familiar with the basic operation process of the 3D probe.
> 
> {.is-info}

---

## 🛠️ Usage Flow

### Step 1: Install 3D Probe and Complete Height Measurement

1. On the main page, click the tool change button
2. Install the 3D probe
3. Complete automatic height measurement

<img src="/eng/himill-d1-d1s/media/height-map/1.换测头并测高.webp" alt="MAXMAKE HiMill D1/D1S Install Probe and Measure Height" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 2: Complete Automatic Detection of Machining Origin

1. Switch to the Probe page
2. Complete automatic detection of the machining origin, including XYZ zero points

<img src="/eng/himill-d1-d1s/media/height-map/2.probe页面.webp" alt="MAXMAKE HiMill D1/D1S Probe Page" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 3: Switch to Height Map Page and Import Machining File

1. Switch to the height map page
2. Import the machining file (can also be imported at the beginning)

<img src="/eng/himill-d1-d1s/media/height-map/3.切换并导入文件.webp" alt="MAXMAKE HiMill D1/D1S Switch and Import File" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 4: Create and Edit Detection Points

1. Click the Create button, which will automatically open the Edit interface
2. Create and edit detection points

<img src="/eng/himill-d1-d1s/media/height-map/4.编辑探测点.webp" alt="MAXMAKE HiMill D1/D1S Edit Detection Points" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

#### Editing Parameters Explanation

- **Border**：
  - XY：Coordinate information of the detection range
  - WH：Width and height of the detection range
  - Click the auto button to set the detection range to the machining range of the imported file

- **Probe Grid**：
  - XY：Number of detection points in horizontal and vertical directions (more points = higher accuracy but longer time)
  - Zt：Safe height for probing
  - Zb：Downward probing distance

- **Interpolation**：
  This function is not yet implemented. Currently, you can only change the value but it has no actual effect. This function will be added in future updates

- **Zt/Zb Parameter Settings**：
  - **Zt (Safe Height)**: Set to a value higher than the highest point of the workpiece to ensure the probe does not collide with the workpiece during movement
  - **Zb (Downward Probing Distance)**: Set to a value lower than the lowest point of the workpiece to ensure the lowest position of the workpiece can be detected

  <img src="/eng/himill-d1-d1s/media/height-map/zt_zb_setting.webp" alt="MAXMAKE HiMill D1/D1S Zt and Zb Parameter Settings Diagram" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 5: Start Detection

1. Click Grid Probe to start detection
2. At the beginning, it will automatically detect once at XY0, and the found position will be used as the reference plane
3. Subsequent detections will calculate Z coordinate differences based on this point
4. You can click the Gcode list to view the detected differences

<img src="/eng/himill-d1-d1s/media/height-map/5.点击开始探测.webp" alt="MAXMAKE HiMill D1/D1S Click to Start Detection" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 6: Apply Height Map

1. After detection is complete, click the Edit button to exit the detection interface
2. Click Use Height Map to apply the just-detected values
3. You can observe that the path has changed

<img src="/eng/himill-d1-d1s/media/height-map/6.点击使用.webp" alt="MAXMAKE HiMill D1/D1S Click to Use Height Map" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### Step 7: Change Tool and Start Machining

1. Switch to the main interface and click the tool change button
2. Change to the tool to be used for machining
3. Click to start machining

---

## HowTo Schema Markup

<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "name": "How to Use HiMill D1S 3D Probe Height Map Feature",
  "description": "Complete guide for using the height map feature on MAXMAKE HiMill D1S CNC machine with 3D probe for automatic surface compensation on uneven workpieces.",
  "step": [
    {
      "@type": "HowToStep",
      "name": "Install 3D Probe and Complete Height Measurement",
      "text": "On the main page, click tool change button, install the 3D probe, and complete automatic height measurement."
    },
    {
      "@type": "HowToStep",
      "name": "Complete Automatic Detection of Machining Origin",
      "text": "Switch to Probe page and complete automatic detection of machining origin including XYZ zero points."
    },
    {
      "@type": "HowToStep",
      "name": "Switch to Height Map Page and Import Machining File",
      "text": "Switch to height map page and import your machining file (can also be imported at the beginning)."
    },
    {
      "@type": "HowToStep",
      "name": "Create and Edit Detection Points",
      "text": "Click Create button to open Edit interface, create and edit detection points including border coordinates and grid settings."
    },
    {
      "@type": "HowToStep",
      "name": "Start Automatic Detection",
      "text": "Click Detect button, the device will automatically move the 3D probe to detect each point and record height values."
    },
    {
      "@type": "HowToStep",
      "name": "Apply Height Map",
      "text": "After detection completes, click Edit to exit detection interface, then click Use Height Map to apply detected values."
    },
    {
      "@type": "HowToStep",
      "name": "Change Tool and Start Machining",
      "text": "Switch to main interface, click tool change button to replace with machining tool, then start machining with surface compensation."
    }
  ],
  "tool": [
    {
      "@type": "HowToTool",
      "name": "HiMill D1S 3D Touch Probe"
    },
    {
      "@type": "HowToTool",
      "name": "MaxmakeLab Software"
    }
  ]
}
</script>

---

## ⚠️ Notes

> ⚠️ **Gcode File Import Requirement**：
> - When using the height map feature, you must first import a Gcode file before clicking Create, editing detection points, and then clicking Grid Probe
> - If you switch files midway or enter the height map first and then import a file, clicking Grid Probe will directly start machining the imported file
> - In such cases, you need to cancel Edit and then click Create to re-enter the editing interface
> - This issue will be fixed in future versions
> 
> {.is-warning}

> ℹ️ **Detection Time**：
> - More detection points mean higher accuracy but also longer time consumption
> - Please balance accuracy and time according to actual machining needs
> 
> {.is-info}

> ℹ️ **Communication Stability**：
> - When using WiFi connection, ensure network stability to avoid failures due to communication errors during detection
> 
> {.is-info}

---

## ❓ Common Issues

### Q: What should I do if communication errors occur during detection?
A: Check the network connection, ensure stable USB connection or good WiFi signal, then restart the detection process.

### Q: What if the detection results are inaccurate?
A: Increase the number of detection points, ensure the detection range covers the entire machining area, and check if the 3D probe is correctly installed.

---

## 📅 Future Updates

- **Interpolation Feature**：Future versions will implement the interpolation function to further improve the accuracy of the height map
- **Gcode File Import Flow Optimization**：Optimize the interaction flow between Gcode file import and height map feature to avoid directly machining when clicking Grid Probe
- **Operation Optimization**：Simplify the detection process and reduce user operation steps

---

> ⚠️ Note: When using the height map feature, ensure the 3D probe is correctly installed and height measurement is completed to avoid equipment damage due to improper operation.
> 
> {.is-warning}