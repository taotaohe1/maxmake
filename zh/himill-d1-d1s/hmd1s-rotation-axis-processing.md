# MaxmakeLab 旋转轴加工-导入NC程序的加工流程

## 1. 切换为CNC模式

切换模式为CNC模式。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/1-切换cnc模式.webp" alt="切换CNC模式" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. 导入文件

连接设备后，导入准备好的NC程序。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/1-导入文件.webp" alt="导入文件" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. 上调主轴

因旋转轴本身高度较高，可能需要上调主轴。松开主轴的4颗固定螺丝，上移后重新固定。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/2-上调主轴.webp" alt="上调主轴" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. 移动定位

打开主轴，控制刀具移动到加工原点。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/3-移动定位-打开主轴.webp" alt="打开主轴" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/3-移动定位-移动.webp" alt="移动" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. 设置原点

刀具位于加工原点时，点击设置XY0。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-1-刀具位于原点时.webp" alt="刀具位于原点时" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-1-设置xy0点.webp" alt="设置XY0点" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

慢慢降下Z轴，刀具刚刚接触到工件时，点击设置Z0。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-2-降下z轴.webp" alt="降下Z轴" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-2-设置z0点.webp" alt="设置Z0点" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **设置原点注意事项**：
> 
> - 此案例中，NC程序的Z0位于方形工件的角边，所以设置Z0时需要将角调整至正上方
> - 旋转轴加工前，在设计刀路时，建议先装夹工件。一定要考虑好装夹的位置，生成的刀具路径需避开爪盘，避免撞击
> - 同时需提前确定好加工的Z轴范围，提前算好刀具长度，避免刀具不够长，导致无法加工
> 
> {.is-warning}

## 6. 预览仿真

在3D界面，可以预览仿真路径。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/5-预览仿真.webp" alt="预览仿真" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **预览仿真提示**：
> 
> - 可调节播放倍率，实时预览
> - 可直接拖动进度条
> 
> {.is-info}

## 7. 传输文件并开始加工

点击开始加工按钮，传输加工文件至设备SD卡。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/6-点击开始.webp" alt="点击开始" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

根据提示，等到指示灯显示彩虹旋转灯效时，长按设备按键2s，启动加工。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/6-接受文件开始加工.webp" alt="接受文件开始加工" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **加工控制注意事项**：
> 
> - 加工中，单击按键暂停加工。长按2s恢复加工
> - 如果启用了安全门功能，恢复加工前需关好门
> 
> {.is-warning}

## 8. 加工过程中，可更改转速和进给率

加工过程中，可更改转速和进给率。

<img src="/zh/himill-d1-d1s/media/hmd1s-rotation-axis-processing/7-覆写功能.webp" alt="覆写功能" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **参数调整注意事项**：
> 
> - 加工过程中，不建议降低转速，尤其是金属加工，避免负载增大，导致断刀
> - 改变数值后，速度会慢慢增加或减少。需要根据实际情况，慢慢增加或减少数值
> 
> {.is-warning}