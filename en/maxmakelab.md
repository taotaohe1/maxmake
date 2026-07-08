# MaxmakeLab Software: HiMill CNC Control & Design Tool

MaxmakeLab is the official control software for [MAXMAKE HiMill D1/D1S](https://www.maxmake.com/products) CNC machines. This page provides quick access to installation guides, feature introductions, software manuals, and safety information for CNC and laser processing.

<img src="/eng/himill-d1-d1s/media/icon/maxmakelab.png" alt="MaxmakeLab Main Interface" style="width: 100px; height: auto; margin-bottom: 8px; border-radius: 6px;" />


## Quick Start
Necessary and simple operation steps to help you quickly get started with MaxmakeLab.
* [MaxmakeLab Software Installation Guide](/en/maxmakelab/maxmakelab-installation.md)

## Software Features
Detailed introduction to the core functions and features of MaxmakeLab.
* [MaxmakeLab Software Introduction](/en/maxmakelab/maxmakelab-introduction.md)

## Software Operations
Detailed operation instructions for MaxmakeLab software to help you use it correctly.
* [MaxmakeLab Software Manual](/en/maxmakelab/maxmakelab-software-manual.md)

## Related Resources
If you want to learn more about MaxmakeLab's features, you can refer to:
- [HiMill D1S Processing Control](/en/himill-d1-d1s/hmd1s-processing-control.md)
- [HiMill D1S Laser Processing](/en/himill-d1-d1s/hmd1s-laser-processing.md)

## Community Support
If you encounter any issues while using the software, please click this link to join our Discord and create a ticket for help:
- [Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)

---

## ⚠️ Important Safety Notice

> **We strongly recommend using MaxmakeLab software for processing control**
>
> **Reasons**: Our MaxmakeLab software is specifically developed for our equipment, with safety optimizations for various operating scenarios, such as:
>
> - When encountering tool change commands like T*M6, it automatically stops sending subsequent codes to ensure the safety of tool change operations (avoiding issues like spindle not stopping that may occur with other software)
> - Optimized for the equipment's motion characteristics to ensure smoothness and precision during processing
> - Built-in safety protection mechanisms to effectively prevent equipment damage caused by abnormal operations
> - Fully compatible with equipment hardware, avoiding various abnormal behaviors caused by software incompatibility
>
> **Using other control software may lead to unknown abnormal behaviors, and could even cause equipment damage or personal injury. For your safety and the normal operation of the equipment, we recommend always using MaxmakeLab software for processing control.**
> {.is-warning}