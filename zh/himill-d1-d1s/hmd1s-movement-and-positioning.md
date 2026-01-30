# MaxmakeLab 移动与定位


## CNC加工中的移动与定位

在加工前，一般需要确定加工原点。通过移动按钮控制主轴移动，移动到工件的加工原点后，再设置设备的加工原点。（由NC程序确定，比如NC程序中加工原点为中心点，那么就要找到工件的中心点，将工件的中心点设置为加工原点）

### 1. X轴移动控制

在移动控制中，点击此按钮，可以控制X轴左右移动。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向右移动.webp" alt="主轴向右移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向右移动.webp" alt="主轴向右移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向左移动.webp" alt="主轴向左移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向左移动.webp" alt="主轴向左移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. Y轴移动控制

点此按钮，可以控制Y轴前后移动。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-垫板向内移动.webp" alt="垫板向内移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-垫板向内移动.webp" alt="垫板向内移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-垫板向外移动.webp" alt="垫板向外移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-垫板向外移动.webp" alt="垫板向外移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

> ⚠️ **Y轴移动说明**：
> 
> 这里Y轴是底板移动，主轴是相对于底板的移动。所以点击向前移动时，是主轴相对的向前移动，Y轴底板向后移动
> 
> {.is-warning}

### 3. Z轴移动控制

点此按钮，可以控制Z轴上下移动。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向下移动.webp" alt="主轴向下移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向下移动.webp" alt="主轴向下移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向上移动.webp" alt="主轴向上移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向上移动.webp" alt="主轴向上移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 4. A轴（旋转轴）移动控制

点此按钮，可以控制A轴（旋转轴）移动。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/2-a轴移动.webp" alt="旋转轴移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 5. 步距和进给率设置

移动时，可设置步距和进给率。
- 步距：主轴每次移动的距离
- 进给率：主轴每次移动的速度（HiMill设备最大速度为1000mm/min，设置超过1000mm/min会按照1000mm/min运动）

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/3-设置步距和进给率.webp" alt="步距和进给率设置" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 6. 设置XY0点

当刀具移动至工件的中心时，点此按钮，可设置XY0点。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/4-设置xy0点.webp" alt="设置XY0点" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 7. 设置Z0点

当刀具刚刚接触工件时，点此按钮，可设置Z0点。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/4-设置z0点.webp" alt="设置Z0点" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## 激光加工中的移动与定位

### 1. 激光移动操作

在激光加工时，同样可以使用移动按钮移动至物体上方。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-2-激光移动界面截图.webp" alt="激光移动界面" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. 快速移动定位

也可以使用快速移动，左键点击画布中的位置，主轴就会移动到相应的坐标处。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-3-快速移动.webp" alt="快速移动定位" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 3. 激光边框定位

激活激光按钮打开后，点击边框按钮，激光会以弱光走出加工范围。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-4-激光激活+边框定位.webp" alt="激光激活+边框定位" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-5-拍摄边框定位.webp" alt="边框定位效果" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **激光边框定位注意事项**：
> 
> - 一般设置为当前位置，会以当前激光所在位置，试走出加工范围，便于随时调节；如果设置为绝对坐标，试走边框的范围会是固定的，需要调整加工材料的位置
> - 如果越界，界面会弹出越界提示，请向前调整主轴，再次试走边框
> - 因激光安装在主轴前侧，加工范围实际上向前移动了，必要时，需要打开安全门，防止材料撞到安全门上
> 
> {.is-warning}

### 4. 激光焦距调节

激光加工需要调节焦距，遮光罩底部到材料5mm为激光加工的最佳焦距位置。可以使用激光配件盒中的对焦辅助块，降下Z轴，直到对焦辅助块刚好能通过间隙。

<img src="/zh/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-6-对焦辅助片.webp" alt="对焦辅助片" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **激光焦距调节注意事项**：
> 
> 降下激光器时，尽量使用小步距慢移动，防止移动过快撞坏激光器
> 
> {.is-warning}