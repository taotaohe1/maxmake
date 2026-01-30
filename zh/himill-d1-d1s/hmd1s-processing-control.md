# MaxmakeLab CNC加工-导入NC程序的加工流程


## 1. 切换CNC模式

切换模式为CNC模式。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/1-切换cnc模式.webp" alt="切换CNC模式" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. 导入文件

连接设备后，导入准备好的NC程序。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/1-导入文件.webp" alt="导入文件" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. 移动定位

打开主轴，控制刀具移动到加工原点。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/2-转动主轴.webp" alt="转动主轴" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/2-移动到原点.webp" alt="移动到原点" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. 设置原点

以加工原点在工件中心点为例，刀具处于工件中心点时，点击设置XY0。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-刀具处于中心点.webp" alt="刀具处于中心点" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-设置xy0点.webp" alt="设置XY0点" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

慢慢降下Z轴，刀具刚刚接触到工件时，点击设置Z0。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-降z轴.webp" alt="降Z轴" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-设置z0点.webp" alt="设置Z0点" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. 预览仿真

在3D界面，可以预览仿真路径。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/4-预览仿真.webp" alt="预览仿真" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **预览仿真提示**：
> 
> - 可调节播放倍率，实时预览
> - 可直接拖动进度条
> 
> {.is-info}

## 6. 传输文件并开始加工

点击开始加工按钮，传输加工文件至设备SD卡。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/5-开始.webp" alt="开始加工" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

根据提示，等到指示灯显示彩虹旋转灯效时，长按设备按键2s，启动加工。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/5-接受文件开始加工.webp" alt="接受文件开始加工" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **加工控制注意事项**：
> 
> - 加工中，单击按键暂停加工。长按2s恢复加工
> - 如果启用了安全门功能，恢复加工前需关好门；如果未关门，长按2s后，也会显示恢复加工灯效，最后变为绿色常亮但设备无动作
> 
> {.is-warning}

## 7. 加工过程中参数调整

加工过程中，可更改进给率。

<img src="/chi/himill-d1-d1s/media/hmd1s-processing-control/6-覆写功能，更改转速进给率.webp" alt="覆写功能更改转速进给率" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **参数调整注意事项**：
> 
> - 加工过程中，不建议降低转速，尤其是金属加工，避免负载增大，导致断刀
> - 改变数值后，速度会慢慢增加或减少。需要根据实际情况，慢慢增加或减少数值
> 
> {.is-warning}