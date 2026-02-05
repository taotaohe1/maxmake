# NX 后处理器安装教程

本文档提供了在 Siemens NX 软件中安装 HiMill 系列设备后处理器的详细步骤。

---

## 📋 安装步骤

### 步骤 1：解压后处理器文件

1. 从 [后处理器下载页面](/zh/post-processors.md) 下载 NX 后处理器压缩包
2. 解压压缩包，您将得到 3 个文件

<img src="/chi/himill-d1-d1s/media/post/1解压.png" alt="解压后处理器文件" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤 2：复制后处理器文件到 NX 安装目录

1. 打开 Siemens NX 软件的安装路径
2. 找到后处理器的默认安装位置：
   ```
   X:\Program Files\Siemens\NX 12.0\MACH\resource\postprocessor
   ```
   *注：X 代表您安装 NX 软件的盘符，12.0 代表您的 NX 软件版本号*
3. 将解压得到的 3 个后处理器文件粘贴到该目录

<img src="/chi/himill-d1-d1s/media/post/2复制.png" alt="复制后处理器文件" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤 3：编辑 template_post.dat 文件

1. 在 postprocessor 目录下找到并右键点击 `template_post.dat` 文件
2. 选择「打开方式」→「记事本」

<img src="/chi/himill-d1-d1s/media/post/3添加命令.png" alt="编辑template_post.dat文件" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 步骤 4：添加后处理器配置

1. 在 `template_post.dat` 文件的末尾添加新的一行
2. 粘贴以下内容：
   ```
   HiMill,${UGII_CAM_POST_DIR}HiMill.tcl,${UGII_CAM_POST_DIR}HiMill.def
   ```
3. 保存并关闭文件

---

## ✅ 验证安装

完成以上步骤后，您可以在 NX 软件的后处理器列表中选择「HiMill」后处理器来生成适用于 HiMill 系列设备的 G 代码。

---

## 💡 注意事项

- 确保您使用的是与您的 NX 软件版本兼容的后处理器
- 如果您修改了 NX 软件的默认安装路径，请根据实际路径进行操作
- 安装后处理器时请确保 NX 软件未运行，以避免文件被占用

---

## 🔗 相关链接

- [后处理器下载页面](/zh/post-processors.md)
- [HiMill 系列设备使用指南](/zh/himill-d1-d1s/hmd1-first-use.md)