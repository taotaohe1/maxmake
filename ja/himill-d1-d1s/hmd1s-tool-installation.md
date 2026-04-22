# HiMill D1S 工具取り付けガイド

この文書では、HiMill D1S機器の工具取り付け方法について詳しく説明し、安全かつ正確な工具交換操作を確保します。

---

## 1. ソフトウェアによる工具交換の準備

工具を取り付ける前に、ソフトウェアの工具交換ボタンをクリックする必要があります。

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/1软件中点击换刀.gif" alt="ソフトウェアで工具交換ボタンをクリック" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📋 **工具交換準備のポイント**：
> 
> - ソフトウェアインターフェースが正常に表示されていることを確認
> - 機器の接続状態を確認
> - 現在進行中の加工タスクがないことを確認
> 
> {.is-info}

---

## 2. 機器の工具交換状態

機器が工具交換モードに入り、主軸が工具交換に便利な位置（X140,Y0）に移動し、工具交換を待ちます。このとき、インジケーターライトは黄色の点滅効果を示します。

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/2主轴移动至换刀位置.webp" alt="主軸が工具交換位置に移動" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/2指示灯黄色跳动.webp" alt="インジケーターライトの黄色点滅" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📱 **機器の状態確認**：
> 
> - 主軸が工具交換位置に移動していること
> - インジケーターライトが黄色に点滅し、工具交換が可能であることを示していること
> - 工具交換エリアに障害物がないことを確認
> 
> {.is-info}

---

## 3. 工具の取り付け

ハンドルを下に引き、工具を挿入します。工具のクランプは≥15mmでなければなりません。ゆっくりとハンドルを離します。

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/3拉下把手_放入刀具.webp" alt="ハンドルを引いて工具を挿入" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/3刀具夹持大于等于15mm.webp" alt="工具のクランプ長さは15mm以上" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **工具取り付けの安全要件**：
> 
> - 工具のクランプ深度は15mm～34mmの範囲内としてください（最大挿入深度は34mmです）
> - 工具の取り付けがしっかりしていることを確認
> - 工具の位置ずれや緩みを避ける
> 
> {.is-warning}

---

## 4. 工具の高さ測定

正しく取り付けられていることを確認した後、ボタンをクリックすると（内部または外部のいずれでも可）、主軸が高さ測定器の上に移動して高さ測定を完了します。

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/4内外部均可.webp" alt="内部および外部のボタンの両方が利用可能" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/4单击按键.webp" alt="ボタンをクリックして高さ測定をトリガー" style="width: 500px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> ⚠️ **工具の高さ測定の注意事項**：
> 
> - ファイルコードにT*M6がある限り、システムは工具交換ステップを実行します。このステップの前の工具の高さが測定されていない場合、T*M6を実行した後、工具補正が間違ってしまいます
> - 加工前の最初の工具は、Z0を設定する前に必ず高さ測定を完了する必要があります。これにより、他の工具に交換した後の工具補正エラーを回避します
> - 工具が1つしかない場合でも、Z0を設定する前にまず工具を交換して高さを測定する必要があります。これにより、プログラムのT1M6コードによる補正エラーを防ぎます
> 
> {.is-warning}

---

## 5. コレットと工具の一致

D1Sが6mmコレットを装備している場合、6mmの工具を取り付ける必要があります。

<img src="/eng/himill-d1-d1s/media/hmd1s-tool-installation/5夹头与刀具匹配.webp" alt="コレットと工具の一致" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

> 📏 **工具仕様の説明**：
> 
> - 4mmの工具に交換する場合は、まず工具を4mmのレデューシングスリーブに入れ、次に6mmのコレットに挿入します
> - 3.175mmの工具に交換する場合は、まず工具を3.175mmのレデューシングスリーブに入れ、次に6mmのコレットに挿入します
> - 混合使用は禁止されていることに注意してください
> 
> {.is-info}

---

## 📋 工具取り付けの安全のまとめ

> 🚨 **工具取り付けの安全のポイント**：
> 
> - 工具のクランプ深度は要件を満たさなければならない
> - 工具交換のたびに高さ測定を完了しなければならない
> - 工具の取り付けの堅牢性を確認する
> - 工具仕様の一致原則に従う
> 
> {.is-warning}