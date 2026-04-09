# MaxmakeLabの移動と位置決め

## CNC加工における移動と位置決め

加工前には、一般的に加工原点を決定する必要があります。移動ボタンを通じて主軸の移動を制御します。ワークピースの加工原点に移動した後、機器の加工原点を設定します。（NCプログラムによって決定されます。例えば、NCプログラムの加工原点が中心点である場合は、ワークピースの中心点を見つけて加工原点として設定します）

### 1. X軸の移動制御

移動制御では、このボタンをクリックするとX軸の左右の移動を制御することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向右移动.webp" alt="主軸が右に移動" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向右移动.webp" alt="主軸が右に移動" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向左移动.webp" alt="主軸が左に移動" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向左移动.webp" alt="主軸が左に移動" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. Y軸の移動制御

このボタンをクリックすると、Y軸の前後の移動を制御することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-垫板向内移动.webp" alt="ベースプレートが内側に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-垫板向内移动.webp" alt="ベースプレートが内側に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-垫板向外移动.webp" alt="ベースプレートが外側に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-垫板向外移动.webp" alt="ベースプレートが外側に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

> ⚠️ **Y軸の移動の注意事項**：
> 
> ここでのY軸はベースプレートの移動であり、主軸はベースプレートに対して移動します。したがって、前進ボタンをクリックすると、主軸が相対的に前進し、Y軸のベースプレートが後退します
> 
> {.is-warning}

### 3. Z軸の移動制御

このボタンをクリックすると、Z軸の上下の移動を制御することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向下移动.webp" alt="主軸が下に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向下移动.webp" alt="主軸が下に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-录屏-主轴向上移动.webp" alt="主軸が上に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/1-移动操作-拍摄-主轴向上移动.webp" alt="主軸が上に移动" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 4. A軸（回転軸）の移動制御

このボタンをクリックすると、A軸（回転軸）の移動を制御することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/2-a轴移动.webp" alt="回転軸の移动" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 5. ステップサイズと送り速度の設定

移動するときは、ステップサイズと送り速度を設定することができます。
- ステップサイズ：主軸が毎回移動する距離
- 送り速度：主軸が毎回移動する速度（HiMill機器の最大速度は1000mm/minで、1000mm/minを超える設定は1000mm/minで移動します）

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/3-设置步距和进给率.webp" alt="ステップサイズと送り速度の設定" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 6. XY0点の設定

工具がワークピースの中心に移動したとき、このボタンをクリックしてXY0点を設定します。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/4-设置xy0点.webp" alt="XY0点の設定" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 7. Z0点の設定

工具がワークピースに接触したとき、このボタンをクリックしてZ0点を設定します。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/4-设置z0点.webp" alt="Z0点の設定" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

---

## レーザー加工における移動と位置決め

### 1. レーザーの移動操作

レーザー加工中にも、移動ボタンを使用して物体の上に移動することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-2-激光移动界面截图.webp" alt="レーザーの移動インターフェース" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 2. クイック移動の位置決め

クイック移動を使用することもできます。キャンバス内の位置を左クリックすると、主軸が対応する座標位置に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-3-快速移动.webp" alt="クイック移動の位置決め" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 3. レーザーのボーダー位置決め

レーザーボタンを有効にした後、ボーダーボタンをクリックすると、レーザーが弱い光で加工範囲を歩きます。

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-4-激光激活+边框定位.webp" alt="レーザーの有効化 + ボーダーの位置決め" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-movement-and-positioning/5-5-拍摄边框定位.webp" alt="ボーダーの位置決めの効果" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **レーザーのボーダー位置決めの注意事項**：
> 
> - 一般的に現在の位置に設定し、現在のレーザー位置から加工範囲を歩いて随時調整しやすくします。絶対座標に設定すると、ボーダーの歩行範囲が固定され、加工材料の位置の調整が必要になります。
> - 範囲外になると、インターフェースに範囲外のプロンプトがポップアップします。主軸を前に移動して、再度ボーダーの歩行を試してください。
> - レーザーは主軸の前面に取り付けられているため、実際の加工範囲は前に移動します。必要に応じて安全ドアを開いて、材料が安全ドアにぶつからないようにしてください。
> 
> {.is-warning}