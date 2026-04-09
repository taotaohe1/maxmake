# MaxmakeLab回転軸加工 - NCプログラムインポート加工ワークフロー

## 1. CNCモードに切り替える

モードをCNCモードに切り替えます。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/1-切换cnc模式.webp" alt="CNCモードに切り替える" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. ファイルをインポートする

機器に接続した後、準備したNCプログラムをインポートします。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/1-导入文件.webp" alt="ファイルをインポート" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. 主軸を上げる

回転軸自体の高さが比較的高いため、主軸を上げる必要がある場合があります。主軸の3つの固定ネジを緩め、上に移動させてから再固定します。

<img src="/eng/himill-d1-d1s/media/hmd1-rotation-axis-processing/1-上调主轴.webp" alt="主軸を上げる" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. 移動と位置決め

主軸をオンにし、工具を加工原点に移動させます。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/3-移动定位-打开主轴.webp" alt="主軸をオンにする" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/3-移动定位-移动.webp" alt="移動" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. 原点を設定する

工具が加工原点にあるときに、XY0を設定するためにクリックします。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-1-刀具位于原点时.webp" alt="工具が原点にある" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-1-设置xy0点.webp" alt="XY0点を設定" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z軸をゆっくりと下げます。工具がワークピースに接触したときに、Z0を設定するためにクリックします。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-2-降下z轴.webp" alt="Z軸を下げる" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/4-设置原点-2-设置z0点.webp" alt="Z0点を設定" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **原点設定の注意事項**：
> 
> - この場合、NCプログラムのZ0は正方形ワークピースの角のエッジにあるため、Z0を設定するときは、角を真上に調整する必要があります
> - 回転軸加工の前に、工具パスを設計する際は、まずワークピースをクランプすることを推奨します。クランプ位置を注意深く考慮する必要があります。生成された工具パスは、衝突を防ぐためにチャックジョーを避ける必要があります
> - 同時に、Z軸の加工範囲を事前に決定する必要があり、工具の長さを事前に計算して、工具の長さが不十分で加工できなくなるのを防ぐ必要があります
> 
> {.is-warning}

## 6. プレビューシミュレーション

3Dインターフェースで、シミュレーションパスをプレビューすることができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/5-预览仿真.webp" alt="プレビューシミュレーション" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **プレビューシミュレーションのヒント**：
> 
> - リアルタイムプレビューのために再生速度を調整することができます
> - プログレスバーを直接ドラッグすることができます
> 
> {.is-info}

## 7. ファイルを転送して加工を開始する

加工開始ボタンをクリックして、加工ファイルをデバイスのSDカードに転送します。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/6-点击开始.webp" alt="開始をクリック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

プロンプトに従って、インジケーターライトが虹色の回転ライト効果を示すまで待ってから、機器のボタンを2秒間長押しして加工を開始します。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/6-接受文件开始加工.webp" alt="ファイルを受け入れて加工を開始" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **加工制御の注意事項**：
> 
> - 加工中にボタンを単クリックすると加工が一時停止します。2秒間長押しすると加工が再開します
> - 安全ドア機能が有効になっている場合、加工を再開する前にドアを閉めてください
> 
> {.is-warning}

## 8. 加工中に主軸速度と送り速度を変更することができる

加工中に主軸速度と送り速度を変更することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-rotation-axis-processing/7-覆写功能.webp" alt="オーバーライド機能" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **パラメータ調整の注意事項**：
> 
> - 加工中は、特に金属加工の場合、主軸速度を下げないことを推奨します。負荷が増加して工具の破損を引き起こす可能性があります
> - 値を変更した後、速度は徐々に上昇または下降します。実際の状況に応じて値を徐々に増加または減少させる必要があります
> 
> {.is-warning}