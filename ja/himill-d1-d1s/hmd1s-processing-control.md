# MaxmakeLab CNC加工 - NCプログラムインポート加工ワークフロー


## 1. CNCモードに切り替える

モードをCNCモードに切り替えます。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/1-切换cnc模式.webp" alt="CNCモードに切り替える" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. ファイルをインポートする

機器に接続した後、準備したNCプログラムをインポートします。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/1-导入文件.webp" alt="ファイルをインポート" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. 移動と位置決め

主軸をオンにし、工具を加工原点に移動させます。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/2-转动主轴.webp" alt="主軸をオンにする" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/2-移动到原点.webp" alt="原点に移動" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 4. 原点を設定する

ワークピースの中心点を加工原点とする例では、工具がワークピースの中心点にあるときに、XY0を設定するためにクリックします。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-刀具处于中心点.webp" alt="工具が中心点にある" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-设置xy0点.webp" alt="XY0点を設定" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

Z軸をゆっくりと下げます。工具がワークピースに接触したときに、Z0を設定するためにクリックします。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-降z轴.webp" alt="Z軸を下げる" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />  

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/3-设置原点-设置z0点.webp" alt="Z0点を設定" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. プレビューシミュレーション

3Dインターフェースで、シミュレーションパスをプレビューすることができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/4-预览仿真.webp" alt="プレビューシミュレーション" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **プレビューシミュレーションのヒント**：
> 
> - リアルタイムプレビューのために再生速度を調整することができます
> - プログレスバーを直接ドラッグすることができます
> 
> {.is-info}

## 6. ファイルを転送して加工を開始する

加工開始ボタンをクリックして、加工ファイルをデバイスのSDカードに転送します。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/5-开始.webp" alt="加工を開始" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

プロンプトに従って、インジケーターライトが虹色の回転ライト効果を示すまで待ってから、機器のボタンを2秒間長押しして加工を開始します。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/5-接受文件开始加工.webp" alt="ファイルを受け入れて加工を開始" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **加工制御の注意事項**：
> 
> - 加工中にボタンを単クリックすると加工が一時停止します。2秒間長押しすると加工が再開します
> - 安全ドア機能が有効になっている場合、加工を再開する前にドアを閉めてください。ドアが閉まっていない場合、2秒間長押しした後も再開加工のライト効果が表示され、最終的に緑色の定常ライトになりますが、機器に動作はありません
> 
> {.is-warning}

## 7. 加工中のパラメータ調整

加工中に送り速度を変更することができます。

<img src="/eng/himill-d1-d1s/media/hmd1s-processing-control/6-覆写功能，更改转速进给率.webp" alt="オーバーライド機能、主軸速度と送り速度の変更" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **パラメータ調整の注意事項**：
> 
> - 加工中は、特に金属加工の場合、主軸速度を下げないことを推奨します。負荷が増加して工具の破損を引き起こす可能性があります
> - 値を変更した後、速度は徐々に上昇または下降します。実際の状況に応じて値を徐々に増加または減少させる必要があります
> 
> {.is-warning}