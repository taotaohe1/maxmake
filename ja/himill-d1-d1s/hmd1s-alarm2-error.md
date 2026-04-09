# Alarm2エラーの問題

## 問題の説明

機器が加工中にAlarm2エラーを表示する場合、通常はZ軸の移動範囲が不足していることが原因です。このガイドでは、この問題のトラブルシューティングと解決方法について詳しく説明します。

## トラブルシューティングの手順

### ステップ1：機器に接続する

**操作手順**：
機器がコンピュータに正しく接続されていることを確認し、MaxmakeLabソフトウェアを開きます。

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/1连接设备.gif" alt="機器接続のビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

### ステップ2：ワークフローをクリックして加工インターフェースに入る

**操作手順**：
1. MaxmakeLabソフトウェアで、上部のナビゲーションバーの「ワークフロー」ボタンをクリックします
2. 加工インターフェースに入り、後続の操作の準備をします

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/2进入加工界面.gif" alt="加工インターフェースに入るビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参照画像**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/1.jpg" alt="加工インターフェースに入る" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ3：工具交換コマンドを実行して3Dプローブを取り付ける

**操作手順**：
1. 加工インターフェースで「工具交換」ボタンを見つけてクリックします
2. 機器が工具交換位置に到達するのを待って、3Dプローブを取り付けます
3. 3Dプローブがしっかりと取り付けられていることを確認します

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/3换上三坐标.gif" alt="3Dプローブを取り付けるビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参照画像**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/2.jpg" alt="3Dプローブを取り付ける" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ4：XYZ零点を設定する

**操作手順**：
1. 3Dプローブを使用してワークピース表面を検出します
2. ソフトウェアでXYZ零点座標を設定します
3. 零点が正しく設定されていることを確認します

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/4设置零点.gif" alt="XYZ零点を設定するビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参照画像**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/3.jpg" alt="XYZ零点を設定する" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ5：工具交換コマンドを実行して加工工具を取り付ける

**操作手順**：
1. もう一度「工具交換」ボタンをクリックします
2. 機器が自動的に加工工具を取り付けるのを待ちます
3. 工具がしっかりと取り付けられていることを確認します

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/5换上加工刀具.gif" alt="加工工具を取り付けるビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参照画像**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/4.jpg" alt="加工工具を取り付ける" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ6：工具交換後の高さ補正を確認する

**操作手順**：
1. ソフトウェアに表示される高さ補正値を確認します
2. 補正値が正しく設定されていることを確認します
3. 必要に応じて調整します

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/6检验高度补偿.gif" alt="高さ補正を確認するビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参照画像**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/5.jpg" alt="高さ補正を確認する" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ7：Z軸の移動範囲を確認する

**操作手順**：
1. 加工ファイルを読み込みます
2. 3DプレビューでZの移動範囲を確認します
3. Zの移動範囲が機器の許容範囲内にあるかどうかを確認します
4. Zの移動範囲が機器の許容範囲を超えている場合は、Z零点の位置を調整します

**操作ビデオ**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/7加工报错.gif" alt="加工エラーのビデオ" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 0px;" />

**参照画像**：
<img src="/eng/himill-d1-d1s/media/hmd1s-alarm2-error/6.jpg" alt="Z軸の移動範囲を確認する" style="width:100%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

**問題の分析**：
ビデオでは、3Dプレビューの左下隅のZ移動が-10.5から5であることがわかります。これは、Z零点が最大5mm上方向の移動と10.5mm下方向の移動を必要とすることを意味します。

Z零点が73mmに設定され、機器の最大Z移動が80mmの場合、利用可能な移動範囲は80mm - 73mm = 7mmです。これは加工に必要な10.5mmの下方向移動にははるかに不足しているため、加工中に必ずエラーが発生します。

## 解決策

このような場合、Z軸の移動のために十分な加工距離を確保する必要があります：

1. **Z零点の位置を調整する**：Z零点をより適切な位置に設定し、十分な移動スペースを確保します
2. **ワークピースの高さを確認する**：ワークピースが低すぎる場合は、垫块を使用するか加工戦略を調整してください
3. **移動範囲を確認する**：加工前に、3DプレビューでZの移動範囲を常に確認し、機器の許容範囲内にあることを確認します
4. **安全距離を確保する**：零点を設定する際は、少なくとも5-10mmの安全距離を確保することを推奨します

## 予防策

1. **加工前のチェック**：各加工前に、3Dプレビューで移動範囲を必ず確認します
2. **零点の設定**：機器の移動限界に近づかないように合理的に零点を設定します
3. **工具の長さ**：工具が長すぎることによる移動不足を避けるため、適切な長さの工具を使用します
4. **ワークピースのクランプ**：ワークピースがしっかりとクランプされ、適切な高さにあることを確認します

> 💡 **ヒント**：引き続きAlarm2エラーが発生する場合は、機器のリミットスイッチが正常に動作しているかどうか、およびファームウェアのバージョンが最新であるかどうかを確認してください。
> {.is-info}