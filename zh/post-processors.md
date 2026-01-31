# HiMill 系列后处理器下载

本文档提供 MAXMAKE HiMill 系列 CNC 设备兼容的后处理器下载服务。我们将持续添加主流 CAM 软件的适配后处理器，并在本页面实时更新。

## 三轴后处理器列表

| 名称 | 适用软件 | 下载链接 |
|------|----------|----------|
| Fusion360 后处理器 | Autodesk Fusion 360 | <a href="/chi/himill-d1-d1s/media/post/fusion360.zip" target="_blank" rel="noopener noreferrer">下载</a> |
| Vectric 后处理器 | Vectric VCarve / Aspire / Cut2D | <a href="/chi/himill-d1-d1s/media/post/vectric.zip" target="_blank" rel="noopener noreferrer">下载</a> |
| Kiri:moto 后处理器 | Kiri:moto | <a href="/chi/himill-d1-d1s/media/post/kiri-moto.zip" target="_blank" rel="noopener noreferrer">下载</a> |
| Estlcam 后处理器 | Estlcam | <a href="/chi/himill-d1-d1s/media/post/estlcam-maxmake.zip" target="_blank" rel="noopener noreferrer">下载</a> |

## 四轴后处理器列表

| 名称 | 适用软件 | 下载链接 |
|------|----------|----------|
| Fusion360 四轴后处理器 | Autodesk Fusion 360 | <a href="/chi/himill-d1-d1s/media/post/fusion360-4axis.zip" target="_blank" rel="noopener noreferrer">下载（测试版本）</a> |
| Vectric 四轴后处理器 | Vectric VCarve / Aspire / Cut2D | <a href="/chi/himill-d1-d1s/media/post/vectric-y2a.zip" target="_blank" rel="noopener noreferrer">下载</a> |

## 使用说明

1. 下载与您使用的 CAM 软件对应的后处理器压缩文件
2. 解压下载的压缩文件，获取后处理器文件
3. 按照对应 CAM 软件的后处理器添加方式进行安装
4. 生成 G 代码时选择「MAXMAKE HiMill」后处理器
5. 生成的 G 代码可直接用于 HiMill 系列设备

## 注意事项

HiMill 系列设备的换刀机制具有特定要求：

- 设备换刀时**仅支持** `T*M6` 格式的换刀代码
- **不支持** `G43H**` 格式的刀具补偿代码

因此，当您使用**非本页面提供的后处理器**或**自定义后处理器**时，请务必检查生成的 G 代码：

1. 找到所有换刀指令（`T*M6`）
2. 检查换刀指令后是否跟随 `G43H**` 类代码
3. 若存在此类代码，请手动删除后再使用 G 代码

使用本页面提供的官方后处理器生成的 G 代码已针对 HiMill 设备优化，无需额外修改。

### 半自动换刀机制说明

HiMill 系列设备采用**半自动换刀**方式，具有以下特点：

- 尽管 G 代码中使用 `T1M6`、`T2M6`、`T3M6` 等指令区分不同刀具，但设备固件的处理逻辑始终视为同一把刀具在工作
- 每次执行换刀指令后，设备会自动进行刀具测高，并根据测高结果调整刀具高度补偿值

#### 操作规则

加工前请严格遵循以下步骤，以确保刀具补偿应用正确：

1. 首先点击「换刀」按钮，进入换刀模式
2. 安装第一把刀具并确认
3. 等待设备完成自动测高
4. **测高完成后**，再设置 Z 轴零点（Z0）

关于详细的换刀操作流程，请参考 [刀具安装页面](/zh/himill-d1-d1s/hmd1-tool-installation.md)。
