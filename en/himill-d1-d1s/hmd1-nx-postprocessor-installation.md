# HiMill NX Post-Processor Installation Guide: Siemens NX Setup Tutorial

Learn how to install the HiMill post-processor for Siemens NX software. This comprehensive guide covers file extraction, directory setup, template configuration, and verification steps.

---

## 📋 Installation Steps

### Step 1: Extract Post-Processor Files

1. Download the NX post-processor package from the [Post-Processors Download Page](/en/post-processors.md)
2. Extract the compressed package, you will get 3 files

<img src="/eng/himill-d1-d1s/media/post/1解压.png" alt="Extract post-processor files" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 2: Copy Post-Processor Files to NX Installation Directory

1. Open the installation path of Siemens NX software
2. Find the default installation location of post-processors:
   ```
   X:\Program Files\Siemens\NX 12.0\MACH\resource\postprocessor
   ```
   *Note: X represents the drive letter where you installed NX software, and 12.0 represents your NX software version*
3. Paste the 3 extracted post-processor files into this directory

<img src="/eng/himill-d1-d1s/media/post/2复制.png" alt="Copy post-processor files" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 3: Edit template_post.dat File

1. Find and right-click the `template_post.dat` file in the postprocessor directory
2. Select "Open with" → "Notepad"

<img src="/eng/himill-d1-d1s/media/post/3添加命令.png" alt="Edit template_post.dat file" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Step 4: Add Post-Processor Configuration

1. Add a new line at the end of the `template_post.dat` file
2. Paste the following content:
   ```
   HiMill,${UGII_CAM_POST_DIR}HiMill.tcl,${UGII_CAM_POST_DIR}HiMill.def
   ```
3. Save and close the file

---

## ✅ Verify Installation

After completing the above steps, you can select the "HiMill" post-processor from the post-processor list in NX software to generate G-code suitable for HiMill series machines.

---

## 💡 Notes

- Ensure you are using a post-processor compatible with your NX software version
- If you have modified the default installation path of NX software, please operate according to the actual path
- Make sure NX software is not running when installing the post-processor to avoid file occupation

---

## 🔗 Related Links

- [Post-Processors Download Page](/en/post-processors.md)
- [HiMill Series Machine Usage Guide](/en/himill-d1-d1s/hmd1-first-use.md)