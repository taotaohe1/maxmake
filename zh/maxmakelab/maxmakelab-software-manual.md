# MaxmakeLab 软件说明书

## 目录

- [1. 主界面功能区介绍](#1-主界面功能区介绍)
- [2. 菜单栏](#2-菜单栏)
- [3. 设计栏](#3-设计栏)
- [4. 参数栏](#4-参数栏)
- [5. 颜色栏](#5-颜色栏)
- [6. 设备栏](#6-设备栏)
- [7. 图层栏](#7-图层栏)
- [8. 刀路生成](#8-刀路生成)
- [9. CNC加工流程](#9-cnc加工流程)
- [10. 激光加工流程](#10-激光加工流程)

---

## <a id="1-主界面功能区介绍"></a>1. 主界面功能区介绍

<div style="display: flex; gap: 16px; flex-wrap: wrap;">
  <img src="/zh/maxmakelab/media/software-manual/main-interface1.png" alt="主界面整体布局1" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
  <img src="/zh/maxmakelab/media/software-manual/main-interface2.png" alt="主界面整体布局2" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
</div>

#### 界面功能分区

| 区域 | 名称 | 功能描述 |
|------|------|----------|
| 1 | 菜单栏 | 导入导出文件，调整视图大小，软件设置，帮助引导，切换语言，切换模式 |
| 2 | 设计栏 | 添加各种类型的图元 |
| 3 | 画布 | 一般为设备幅面大小 |
| 4 | 颜色栏 | 给图元分配不同颜色 |
| 5 | 设备栏 | 选择、连接、快捷控制设备 |
| 6 | 参数设置 | CNC中为设置毛坯参数和刀具库参数 |
| 7 | 生成刀路 | 选择生成刀具路径的方式 |
| 8 | 刀具路径列表 | 显示已经生成的刀具路径 |
| 9 | 快捷控制 | 激光中为快捷控制功能，如快速移动、复位 |
| 10 | 图层栏 | 给不同颜色的图元分配不同的加工参数 |
| 11 | 仿真预览 | 仿真预览加工路径 |
| - | workflow | 点击进入加工预览界面 |

---

## <a id="2-菜单栏"></a>2. 菜单栏

<img src="/zh/maxmakelab/media/software-manual/menu-bar.png" alt="菜单栏界面" style="width: 200px; height: auto; border-radius: 8px;" />

#### 常用操作

| 功能 | 说明 |
|------|------|
| **下拉菜单** | 点击下拉列表选择具体操作 |
| <img src="/zh/maxmakelab/media/software-manual/dropdown-menu.png" alt="下拉菜单示例" style="width: 250px; height: auto; border-radius: 8px;" /> | |
| **保存** | 保存当前的项目 |
| **撤销** | 撤销上一步操作 |
| **重做** | 还原下一步操作 |

---

## <a id="3-设计栏"></a>3. 设计栏

<img src="/zh/maxmakelab/media/software-manual/design-panel.png" alt="设计栏界面" style="width: 40px; height: auto; border-radius: 8px;" />

#### 工具箱

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">工具</th>
      <th style="width: 10%;">功能说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Select 选择**</td>
      <td>进入选择模式，可选择图元，移动图元</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-Select.gif" alt="Select选择" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Image 图片**</td>
      <td>插入图片，支持png，jpg，jpeg格式</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-image.gif" alt="Image图片" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Basic 基础图元**</td>
      <td>添加直线，正方形，圆形</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-basic.gif" alt="Basic基础图元" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Text 文本**</td>
      <td>添加文本</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-text.gif" alt="Text文本" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Pen 钢笔工具**</td>
      <td>添加贝塞尔曲线</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-pen.gif" alt="Pen钢笔工具" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Node 节点编辑**</td>
      <td>节点编辑工具</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-node.gif" alt="Node节点编辑" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Offset 偏移工具**</td>
      <td>偏移出当前图形的内外轮廓</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-offset.gif" alt="Offset偏移工具" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Clipart 图形库**</td>
      <td>添加各种类别的图形</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-offset-clipart.gif" alt="Clipart图形库" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Plugin 扩展**</td>
      <td>包含盒子生成，齿轮生成</td>
      <td><img src="/zh/maxmakelab/media/software-manual/design-panel-plugin.gif" alt="Plugin扩展" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="4-参数栏"></a>4. 参数栏

<img src="/zh/maxmakelab/media/software-manual/parameter-panel.png" alt="参数栏界面" style="width: 600px; height: auto; border-radius: 8px;" />

> 💡 参数栏在选择图形后显示，取消选择后隐藏

#### 基础变换

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**点坐标**</td>
      <td>选择不同点位，显示或者设置当前点位的坐标值</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-点坐标.gif" alt="点坐标" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**宽高度**</td>
      <td>显示或者设置当前图元的宽度和高度</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-宽高度.gif" alt="宽高度" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**锁定**</td>
      <td>锁定或者解锁图形比例</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-锁定.gif" alt="锁定" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**旋转角度**</td>
      <td>设置图元的旋转角度</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-旋转角度.gif" alt="旋转角度" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**水平镜像**</td>
      <td>水平反转图元</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-水平镜像.gif" alt="水平镜像" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**垂直镜像**</td>
      <td>垂直翻转图元</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-垂直镜像.gif" alt="垂直镜像" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 排列工具

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**对齐**</td>
      <td>左对齐，右对齐，水平居中对齐，顶部对齐，底部对齐，垂直居中对齐</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-对齐.gif" alt="对齐" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**分布**</td>
      <td>水平间隔分布，垂直间隔分布</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-分布.gif" alt="分布" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 阵列工具

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**矩形阵列**</td>
      <td>以矩形阵列的方式快速添加图元</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-矩形阵列.gif" alt="矩形阵列" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**环形阵列**</td>
      <td>以环形阵列的方式快速添加图元</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-环形阵列.gif" alt="环形阵列" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**布尔运算**</td>
      <td>对两个及以上图元对象进行相加、相减、相交或排除重叠等操作，生成新图元</td>
      <td><img src="/zh/maxmakelab/media/software-manual/parameter-panel-布尔运算.gif" alt="布尔运算" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="5-颜色栏"></a>5. 颜色栏

<img src="/zh/maxmakelab/media/software-manual/color-panel.png" alt="颜色栏界面" style="width: 300px; height: auto; border-radius: 8px;" />

#### 使用说明

- **设置已有图元颜色**：选择图元后，点击颜色图标，可将选择的图元设置为该颜色
  <img src="/zh/maxmakelab/media/software-manual/color-panel-选图元设置颜色.gif" alt="选图元设置颜色" style="width: 600px; height: auto; border-radius: 8px;" />

- **设置新图元颜色**：选择颜色后，添加图元，添加的图元为该颜色
  <img src="/zh/maxmakelab/media/software-manual/color-panel-选择颜色添加图元.gif" alt="选图元设置颜色" style="width: 600px; height: auto; border-radius: 8px;" />

- **坐标显示**：下方坐标显示当前鼠标指针所在的坐标值

---

## <a id="6-设备栏"></a>6. 设备栏

<img src="/zh/maxmakelab/media/software-manual/device-panel.png" alt="设备栏界面" style="width: 400px; height: auto; border-radius: 8px;" />

#### 连接与控制

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**模式下拉选项**</td>
      <td>选择设备的加工模式</td>
      <td><img src="/zh/maxmakelab/media/software-manual/device-panel-模式下拉选项.gif" alt="模式下拉选项" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**连接图标**</td>
      <td>连接或者断开连接</td>
      <td><img src="/zh/maxmakelab/media/software-manual/device-panel-连接图标.gif" alt="连接图标" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**选择设备**</td>
      <td>选择设备并加载该设备的参数</td>
      <td><img src="/zh/maxmakelab/media/software-manual/device-panel-选择设备.gif" alt="选择设备" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**设备设置**</td>
      <td>该设备支持的设置选项</td>
      <td><img src="/zh/maxmakelab/media/software-manual/device-panel-设备设置.gif" alt="设备设置" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**帮助**</td>
      <td>该设备的帮助选项</td>
      <td><img src="/zh/maxmakelab/media/software-manual/device-panel-帮助.gif" alt="帮助" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**快捷按钮**</td>
      <td>激光中为该设备支持的快捷操作按钮</td>
      <td><img src="/zh/maxmakelab/media/software-manual/device-panel-快捷按钮.gif" alt="快捷按钮" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="7-图层栏"></a>7. 图层栏

<img src="/zh/maxmakelab/media/software-manual/layer-panel.png" alt="图层栏界面" style="width: 300px; height: auto; border-radius: 8px;" />

#### 功能说明

- **加工参数设置**：激光模式下，可显示或者设置不同颜色图元的加工参数
  <img src="/zh/maxmakelab/media/software-manual/layer-panel-设置加工参数.gif" alt="图层加工参数" style="width: 600px; height: auto; border-radius: 8px;" />

- **图层管理**：可上移图层，下移图层，删除图层

---

## <a id="8-刀路生成"></a>8. 刀路生成

<img src="/zh/maxmakelab/media/software-manual/toolpath-generation.png" alt="刀路生成界面" style="width: 250px; height: auto; border-radius: 8px;" />

#### 功能列表

| 功能 | 说明 |
|------|------|
| **设置毛坯** | 设置毛坯的尺寸 |
| **刀具参数库** | 添加刀具参数信息 |
| **刀具路径及操作** | 轮廓铣，平面铣，V型铣，钻孔，浮雕，导入刀路程序 |
| **刀具路径** | 显示已生成的刀具路径 |

---

## <a id="9-cnc加工流程"></a>9. CNC加工流程

<img src="/zh/maxmakelab/media/software-manual/cnc-workflow.png" alt="CNC workflow界面" style="width: 600px; height: auto; border-radius: 8px;" />

#### 状态与控制

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**状态栏**</td>
      <td>显示工件坐标系，机床坐标系，安全门状态，模态信息</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-状态栏.png" alt="状态栏" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**单步控制**</td>
      <td>控制XYZA轴的移动，可设置步距，进给率</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-单步控制.gif" alt="单步控制" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**主轴开关**</td>
      <td>可控制主轴按照设定的转速开关</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-主轴开关.gif" alt="主轴开关" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**换刀**</td>
      <td>换刀并自动测量刀具的高度</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-换刀.gif" alt="换刀" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 坐标设置

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**设置XY0**</td>
      <td>设置当前XY坐标为加工时的XY零点</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-设置xy0.gif" alt="设置XY0" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**设置Z0**</td>
      <td>设置当前Z坐标为加工时的Z零点</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-设置z0.gif" alt="设置Z0" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**移动到XY零点**</td>
      <td>自动抬升至安全高度后，移动到XY零点的位置</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-移动到xy零点.gif" alt="移动到XY零点" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 文件与输出

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**文件**</td>
      <td>选择加工文件</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-文件.gif" alt="文件" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**控制台**</td>
      <td>可手动或运用宏按钮，发送G代码</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-控制台.gif" alt="控制台" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Gcode**</td>
      <td>显示加载的Gcode</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-gcode.gif" alt="Gcode" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**预览仿真区域**</td>
      <td>显示代码的2D视图或3D仿真视图</td>
      <td><img src="/zh/maxmakelab/media/software-manual/cnc-workflow-预览仿真区域.gif" alt="预览仿真区域" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 其他操作

| 功能 | 说明 |
|------|------|
| **回零** | 设备回零，开机后必须执行此操作才可运行设备 |
| **边框** | 主轴试走加工范围，注意应手动上升主轴至安全高度后，再点击此按钮 |
| **重置** | 软件系统复位，终止当前操作并回复系统初始状态 |
| **解锁** | 解除报警锁定状态，恢复轴的运动权限 |
| **恢复** | 恢复设备的Grbl配置，在修改设备$参数后可以点击恢复默认值 |

<img src="/zh/maxmakelab/media/software-manual/cnc-workflow-other.png" alt="其他控制功能" style="width: 600px; height: auto; border-radius: 8px;" />

---

## <a id="10-激光加工流程"></a>10. 激光加工流程

<img src="/zh/maxmakelab/media/software-manual/laser-workflow.png" alt="激光workflow界面" style="width: 600px; height: auto; border-radius: 8px;" />

> 📌 激光加工流程与CNC有以下主要区别：

#### 特有功能

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">功能</th>
      <th style="width: 10%;">说明</th>
      <th style="width: 80%;">演示</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**保存Gcode**</td>
      <td>保存当前所有加工内容到文本格式</td>
      <td><img src="/zh/maxmakelab/media/software-manual/laser-workflow-保存gcode.gif" alt="保存Gcode" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**激活激光**</td>
      <td>点击后，激活激光功能和电机的高速模式。再次点击退出激光功能和恢复电机正常模式</td>
      <td><img src="/zh/maxmakelab/media/software-manual/laser-workflow-激活激光.gif" alt="激活激光" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**开始位置**</td>
      <td>设置加工开始的位置</td>
      <td><img src="/zh/maxmakelab/media/software-manual/laser-workflow-开始位置.gif" alt="开始位置" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 坐标模式

| 模式 | 说明 |
|------|------|
| **绝对坐标模式** | 以图形所在的机械坐标位置加工，加工位置随着图形变化 |
| **当前位置模式** | 以机头所在位置进行加工，加工位置随着机头变化 |

---

## 快捷键参考

| 快捷键 | 功能 |
|--------|------|
| Ctrl + Z | 撤销 |
| Delete | 删除选中图元 |
| Esc | 取消选择 |

---

