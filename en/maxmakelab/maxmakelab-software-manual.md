# MaxmakeLab Software Manual

## Table of Contents

- [1. Main Interface Function Areas Introduction](#1-main-interface-function-areas-introduction)
- [2. Menu Bar](#2-menu-bar)
- [3. Design Panel](#3-design-panel)
- [4. Parameter Panel](#4-parameter-panel)
- [5. Color Panel](#5-color-panel)
- [6. Device Panel](#6-device-panel)
- [7. Layer Panel](#7-layer-panel)
- [8. Toolpath Generation](#8-toolpath-generation)
- [9. CNC Processing Workflow](#9-cnc-processing-workflow)
- [10. Laser Processing Workflow](#10-laser-processing-workflow)

---

## <a id="1-main-interface-function-areas-introduction"></a>1. Main Interface Function Areas Introduction

<div style="display: flex; gap: 16px; flex-wrap: wrap;">
  <img src="/eng/maxmakelab/media/software-manual/main-interface1.png" alt="Main Interface Overall Layout 1" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
  <img src="/eng/maxmakelab/media/software-manual/main-interface2.png" alt="Main Interface Overall Layout 2" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
</div>

#### Interface Function Areas

| Area | Name | Function Description |
|------|------|---------------------|
| 1 | Menu Bar | Import/export files, adjust view size, software settings, help guidance, switch language, switch mode |
| 2 | Design Panel | Add various types of graphic elements |
| 3 | Canvas | Generally the equipment working area size |
| 4 | Color Panel | Assign different colors to graphic elements |
| 5 | Device Panel | Select, connect, and quickly control devices |
| 6 | Parameter Settings | In CNC, set blank parameters and tool library parameters |
| 7 | Generate Toolpath | Select the method for generating tool paths |
| 8 | Toolpath List | Display generated tool paths |
| 9 | Quick Control | In laser, quick control functions such as fast movement and reset |
| 10 | Layer Panel | Assign different processing parameters to graphic elements of different colors |
| 11 | Simulation Preview | Simulate and preview processing paths |
| - | Workflow | Click to enter processing preview interface |

---

## <a id="2-menu-bar"></a>2. Menu Bar

<img src="/eng/maxmakelab/media/software-manual/menu-bar.png" alt="Menu Bar Interface" style="width: 200px; height: auto; border-radius: 8px;" />

#### Common Operations

| Function | Description |
|----------|-------------|
| **Dropdown Menu** | Click dropdown list to select specific operations |
| <img src="/eng/maxmakelab/media/software-manual/dropdown-menu.png" alt="Dropdown Menu Example" style="width: 250px; height: auto; border-radius: 8px;" /> | |
| **Save** | Save current project |
| **Undo** | Undo previous operation |
| **Redo** | Restore next operation |

---

## <a id="3-design-panel"></a>3. Design Panel

<img src="/eng/maxmakelab/media/software-manual/design-panel.png" alt="Design Panel Interface" style="width: 40px; height: auto; border-radius: 8px;" />

#### Toolbox

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Tool</th>
      <th style="width: 20%;">Function Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Select**</td>
      <td>Enter selection mode, can select graphic elements, move graphic elements</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-select.gif" alt="Select Selection" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Image**</td>
      <td>Insert image, supports png, jpg, jpeg formats</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-image.gif" alt="Image Insert" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Basic**</td>
      <td>Add lines, squares, circles</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-basic.gif" alt="Basic Graphics" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Text**</td>
      <td>Add text</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-text.gif" alt="Text Insert" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Pen**</td>
      <td>Add Bezier curves</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-pen.gif" alt="Pen Tool" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Node**</td>
      <td>Node editing tool</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-node.gif" alt="Node Editing" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Offset**</td>
      <td>Offset the inner and outer contours of the current graphics</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-offset.gif" alt="Offset Tool" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Clipart**</td>
      <td>Add graphics of various categories</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-offset-clipart.gif" alt="Clipart Library" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Plugin**</td>
      <td>Include box generation, gear generation</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-plugin.gif" alt="Plugin Extensions" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="4-parameter-panel"></a>4. Parameter Panel

<img src="/eng/maxmakelab/media/software-manual/parameter-panel.png" alt="Parameter Panel Interface" style="width: 600px; height: auto; border-radius: 8px;" />

> 💡 Parameter panel displays after selecting graphics, hides after deselecting

#### Basic Transformations

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Point Coordinates**</td>
      <td>Select different points, display or set coordinate values of current points</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-点坐标.gif" alt="Point Coordinates" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Width and Height**</td>
      <td>Display or set width and height of current graphic element</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-宽高度.gif" alt="Width and Height" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Lock**</td>
      <td>Lock or unlock graphics aspect ratio</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-锁定.gif" alt="Lock" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Rotation Angle**</td>
      <td>Set rotation angle of graphic element</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-旋转角度.gif" alt="Rotation Angle" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Horizontal Mirror**</td>
      <td>Horizontally flip graphic element</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-水平镜像.gif" alt="Horizontal Mirror" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Vertical Mirror**</td>
      <td>Vertically flip graphic element</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-垂直镜像.gif" alt="Vertical Mirror" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### Alignment Tools

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Align**</td>
      <td>Left align, right align, horizontal center align, top align, bottom align, vertical center align</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-对齐.gif" alt="Align" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Distribute**</td>
      <td>Horizontal interval distribution, vertical interval distribution</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-分布.gif" alt="Distribute" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### Array Tools

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Rectangular Array**</td>
      <td>Quickly add graphics in rectangular array format</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-矩形阵列.gif" alt="Rectangular Array" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Circular Array**</td>
      <td>Quickly add graphics in circular array format</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-环形阵列.gif" alt="Circular Array" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Boolean Operations**</td>
      <td>Perform addition, subtraction, intersection, or exclusion of overlapping operations on two or more graphic objects to generate new graphics</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-布尔运算.gif" alt="Boolean Operations" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="5-color-panel"></a>5. Color Panel

<img src="/eng/maxmakelab/media/software-manual/color-panel.png" alt="Color Panel Interface" style="width: 300px; height: auto; border-radius: 8px;" />

#### Usage Instructions

- **Set Existing Element Color**: After selecting elements, click the color icon to set the selected element to that color
  <img src="/eng/maxmakelab/media/software-manual/color-panel-选图元设置颜色.gif" alt="Select Elements Set Color" style="width: 600px; height: auto; border-radius: 8px;" />

- **Set New Element Color**: After selecting a color, add elements, the added elements will be that color
  <img src="/eng/maxmakelab/media/software-manual/color-panel-选择颜色添加图元.gif" alt="Select Color Add Element" style="width: 600px; height: auto; border-radius: 8px;" />

- **Coordinate Display**: The coordinate display below shows the coordinate value where the current mouse pointer is located

---

## <a id="6-device-panel"></a>6. Device Panel

<img src="/eng/maxmakelab/media/software-manual/device-panel.png" alt="Device Panel Interface" style="width: 400px; height: auto; border-radius: 8px;" />

#### Connection and Control

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Mode Dropdown Option**</td>
      <td>Select equipment processing mode</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-模式下拉选项.gif" alt="Mode Dropdown Option" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Connection Icon**</td>
      <td>Connect or disconnect connection</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-连接图标.gif" alt="Connection Icon" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Select Device**</td>
      <td>Select device and load device parameters</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-选择设备.gif" alt="Select Device" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Device Settings**</td>
      <td>Supported setting options for that device</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-设备设置.gif" alt="Device Settings" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Help**</td>
      <td>Help options for that device</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-帮助.gif" alt="Help" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Quick Buttons**</td>
      <td>In laser, quick operation buttons supported by that device</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-快捷按钮.gif" alt="Quick Buttons" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="7-layer-panel"></a>7. Layer Panel

<img src="/eng/maxmakelab/media/software-manual/layer-panel.png" alt="Layer Panel Interface" style="width: 300px; height: auto; border-radius: 8px;" />

#### Function Description

- **Processing Parameters Setting**: In laser mode, display or set processing parameters for graphic elements of different colors
  <img src="/eng/maxmakelab/media/software-manual/layer-panel-设置加工参数.gif" alt="Layer Processing Parameters" style="width: 600px; height: auto; border-radius: 8px;" />

- **Layer Management**: Can move layer up, move layer down, delete layer

---

## <a id="8-toolpath-generation"></a>8. Toolpath Generation

<img src="/eng/maxmakelab/media/software-manual/toolpath-generation.png" alt="Toolpath Generation Interface" style="width: 250px; height: auto; border-radius: 8px;" />

#### Function List

| Function | Description |
|----------|-------------|
| **Set Blank** | Set blank size |
| **Tool Parameter Library** | Add tool parameter information |
| **Toolpath and Operations** | Contour milling, planar milling, V-type milling, drilling, relief, import toolpath programs |
| **Toolpath** | Display generated toolpaths |

---

## <a id="9-cnc-processing-workflow"></a>9. CNC Processing Workflow

<img src="/eng/maxmakelab/media/software-manual/cnc-workflow.png" alt="CNC Workflow Interface" style="width: 600px; height: auto; border-radius: 8px;" />

#### Status and Control

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Status Bar**</td>
      <td>Display workpiece coordinate system, machine coordinate system, safety door status, modal information</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-状态栏.png" alt="Status Bar" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Step Control**</td>
      <td>Control movement of XYZA axis, can set step size, feed rate</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-单步控制.gif" alt="Step Control" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Spindle Switch**</td>
      <td>Can control spindle to turn on/off according to set rotation speed</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-主轴开关.gif" alt="Spindle Switch" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Tool Change**</td>
      <td>Change tool and automatically measure tool height</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-换刀.gif" alt="Tool Change" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### Coordinate Settings

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Set XY0**</td>
      <td>Set current XY coordinates as XY zero point during processing</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-设置xy0.gif" alt="Set XY0" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Set Z0**</td>
      <td>Set current Z coordinates as Z zero point during processing</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-设置z0.gif" alt="Set Z0" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Move to XY Zero Point**</td>
      <td>Automatically raise to safety height, then move to XY zero point position</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-移动到xy零点.gif" alt="Move to XY Zero Point" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### File and Output

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**File**</td>
      <td>Select processing file</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-文件.gif" alt="File" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Console**</td>
      <td>Can manually or use macro buttons to send G-code</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-控制台.gif" alt="Console" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Gcode**</td>
      <td>Display loaded Gcode</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-gcode.gif" alt="Gcode" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Preview Simulation Area**</td>
      <td>Display 2D view or 3D simulation view of code</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-预览仿真区域.gif" alt="Preview Simulation Area" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### Other Operations

| Function | Description |
|----------|-------------|
| **Return to Zero** | Equipment returns to zero, must perform this operation after power-on before running equipment |
| **Border** | Spindle trial run processing range, note should manually raise spindle to safety height before clicking this button |
| **Reset** | Software system reset, terminate current operation and restore system initial state |
| **Unlock** | Release alarm lock state, restore axis movement permissions |
| **Restore** | Restore equipment Grbl configuration, can click to restore default values after modifying equipment $ parameters |

<img src="/eng/maxmakelab/media/software-manual/cnc-workflow-other.png" alt="Other Controls" style="width: 600px; height: auto; border-radius: 8px;" />

---

## <a id="10-laser-processing-workflow"></a>10. Laser Processing Workflow

<img src="/eng/maxmakelab/media/software-manual/laser-workflow.png" alt="Laser Workflow Interface" style="width: 600px; height: auto; border-radius: 8px;" />

> 📌 Laser processing workflow has the following main differences from CNC:

#### Unique Functions

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">Function</th>
      <th style="width: 20%;">Description</th>
      <th style="width: 70%;">Demo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Save Gcode**</td>
      <td>Save all current processing content to text format</td>
      <td><img src="/eng/maxmakelab/media/software-manual/laser-workflow-保存gcode.gif" alt="Save Gcode" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Activate Laser**</td>
      <td>After clicking, activate laser function and motor high-speed mode. Click again to exit laser function and restore motor normal mode</td>
      <td><img src="/eng/maxmakelab/media/software-manual/laser-workflow-激活激光.gif" alt="Activate Laser" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Start Position**</td>
      <td>Set processing start position</td>
      <td><img src="/eng/maxmakelab/media/software-manual/laser-workflow-开始位置.gif" alt="Start Position" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### Coordinate Mode

| Mode | Description |
|------|-------------|
| **Absolute Coordinate Mode** | Process based on mechanical coordinate position where graphics are located. Processing position changes with graphics |
| **Current Position Mode** | Process based on position where machine head is located. Processing position changes with machine head |

---

## Shortcut Reference

| Shortcut | Function |
|----------|----------|
| Ctrl + Z | Undo |
| Delete | Delete Selected Elements |
| Esc | Deselect |

---

