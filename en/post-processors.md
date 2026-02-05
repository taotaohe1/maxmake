# HiMill Series Post-Processors Download

This document provides download services for post-processors compatible with MAXMAKE HiMill series CNC machines. We will continuously add optimized post-processors for mainstream CAM software, with real-time updates available on this page.

## 3-Axis Post-Processors List

| Name | Compatible Software | Download Link |
|------|---------------------|---------------|
| Fusion360 Postprocessor | Autodesk Fusion 360 | <a href="/eng/himill-d1-d1s/media/post/fusion360.zip" target="_blank" rel="noopener noreferrer">Download</a> |
| Vectric Postprocessor | Vectric VCarve / Aspire / Cut2D | <a href="/eng/himill-d1-d1s/media/post/vectric.zip" target="_blank" rel="noopener noreferrer">Download</a> |
| Kiri:moto Postprocessor | Kiri:moto | <a href="/eng/himill-d1-d1s/media/post/kiri-moto.zip" target="_blank" rel="noopener noreferrer">Download</a> |
| Estlcam Postprocessor | Estlcam | <a href="/eng/himill-d1-d1s/media/post/estlcam-maxmake.zip" target="_blank" rel="noopener noreferrer">Download</a> |
| NX Postprocessor | Siemens NX | <a href="/eng/himill-d1-d1s/media/post/nx.zip" target="_blank" rel="noopener noreferrer">Download</a> · <a href="/en/himill-d1-d1s/hmd1-nx-postprocessor-installation.md" target="_blank" rel="noopener noreferrer">Installation Guide</a> |

## 4-Axis Post-Processors List

| Name | Compatible Software | Download Link |
|------|---------------------|---------------|
| Fusion360 4-Axis Postprocessor | Autodesk Fusion 360 | <a href="/eng/himill-d1-d1s/media/post/fusion360-4axis.zip" target="_blank" rel="noopener noreferrer">Download (Beta Version)</a> |
| Vectric 4-Axis Postprocessor | Vectric VCarve / Aspire / Cut2D | <a href="/eng/himill-d1-d1s/media/post/vectric-y2a.zip" target="_blank" rel="noopener noreferrer">Download</a> |

## Instructions

1. Download the post-processor compressed file corresponding to your CAM software
2. Extract the downloaded compressed file to obtain the post-processor file
3. Install the post-processor file according to the post-processor addition method for your CAM software
4. Select "MAXMAKE HiMill" post-processor when generating G-code
5. The generated G-code can be used directly with HiMill series machines

## Notes

The HiMill series machines have specific requirements for tool change commands:

- The machine **only supports** tool change commands in the format `T*M6`
- It **does not support** tool length compensation commands in the format `G43H**`

Therefore, when using **non-official post-processors** or **custom post-processors** (not provided on this page), please ensure to check the generated G-code:

1. Locate all tool change commands (`T*M6`)
2. Check if any `G43H**` commands follow these tool change commands
3. If such commands exist, manually delete them before using the G-code

G-code generated using the official post-processors provided on this page has been optimized for HiMill machines and requires no additional modifications.

### Semi-Automatic Tool Change Mechanism

HiMill series machines use a **semi-automatic tool change** system with the following characteristics:

- Although the G-code uses commands like `T1M6`, `T2M6`, `T3M6` to distinguish between different tools, the machine firmware's processing logic always treats them as a single tool
- After each tool change command, the machine automatically performs tool height measurement and adjusts the tool height compensation value based on the measurement result

#### Operation Rules

Please strictly follow these steps before processing to ensure correct tool compensation application:

1. First click the "Tool Change" button to enter tool change mode
2. Install the first tool and confirm
3. Wait for the machine to complete automatic height measurement
4. **After the height measurement is completed**, set the Z-axis zero point (Z0)

For detailed tool change operation procedures, please refer to the [Tool Installation Page](/en/himill-d1-d1s/hmd1-tool-installation.md).

