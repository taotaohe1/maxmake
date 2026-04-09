# MaxmakeLab 3Dプローブの使用方法

## 注意事項

> ⚠️ **3Dプローブ使用の安全注意事項**：
>
> - センタリングは、円や長方形などの規則的な形状のワークピースに適しています。不規則な形状のワークピースには推奨されません
> - Z軸表面検出時には、ワークピースの最も高い表面を選択してください
> - 3Dプローブを移動するときは、ボール先端をワークピースの少し下に保ち、低すぎないようにしてください
> - 3Dプローブの移動を妨げる可能性のある物体があるかどうか事前に確認し、プローブが接触する前に3Dプローブが衝突して損傷するのを避けてください
> - 3Dプローブは精密かつ損傷しやすいアクセサリーですので、3Dプローブをゆっくりと移動させてください
> - 移動中に誤って接触してアラームがトリガーされた場合は、障害物をすぐに取り除き、ゼロに戻って再試行してください
> - 移動前にトリガーされると、3Dプローブはアラームを鳴らします
> - 移動中（G0、G1、G2）にトリガーされると、3Dプローブはアラームを鳴らします
> - 検出距離内に物体が検出されない場合、3Dプローブはアラームを鳴らします
> - 原点復帰中は3Dプローブはアラームをトリガーしないため、3Dプローブの損傷を避けるために、原点復帰経路に障害物がないことを確認してください
>
> {.is-warning}

## 1. 3Dプローブの取り付け

3Dプローブを取り付けた後、ソフトウェアの工具設定（3Dプローブ）インターフェースに切り替えます。「工具交換」ボタンをクリックし、3Dプローブが自動高さ測定を完了するまで待ってから、後続の操作を続ける必要があります。

「工具交換」ボタンをクリックします：

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-换刀-01-录屏换刀.gif" alt="工具交換" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

3Dプローブを取り付け、ボタンをクリックして自動高さ測定を完了します（D1機器の工具交換については、D1の工具交換プロセスに従ってください：レンチでナットを取り外し、3Dプローブをコレットに取り付け、レンチでナットを締めます）

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-组装-02-组装测头.webp" alt="3Dプローブの組み立て" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/1-安装测头-测高-03-完成测高.webp" alt="自動高さ測定の完了" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **工具交換操作の注意事項**：
> 
> - ワークピースが高い場合は、必要に応じて主軸の高さを上に調整してください
> - 3Dプローブを使用してZ0を自動設定する必要がある場合は、このステップを必ず完了してください。そうしないと、後続の工具補正が正しくなりません。使用後は、工具交換をクリックし、工具を交換して自動工具高さ測定を完了してから加工を行ってください
> - センタリングや角検出（XY0の設定）のみに使用する場合は、このステップをスキップすることができますが、最初の工具を交換するときは、引き続き工具交換をクリックして自動高さ測定を完了する必要があります。その後、手動でZ0を設定してください
> - 3Dプローブを挿入した後は、主軸を開かないでください。そうしないと3Dプローブが損傷します！！！
> 
> {.is-warning}

## 2. インターフェースボタンの機能の紹介

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/0-界面-按钮-00-界面功能.jpg" alt="インターフェースボタンの機能" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

コントロール：
- 工具交換：取り付け前にクリックして3Dプローブを取り付け、測定後にクリックして加工工具に交換します
- XY0を設定：現在の位置をXY0点として設定し、手動設定に使用します。自動センタリングを使用する場合は無視してください
- Z0を設定：現在の位置をZ0点として設定し、手動設定に使用します。自動センタリングを使用する場合は無視してください

位置に移動：Xの中心、Yの中心、XYの中心。
- 3Dプローブを使用してXY0を設定した後、対応するアイコンが点灯し、クリックすると設定されたX0またはY0の位置に自動的に移動します（角検出にも適用されます）。

工具設定：
- 工具距離：検出中にプローブが移動する距離。設定された距離内にワークピースが検出されない場合、ポップアップが表示されます
- 工具速度：検出中にプローブがここで設定された速度で移動します
- ボール半径：プローブのボール先端の半径。これはデフォルト値で、変更する必要はありません

## 3. 角検出

ソフトウェアで角検出を選択して、材料の角の位置を検出し、角を自動的にXY0として設定します。左下の角を例にとります。

### X軸検出

移動機能を使用して、3Dプローブをワークピースの左側に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-x轴-移动-01-移动到工件左侧.jpg" alt="X軸の移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

検出をクリックすると、ワークピースが検出された後、検出された位置が自動的にX0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-x轴-探测-02-x轴探测截图.jpg" alt="X軸検出のスクリーンショット" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-x轴-探测-03-x轴探测过程.webp" alt="X軸検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y軸検出

移動機能を使用して、プローブをワークピースの前側に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-y轴-移动-01-移动到工件前侧.webp" alt="Y軸の移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

検出をクリックすると、ワークピースが検出された後、検出された位置が自動的にY0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-y轴-探测-02-y轴探测结果.jpg" alt="Y軸検出" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-y轴-探测-03-y轴探测过程.webp" alt="Y軸検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Z軸検出

移動機能を使用して、3Dプローブをワークピースの上方に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-z轴-移动-01-移动到工件上方.webp" alt="Z軸の移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z平面検出をクリックすると、ワークピースが検出された後、検出された位置が自動的にZ0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-z轴-探测-02-z轴探测成功.jpg" alt="Z軸検出の成功" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />
<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/2-角点-z轴-探测-03-z轴探测过程.webp" alt="Z軸検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 工具交換

すべての設定が完了した後、工具交換をクリックして使用する最初の工具に交換し、自動高さ測定を完了します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="工具交換をクリック" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="工具交換の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/d1换刀.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />


## 4. 長方形の外部センタリング

ソフトウェアで長方形の外部センタリングを選択して、中心位置を検出し自動計算し、検出された中心を手動でXY0点として設定します。

### X軸の左側検出

移動機能を使用して、3Dプローブをワークピースの左側に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x左-移动-01-移动到工件左侧.jpg" alt="X軸の左側移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

検出をクリックし、検出が完了するまで待ちます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x左-探测-02-左侧探测成功.jpg" alt="X軸の左側検出の成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x左-探测-03-左侧探测过程.webp" alt="X軸の左側検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### X軸の右側検出

ワークピースを検出した後、手動でZ軸を安全な高さまで上げ、ワークピースの右側に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-移动-01-移动到工件右侧.webp" alt="X軸の右側移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

検出をクリックし、検出が完了するまで待ちます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-探测-02-右侧探测成功.jpg" alt="X軸の右側検出の成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-探测-03-右侧探测过程.webp" alt="X軸の右側検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

ワークピースを検出した後、ワークピースの両側のX座標が得られます。下のZero Xをクリックすると、中心が自動的に計算され、中心がX0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-x右-分中-04-点击x轴分中.jpg" alt="センタリングをクリック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y軸検出

同じ方法を使用してワークピースの前後を検出し、Zero Yをクリックすると、中心が自動的に計算され、中心がY0として設定されます。

### Z軸検出

移動機能を使用して、3Dプローブをワークピースの上方に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-z轴-移动-01-移动到工件上方.webp" alt="Z軸の移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z平面検出をクリックし、検出が完了するまで待ちます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-z轴-探测-02-z轴探测成功.jpg" alt="Z軸検出の成功" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

ワークピースを検出した後、検出された位置が自動的にZ0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/3-矩形外-z轴-探测-03-z轴探测过程.webp" alt="Z軸検出の過程" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 工具交換

すべての設定が完了した後、工具交換をクリックして使用する最初の工具に交換し、自動高さ測定を完了します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="工具交換をクリック" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="工具交換の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/d1换刀.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />


> ⚠️ **長方形の外部センタリングの注意事項**：
> 
> 円形の外部センタリングと長方形の外部センタリングの操作は似ています。ただし、X中心点を検出するときはY軸座標を変更できず、Y中心点を検出するときはX軸座標を変更できないことに注意してください。例えば：Xの左側を検出した後、Z軸を上げてからXの右側に移動する間、Y軸を移動することはできません。
> 
> {.is-warning}

## 5. 円形の内部センタリング

ソフトウェアで円形の内部センタリングを選択して、中心位置を検出し自動計算し、検出された中心を手動でXY0点として設定します。

### X軸の左側検出

移動機能を使用して、プローブをワークピースの内部に移動し、ワークピース内部の左側に近づけます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x左-移动-01-移动到内部左侧.webp" alt="X軸の左側移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

左検出をクリックし、検出が完了するまで待ちます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x左-探测-02-内部左侧探测成功.jpg" alt="X軸の左側検出の成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x左-探测-03-内部左侧探测过程.webp" alt="X軸の左側検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### X軸の右側検出

ワークピースを検出した後、ワークピースの右側に近づけます（この間、Y軸を移動しないでください）。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-移动-01-移动到内部右侧.webp" alt="X軸の右側移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

右検出をクリックし、検出が完了するまで待ちます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-探测-02-内部右侧探测成功.jpg" alt="X軸の右側検出の成功" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-探测-03-内部右侧探测过程.webp" alt="X軸の右側検出の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

ワークピースを検出した後、ワークピース内部の両側のX座標が得られます。下のZero Xをクリックすると、中心が自動的に計算され、中心がX0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-x右-分中-04-点击x轴分中.jpg" alt="センタリングをクリック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### Y軸検出

同じ方法を使用してワークピース内部の前後を検出し、Zero Yをクリックすると、中心が自動的に計算され、中心がY0として設定されます。

### Z軸検出

移動機能を使用して、3Dプローブをワークピースの上方に移動します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-z轴-移动-01-移动到工件上方.webp" alt="Z軸の移動" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z平面検出をクリックし、検出が完了するまで待ちます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-z轴-探测-02-z轴探测成功.jpg" alt="Z軸検出の成功" style="width: 300px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

ワークピースを検出した後、検出された位置が自動的にZ0として設定されます。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/4-圆形内-z轴-探测-03-z轴探测过程.webp" alt="Z軸検出の過程" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 工具交換

すべての設定が完了した後、工具交換をクリックして使用する最初の工具に交換し、自動高さ測定を完了します。

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-点击-01-录屏点击换刀.gif" alt="工具交換をクリック" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/5-换刀-过程-02-换刀过程.webp" alt="工具交換の過程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-3d-probe-using/d1换刀.webp" alt="换刀过程" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />


> 📋 **センタリング操作のヒント**：
> 
> 長方形の内部センタリングと円形の内部センタリングの操作は似ています。
> 
> {.is-info}

## 6. 高さマップ機能

3Dプローブは高さマップ機能にも使用できます。これにより、ワークピース表面の高さ変動を検出して加工経路を自動調整し、より精密な加工結果を得ることができます。

- [MaxmakeLAB 3Dプローブ高さマップ機能](/en/himill-d1-d1s/hmd1s-height-map.md)