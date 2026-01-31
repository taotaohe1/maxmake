# MaxmakeLab 3D测头使用
## 1. 安装3D测头

在安装好3D测头后，软件中切换为对刀（3D 测头）界面。需点击"换刀"按钮，等待3D测头正常测高完成后，才能执行后续操作。

点击"换刀"按钮：

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-换刀-01-录屏换刀.gif" alt="换刀" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

安装3D测头，单击按键后，并完成自动自动测高(D1设备的换刀请遵循D1的换刀流程，使用扳手取下螺帽，将3D测头安装在筒夹中，再用扳手拧紧螺帽)

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-组装-02-组装测头.webp" alt="组装3D测头" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-测高-03-完成测高.webp" alt="完成自动测高" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **换刀操作注意事项**：
> 
> - 如果工件较高，必要时请向上调节主轴高度
> - 如果需使用3D测头自动设置Z0，此步骤必须执行完成，否则后续刀具补偿会出错。使用完成后，需要点击换刀，更换刀具并自动测量刀具高度后再加工
> - 如果只用来分中或角点探测（设置XY0），可不执行此步骤，但更换第一把刀仍需要点击换刀后，完成自动测高。再去手动设置Z0
> - 在插入3D测头后，禁止打开主轴，否则会造成3D测头损坏！！！ 
> 
> {.is-warning}

## 2. 界面按钮功能介绍

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/0-界面-按钮-00-界面功能.jpg" alt="界面按钮功能" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

控制：
- 换刀：安装前需点击并安装3D测头，测量完后需点击并更换为加工的刀具
- 设置XY0：将当前位置设置为XY0点，手动设置时使用。如果使用自动分中请忽略
- 设置Z0：将当前位置设置为Z0点，手动设置时使用。如果使用自动分中请忽略

移动到位置：中心点X，中心点Y，中心点XY。
- 使用3D测头设置好XY0后，对应的图标会被点亮，点击后，会自动前往设置好的X0或Y0位置（同样适用于角探测）。

对刀设置：
- 对刀距离：探测时会移动此处设置的距离，如果在设定的距离内未探测到工件，会弹窗提示
- 对刀速度：探测时会以此处设置的速度移动。
- 球头半径：测头的球头半径。此处为默认值，无更改

## 3. 角点探测

软件中选择角点探测，可以探测材料的角点位置，并自动将角点设置为XY0。以左下角为例。

### X轴探测

使用移动功能，将3D测头移动至工件左侧。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-x轴-移动-01-移动到工件左侧.jpg" alt="x轴移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击检测，探测到工件后，会自动将探测到的位置设置成X0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-x轴-探测-02-x轴探测截图.jpg" alt="x轴探测截图" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-x轴-探测-03-x轴探测过程.webp" alt="x轴探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y轴探测

使用移动功能，将测头移动至工件前侧。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-y轴-移动-01-移动到工件前侧.webp" alt="y轴移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击检测，探测到工件后，会自动将探测到的位置设置成Y0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-y轴-探测-02-y轴探测结果.jpg" alt="y轴探测" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-y轴-探测-03-y轴探测过程.webp" alt="y轴探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Z轴探测

使用移动功能，将3D测头移动至工件上方。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-z轴-移动-01-移动到工件上方.webp" alt="z轴移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击Z平面检测，探测到工件后，会自动将探测到的位置设置成Z0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-z轴-探测-02-z轴探测成功.jpg" alt="z轴探测成功" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-z轴-探测-03-z轴探测过程.webp" alt="z轴探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 更换刀具

全部设置完成后，需点击换刀，更换需要使用的第一把刀具，并完成自动测高。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="点击换刀" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/d1换刀.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. 矩形外部分中

软件中选择矩形外部分中，可以探测并自动计算中点位置，需手动设置探测的中点为XY0点。

### X轴左侧探测

使用移动功能，将3D测头移动至工件左侧。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x左-移动-01-移动到工件左侧.jpg" alt="x轴左侧移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

并点击检测，等待探测结束。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x左-探测-02-左侧探测成功.jpg" alt="x轴左侧探测成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x左-探测-03-左侧探测过程.webp" alt="x轴左侧探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### X轴右侧探测

探测到工件后，手动上升Z轴至安全高度后，移动至工件右侧。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-移动-01-移动到工件右侧.webp" alt="x轴右侧移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击检测，等待探测结束。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-探测-02-右侧探测成功.jpg" alt="x轴右侧探测成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-探测-03-右侧探测过程.webp" alt="x轴右侧探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

探测到工件后，会得到工件两侧的X坐标，点击下方的Zero X，自动计算中点，并将中点设置为X0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-分中-04-点击x轴分中.jpg" alt="点击分中" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y轴探测

同样方法探测工件的前后侧，点击Zero Y，自动计算中点，并将中点设置为Y0。

### Z轴探测

使用移动功能，将3D测头移动至工件上方。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-z轴-移动-01-移动到工件上方.webp" alt="z轴移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击Z平面检测，等待探测结束。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-z轴-探测-02-z轴探测成功.jpg" alt="z轴探测成功" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

探测到工件后，会自动将探测到的位置设置成Z0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-z轴-探测-03-z轴探测过程.webp" alt="z轴探测过程" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 更换刀具

全部设置完成后，需点击换刀，更换需要使用的第一把刀具，并完成自动测高。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="点击换刀" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/d1换刀.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **矩形外部分中注意事项**：
> 
> 圆形外部分中和矩形外部分中操作类似。但需注意，探测X中点时，Y轴坐标不能更改。探测Y中点时，X轴坐标不能更改。如：探测X左侧后，上升Z轴，再移动到X右侧，期间Y轴不能移动。
> 
> {.is-warning}

## 5. 圆形内部分中

软件中选择圆形内部分中，可以探测并自动计算中点位置，需手动设置探测的中点为XY0点。

### X轴左侧探测

使用移动功能，将测头移动至工件内部，接近工件内部左侧。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x左-移动-01-移动到内部左侧.webp" alt="x轴左侧移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击向左检测，等待探测结束。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x左-探测-02-内部左侧探测成功.jpg" alt="x轴左侧探测成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x左-探测-03-内部左侧探测过程.webp" alt="x轴左侧探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### X轴右侧探测

探测到工件后，移动接近工件右侧（期间请勿移动Y轴）。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-移动-01-移动到内部右侧.webp" alt="x轴右侧移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

点击向右检测，等待探测结束。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-探测-02-内部右侧探测成功.jpg" alt="x轴右侧探测成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-探测-03-内部右侧探测过程.webp" alt="x轴右侧探测过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

探测到工件后，会得到工件内部两侧的X坐标，点击下方的Zero X，自动计算中点，并将中点设置为X0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-分中-04-点击x轴分中.jpg" alt="点击分中" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y轴探测

同样方法探测工件内部前后侧，点击Zero Y，自动计算中点，并将中点设置为Y0。


### Z轴探测

使用移动功能，将3D测头移动至工件上方。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-z轴-移动-01-移动到工件上方.webp" alt="z轴移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

并点击Z平面检测，等待探测结束。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-z轴-探测-02-z轴探测成功.jpg" alt="z轴探测成功" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

探测到工件后，会自动将探测到的位置设置成Z0。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-z轴-探测-03-z轴探测过程.webp" alt="z轴探测过程" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 更换刀具

D1S：全部设置完成后，需点击换刀，更换需要使用的第一把刀具，并完成自动测高。

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="点击换刀" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/chi/himill-d1-d1s/media/hmd1s-3d-probe-using/d1换刀.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **分中操作提示**：
> 
> 矩形内部分中和圆形内部分中操作类似。
> 
> {.is-info}

## 注意事项

> ⚠️ **3D测头使用安全注意事项**：
>
> - 分中适用于规则形状的工件，比如圆形或矩形。不建议在不规则工件上使用
> - Z轴表面探测时，应选择工件的最高面
> - 移动3D测头时，使球头部分略低于工件，不要过低
> - 提前观察有无物体可能阻碍3D测头移动，避免探针还未接触时，3D测头受到撞击损坏
> - 3D测头属于精密易损配件，移动3D测头时，请慢速移动
> - 如果移动过程中误触会报警，请及时移开障碍物，回零并重试
>
> {.is-warning}

## 6. 高度图功能

3D测头还可以用于高度图功能，通过探测工件表面的高度变化，自动调整加工路径，获得更精准的加工效果。

- [MaxmakeLAB 3D测头高度图功能](/zh/himill-d1-d1s/hmd1s-height-map.md)