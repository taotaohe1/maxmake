# HiMill D1/D1Sの移動軸操作の問題

## 注意事項
>- **緊急対応**：軸の衝突や詰まりが続く場合は、機器を即座に停止して電源を切り、機械部品のさらなる損傷を避けてください
>- **安全な操作**：点検や修理を行う前に、機器が完全に電源オフになっていることを確認してください
>- **操作仕様**：軸の位置を手動で調整する場合は、ゆっくりと操作してください
>- **保護対策**：機械部品を取り扱う場合は、擦り傷を防ぐために保護手袋を着用することをお勧めします
> {.is-warning}
---

## 可能性のある現象
- **電源投入後にロックされない**：機器の電源を入れた後、軸がロック状態にならず、自由に動く可能性があります
- **軸が動かない**：コントローラを操作しても、軸に動きの反応がありません
- **軸の動きがスタッタリングする**：軸の動きがスタッタリングしたり、振動したり、異常な音がしたりします

## 可能性のある原因
### 電気的故障
- モータードライバの故障または損傷
- モーターの配線が緩んでいる、接触不良、または切断されている
- モーター自体が故障している

### 機械的故障
- 機械的伝達部品（リードスクリュー、ガイドレールなど）に故障があるか、異物が詰まっている
- ガイドレールまたはリードスクリューの潤滑不足により摩擦が増加している

### 制御システムの問題
- リミットスイッチがトリガーされているか損傷している
- パラメータ設定が正しくない
- コントローラソフトウェアの異常

## 解決策

### 1. リミットスイッチの異常を除外する
- 電源を入れた後、原点復帰操作を試みて正常に動くかどうか確認してください
- 原点復帰が失敗した場合は、[HiMill D1/D1S リミットスイッチの問題](/en/himill-d1-d1s/hmd1s-limit-switch-issue.md)を参照してください

### 2. 機械的伝達部品を確認する
- 伝達経路に異物が詰まっていないか注意深く確認してください
- 詰まりが見つかった場合は、即座に電源を切り、異物を取り除いてください

### 3. モーターの接続線を確認する

#### Xモーターの接続線
主軸を右に移動させて点検します。再接続してみてください：
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/x电机.jpg" alt="Xモーター" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/x电机线.jpg" alt="Xモーターの配線" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### Yモーターの接続線
機器を横に置いて点検します。再接続してみてください：
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/y电机线.jpg" alt="Yモーターの配線" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### Zモーターの接続線
以下の位置を確認してください。再接続してみてください：
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/z电机线.jpg" alt="Zモーターの配線" style="width: 400px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 4. 潤滑状態を確認する
- ガイドレールとリードスクリューの潤滑が不足していないか確認してください
- 長期間潤滑されていないと、動作中に騒音や詰まりが発生します

### 5. 機器を再起動する
- 機器の電源を切り、30秒待ってから再起動してください
- 軸の動きが正常に戻ったかどうか観察してください

### 6. パラメータ設定を復元する
- 動きがまだスタッタリングして異常な音がする場合は、機器を工場出荷時のパラメータに復元してみてください。機器に接続した後、原点復帰してから復元ボタンをクリックしてみてください
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/恢复参数.png" alt="パラメータの復元" style="width: 600px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 7. メインコントロールボードのモーター配線を確認する
- メインコントロールボードのモーター接続線が緩んでいるか接触不良がないか確認してください。カバーの取り外し手順については、メインコントロールボード交換のビデオを参照してください [HiMill D1/D1S エアキャビネットコンポーネントの交換](/en/himill-d1-d1s/hmd1s-replace-air-cabinet.md)
<img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/主控板未插线电机.jpg" alt="モーター配線のないメインコントロールボード" style="width: 350px; height: auto; margin-bottom: 8px; border-radius: 16px;" /> <img src="/eng/himill-d1-d1s/media/hmd1s-moving-axis-issue/主控板插线电机.jpg" alt="モーター配線のあるメインコントロールボード" style="width: 450px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### 8. 技術サポートに連絡する
上記の方法のいずれも効果がない場合は、さらなる支援のためにsupport@maxmake.comに連絡してください