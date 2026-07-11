# MaxmakeLab CAM Feature Introduction

MaxmakeLAB version 0.9.18 introduces new CAM-related features: Stock Setup, Tool Library Management, three toolpath strategies (Profile Milling, Pocket Milling, Relief Toolpath), and Simulation. Here's an overview of each feature:

## 1. Stock Setup (Job Step)

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/毛坯设置.webp" alt="Stock Setup Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- Set stock dimensions (length, width, height)
- The machining origin currently defaults to the top vertex. Bottom origin functionality will be added in future updates
- Set origin position: center point or bottom-left corner
- Set machining safety height

## 2. Tool Library

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/刀具库.webp" alt="Tool Library Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- Modify tool parameters including:
  - Tool number, unit, diameter, etc.
  - Step down, step over, spindle speed, feed rate, plunge rate, etc.
- Add groups, add tools, copy/delete tools or groups

> ⚠️ **Notes**:
>
> - Import/export functionality is temporarily unavailable and will be fixed in future updates
> - Currently supports flat end mill, ball nose end mill, flat tip V-bit, and V-bit. Other tool types will be added in the future
> - Only one material type is currently displayed. More materials will be added later
>
> {.is-warning}

## 3. Profile Toolpath

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/轮廓铣.webp" alt="Profile Toolpath Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- Generate profile toolpath after selecting vectors
- Set machining depth. Machining start height will be added later
- Select tools from the tool library with support for temporary parameter modifications that do not affect the tool library
- Choose from three cutting modes: outside vector, on vector, inside vector
- Select climb or conventional milling
- Ramp and bridge features will be added in future updates

## 4. Pocket Toolpath

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/平面铣.webp" alt="Pocket Toolpath Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- Generate pocket toolpath after selecting vectors
- Set machining depth. Machining start height will be added later
- Select tools from the tool library with support for temporary parameter modifications that do not affect the tool library
- Ramp and rest machining features will be added in future updates

## 5. Relief Toolpath

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/浮雕加工.webp" alt="Relief Toolpath Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- Generate relief toolpath after selecting an image
- Set machining depth, which currently defines the relief height
- Select tools from the tool library with support for temporary parameter modifications that do not affect the tool library
- Defaults to roughing after offsetting from the graphic edge. Boundary limit options will be added later
- Ramp feature will be added in future updates

> ⚠️ **Notes**:
>
> - The relief feature currently reserves a large roughing allowance. It is not recommended for hard woods like sandalwood. This feature will be optimized in future updates
>
> {.is-warning}

## 6. Simulation

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/仿真加工.webp" alt="Simulation Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- After generating toolpath, click the simulate button to view the machining simulation
- Toggle toolpath display on/off
- Adjust playback speed and drag the progress bar for quick navigation
- There may be rendering issues when dragging the progress bar. This will be fixed in future updates

## 7. Export

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/导出.webp" alt="Export Demo" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- After generating toolpath, click the export button to export G-code in NC format
- Can directly import to the machine when connected and zeroed

> ⚠️ **Notes**:
>
> - Exported toolpaths are currently scattered. It is recommended not to modify them. This will be optimized in future updates
> - Since the code always contains tool change commands (T\*M6), you need to click tool change, measure tool height, set zero point, then run the code
>
> {.is-warning}

## 8. Feedback

If you encounter any software issues, please contact us in the Discord software feedback channel. We will actively consider your suggestions and fix issues promptly:

- [Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)