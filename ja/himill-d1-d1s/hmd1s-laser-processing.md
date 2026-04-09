# MaxmakeLabレーザー加工

## ⚠️ 使用のお知らせ

使用前に必ずレーザーの使用仕様を確認してください!!!

[レーザーモジュールの使用方法へのリンク](hmd1s-laser-module.md)

---

## 1. レーザーモードに切り替える

ソフトウェアインターフェースのレーザーモードオプションをクリックします：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/1-切换激光模式.webp" alt="レーザーモードに切り替える" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 2. ファイルを追加する

独自のグラフィックをデザインしたり、素材ライブラリからグラフィックをインポートしたり、画像を追加したりすることができます：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/1-导入文件.webp" alt="ファイルをインポート" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 3. レーザーモードを有効にする

レーザーを有効にするボタンをクリックしてレーザーモードを有効にします：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/1-点击激光模式.webp" alt="レーザーモードをクリック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **レーザーの有効化の注意事項**：
> 
> - レーザーを有効にすると、モーターが高速モードに入り、最大加工速度は2000mm/minになります。動作中に多少の騒音が発生しますが、これは正常です
> - 加工が完了した後、CNCモードに切り替えるときは、レーザーモードをキャンセルするために再び有効化ボタンをクリックする必要があります
> 
> {.is-warning}

## 4. パラメータの設定

レーザーモードでは、最大速度は2000mm/min（約33mm/s）です。テスト結果に基づいて適切にパワーを調整してください：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/2-设置参数.webp" alt="パラメータの設定" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 5. 移動と位置決め

レーザーを材料の上に移動させます：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/3-移动.webp" alt="移動と位置決め" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 6. ボーダーの位置決め

ボーダーボタンをクリックすると、レーザーが弱い光で加工範囲をなぞります：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/4-边框定位.webp" alt="ボーダーの位置決め" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 7. 焦点を調整する

レーザー加工の最適な焦点位置は、遮光板の底面から材料まで5mmです。レーザーアクセサリーボックスの焦点アシストブロックを使用し、Z軸をゆっくりと下げて、焦点アシストブロックがぎりぎり隙間を通るまで調整します：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/5-对焦辅助片.webp" alt="焦点アシストブロック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

## 8. ファイルを転送して加工を開始する

加工を開始するボタンをクリックして、加工ファイルを機器のSDカードに転送します。ボタンを2秒間長押しして加工を開始します：

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/6-点击开始.webp" alt="開始するためにクリック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<br>

<img src="/eng/himill-d1-d1s/media/hmd1s-laser-processing/6-接受文件开始加工.webp" alt="ファイルを受け取って加工を開始" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **加工の注意事項**：
> 
> レーザーと主軸が同軸でないため、実際の加工範囲は約20mm前方にオフセットしています。大きなグラフィックを加工すると、レーザーが機器を超えることがあります。この時は安全ドアを開く必要があり、ソフトウェア設定で安全ドア機能をオフにする必要があります
> 
> {.is-warning}