# MaxmakeLabソフトウェアマニュアル

## 目次

- [1. メインインターフェース機能エリアの紹介](#1-メインインターフェース機能エリアの紹介)
- [2. メニューバー](#2-メニューバー)
- [3. デザインパネル](#3-デザインパネル)
- [4. パラメータパネル](#4-パラメータパネル)
- [5. カラーパネル](#5-カラーパネル)
- [6. デバイスパネル](#6-デバイスパネル)
- [7. レイヤーパネル](#7-レイヤーパネル)
- [8. 工具経路の生成](#8-工具経路の生成)
- [9. CNC加工ワークフロー](#9-cnc加工ワークフロー)
- [10. レーザー加工ワークフロー](#10-レーザー加工ワークフロー)

---

## <a id="1-メインインターフェース機能エリアの紹介"></a>1. メインインターフェース機能エリアの紹介

<div style="display: flex; gap: 16px; flex-wrap: wrap;">
  <img src="/eng/maxmakelab/media/software-manual/main-interface1.png" alt="メインインターフェースの全体レイアウト1" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
  <img src="/eng/maxmakelab/media/software-manual/main-interface2.png" alt="メインインターフェースの全体レイアウト2" style="width: calc(50% - 8px); height: auto; border-radius: 8px;" />
</div>

#### インターフェース機能エリア

| エリア | 名前 | 機能説明 |
|--------|------|----------|
| 1 | メニューバー | ファイルのインポート/エクスポート、ビューサイズの調整、ソフトウェア設定、ヘルプガイダンス、言語切り替え、モード切り替え |
| 2 | デザインパネル | 様々な種類のグラフィック要素を追加 |
| 3 | キャンバス | 一般的に機器の作業エリアサイズ |
| 4 | カラーパネル | グラフィック要素に異なる色を割り当て |
| 5 | デバイスパネル | デバイスの選択、接続、クイックコントロール |
| 6 | パラメータ設定 | CNCでは、ブランクパラメータと工具ライブラリパラメータを設定 |
| 7 | 工具経路の生成 | 工具経路の生成方法を選択 |
| 8 | 工具経路リスト | 生成された工具経路を表示 |
| 9 | クイックコントロール | レーザーでは、高速移動やリセットなどのクイックコントロール機能 |
| 10 | レイヤーパネル | 異なる色のグラフィック要素に異なる加工パラメータを割り当て |
| 11 | シミュレーションプレビュー | 加工経路のシミュレーションとプレビュー |
| - | ワークフロー | クリックして加工プレビューインターフェースに入る |

---

## <a id="2-メニューバー"></a>2. メニューバー

<img src="/eng/maxmakelab/media/software-manual/menu-bar.png" alt="メニューバーインターフェース" style="width: 200px; height: auto; border-radius: 8px;" />

#### 一般的な操作

| 機能 | 説明 |
|------|------|
| **ドロップダウンメニュー** | ドロップダウンリストをクリックして特定の操作を選択 |
| <img src="/eng/maxmakelab/media/software-manual/dropdown-menu.png" alt="ドロップダウンメニューの例" style="width: 250px; height: auto; border-radius: 8px;" /> | |
| **保存** | 現在のプロジェクトを保存 |
| **元に戻す** | 前の操作を元に戻す |
| **やり直す** | 次の操作を復元する |

---

## <a id="3-デザインパネル"></a>3. デザインパネル

<img src="/eng/maxmakelab/media/software-manual/design-panel.png" alt="デザインパネルインターフェース" style="width: 40px; height: auto; border-radius: 8px;" />

#### ツールボックス

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">ツール</th>
      <th style="width: 20%;">機能説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**選択**</td>
      <td>選択モードに入り、グラフィック要素を選択、グラフィック要素を移動可能</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-select.gif" alt="選択ツール" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**画像**</td>
      <td>画像を挿入、png、jpg、jpeg形式をサポート</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-image.gif" alt="画像挿入" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**基本**</td>
      <td>線、正方形、円を追加</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-basic.gif" alt="基本グラフィック" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**テキスト**</td>
      <td>テキストを追加</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-text.gif" alt="テキスト挿入" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**ペン**</td>
      <td>ベジエ曲線を追加</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-pen.gif" alt="ペンツール" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**ノード**</td>
      <td>ノード編集ツール</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-node.gif" alt="ノード編集" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**オフセット**</td>
      <td>現在のグラフィックの内側と外側の輪郭をオフセット</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-offset.gif" alt="オフセットツール" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**クリップアート**</td>
      <td>様々なカテゴリのグラフィックを追加</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-offset-clipart.gif" alt="クリップアートライブラリ" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**プラグイン**</td>
      <td>ボックス生成、ギア生成を含む</td>
      <td><img src="/eng/maxmakelab/media/software-manual/design-panel-plugin.gif" alt="プラグイン拡張" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="4-パラメータパネル"></a>4. パラメータパネル

<img src="/eng/maxmakelab/media/software-manual/parameter-panel.png" alt="パラメータパネルインターフェース" style="width: 600px; height: auto; border-radius: 8px;" />

> 💡 パラメータパネルはグラフィックを選択した後に表示され、選択解除後に非表示になります

#### 基本的な変換

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**点座標**</td>
      <td>異なる点を選択し、現在の点の座標値を表示または設定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-点坐标.gif" alt="点座標" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**幅と高さ**</td>
      <td>現在のグラフィック要素の幅と高さを表示または設定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-宽高度.gif" alt="幅と高さ" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**ロック**</td>
      <td>グラフィックの縦横比をロックまたはロック解除</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-锁定.gif" alt="ロック" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**回転角度**</td>
      <td>グラフィック要素の回転角度を設定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-旋转角度.gif" alt="回転角度" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**水平ミラー**</td>
      <td>グラフィック要素を水平方向に反転</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-水平镜像.gif" alt="水平ミラー" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**垂直ミラー**</td>
      <td>グラフィック要素を垂直方向に反転</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-垂直镜像.gif" alt="垂直ミラー" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 配置ツール

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**配置**</td>
      <td>左揃え、右揃え、水平中央揃え、上揃え、下揃え、垂直中央揃え</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-对齐.gif" alt="配置" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**分布**</td>
      <td>水平間隔分布、垂直間隔分布</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-分布.gif" alt="分布" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### アレイツール

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**長方形アレイ**</td>
      <td>長方形アレイ形式でグラフィックを迅速に追加</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-矩形阵列.gif" alt="長方形アレイ" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**円形アレイ**</td>
      <td>円形アレイ形式でグラフィックを迅速に追加</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-环形阵列.gif" alt="円形アレイ" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**ブール演算**</td>
      <td>2つ以上のグラフィックオブジェクトに加算、減算、交差、または排他的操作を実行して新しいグラフィックを生成</td>
      <td><img src="/eng/maxmakelab/media/software-manual/parameter-panel-布尔运算.gif" alt="ブール演算" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="5-カラーパネル"></a>5. カラーパネル

<img src="/eng/maxmakelab/media/software-manual/color-panel.png" alt="カラーパネルインターフェース" style="width: 300px; height: auto; border-radius: 8px;" />

#### 使用方法

- **既存の要素の色を設定**：要素を選択した後、色アイコンをクリックして選択した要素をその色に設定
  <img src="/eng/maxmakelab/media/software-manual/color-panel-选图元设置颜色.gif" alt="要素を選択して色を設定" style="width: 600px; height: auto; border-radius: 8px;" />

- **新しい要素の色を設定**：色を選択した後、要素を追加すると、追加された要素はその色になります
  <img src="/eng/maxmakelab/media/software-manual/color-panel-选择颜色添加图元.gif" alt="色を選択して要素を追加" style="width: 600px; height: auto; border-radius: 8px;" />

- **座標表示**：下の座標表示は、現在のマウスポインターがある座標値を示します

---

## <a id="6-デバイスパネル"></a>6. デバイスパネル

<img src="/eng/maxmakelab/media/software-manual/device-panel.png" alt="デバイスパネルインターフェース" style="width: 400px; height: auto; border-radius: 8px;" />

#### 接続と制御

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**モードドロップダウンオプション**</td>
      <td>機器の加工モードを選択</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-模式下拉选项.gif" alt="モードドロップダウンオプション" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**接続アイコン**</td>
      <td>接続または接続を切断</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-连接图标.gif" alt="接続アイコン" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**デバイスを選択**</td>
      <td>デバイスを選択し、デバイスパラメータを読み込む</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-选择设备.gif" alt="デバイスを選択" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**デバイス設定**</td>
      <td>そのデバイスでサポートされている設定オプション</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-设备设置.gif" alt="デバイス設定" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**ヘルプ**</td>
      <td>そのデバイスのヘルプオプション</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-帮助.gif" alt="ヘルプ" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**クイックボタン**</td>
      <td>レーザーでは、そのデバイスでサポートされているクイック操作ボタン</td>
      <td><img src="/eng/maxmakelab/media/software-manual/device-panel-快捷按钮.gif" alt="クイックボタン" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

---

## <a id="7-レイヤーパネル"></a>7. レイヤーパネル

<img src="/eng/maxmakelab/media/software-manual/layer-panel.png" alt="レイヤーパネルインターフェース" style="width: 300px; height: auto; border-radius: 8px;" />

#### 機能説明

- **加工パラメータの設定**：レーザーモードでは、異なる色のグラフィック要素の加工パラメータを表示または設定
  <img src="/eng/maxmakelab/media/software-manual/layer-panel-设置加工参数.gif" alt="レイヤー加工パラメータ" style="width: 600px; height: auto; border-radius: 8px;" />

- **レイヤー管理**：レイヤーの上へ移動、レイヤーの下へ移動、レイヤーの削除が可能

---

## <a id="8-工具経路の生成"></a>8. 工具経路の生成

<img src="/eng/maxmakelab/media/software-manual/toolpath-generation.png" alt="工具経路生成インターフェース" style="width: 250px; height: auto; border-radius: 8px;" />

#### 機能一覧

| 機能 | 説明 |
|------|------|
| **ブランクの設定** | ブランクサイズを設定 |
| **工具パラメータライブラリ** | 工具パラメータ情報を追加 |
| **工具経路と操作** | 輪郭フライス、平面フライス、V型フライス、穴あけ、レリーフ、工具経路プログラムのインポート |
| **工具経路** | 生成された工具経路を表示 |

---

## <a id="9-cnc加工ワークフロー"></a>9. CNC加工ワークフロー

<img src="/eng/maxmakelab/media/software-manual/cnc-workflow.png" alt="CNCワークフローインターフェース" style="width: 600px; height: auto; border-radius: 8px;" />

#### ステータスと制御

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**ステータスバー**</td>
      <td>ワークピース座標系、機械座標系、安全ドアの状態、モーダル情報を表示</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-状态栏.png" alt="ステータスバー" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**ステップ制御**</td>
      <td>XYZA軸の移動を制御、ステップサイズ、送り速度を設定可能</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-单步控制.gif" alt="ステップ制御" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**主軸スイッチ**</td>
      <td>設定された回転速度に応じて主軸のオン/オフを制御可能</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-主轴开关.gif" alt="主軸スイッチ" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**工具交換**</td>
      <td>工具を交換し、工具の高さを自動的に測定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-换刀.gif" alt="工具交換" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 座標設定

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**XY0の設定**</td>
      <td>現在のXY座標を加工中のXYゼロ点として設定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-设置xy0.gif" alt="XY0の設定" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Z0の設定**</td>
      <td>現在のZ座標を加工中のZゼロ点として設定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-设置z0.gif" alt="Z0の設定" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**XYゼロ点へ移動**</td>
      <td>自動的に安全な高さまで上昇し、次にXYゼロ点の位置へ移動</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-移动到xy零点.gif" alt="XYゼロ点へ移動" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### ファイルと出力

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**ファイル**</td>
      <td>加工ファイルを選択</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-文件.gif" alt="ファイル" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**コンソール**</td>
      <td>手動またはマクロボタンを使用してGコードを送信可能</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-控制台.gif" alt="コンソール" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**Gコード**</td>
      <td>ロードされたGコードを表示</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-gcode.gif" alt="Gコード" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**プレビューシミュレーションエリア**</td>
      <td>コードの2Dビューまたは3Dシミュレーションビューを表示</td>
      <td><img src="/eng/maxmakelab/media/software-manual/cnc-workflow-预览仿真区域.gif" alt="プレビューシミュレーションエリア" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### その他の操作

| 機能 | 説明 |
|------|------|
| **原点復帰** | 機器が原点に戻る、電源投入後、機器を運転する前に必ずこの操作を実行する必要がある |
| **境界** | 主軸の試運転加工範囲、このボタンをクリックする前に主軸を手動で安全な高さまで上昇させる必要があることに注意 |
| **リセット** | ソフトウェアシステムのリセット、現在の操作を終了し、システムの初期状態に復元 |
| **アンロック** | アラームロック状態を解除し、軸の移動権限を復元 |
| **復元** | 機器のGrbl設定を復元、機器の$パラメータを変更した後にデフォルト値に復元するためにクリック可能 |

<img src="/eng/maxmakelab/media/software-manual/cnc-workflow-other.png" alt="その他のコントロール" style="width: 600px; height: auto; border-radius: 8px;" />

---

## <a id="10-レーザー加工ワークフロー"></a>10. レーザー加工ワークフロー

<img src="/eng/maxmakelab/media/software-manual/laser-workflow.png" alt="レーザーワークフローインターフェース" style="width: 600px; height: auto; border-radius: 8px;" />

> 📌 レーザー加工ワークフローには、CNCとの主な違いがあります：

#### 固有の機能

<table style="width: 100%; table-layout: fixed;">
  <thead>
    <tr>
      <th style="width: 10%;">機能</th>
      <th style="width: 20%;">説明</th>
      <th style="width: 70%;">デモ</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>**Gコードの保存**</td>
      <td>現在のすべての加工内容をテキスト形式で保存</td>
      <td><img src="/eng/maxmakelab/media/software-manual/laser-workflow-保存gcode.gif" alt="Gコードの保存" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**レーザーのアクティブ化**</td>
      <td>クリックすると、レーザー機能とモーター高速モードがアクティブ化されます。もう一度クリックすると、レーザー機能を終了し、モーターの通常モードに戻ります</td>
      <td><img src="/eng/maxmakelab/media/software-manual/laser-workflow-激活激光.gif" alt="レーザーのアクティブ化" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
    <tr>
      <td>**開始位置**</td>
      <td>加工の開始位置を設定</td>
      <td><img src="/eng/maxmakelab/media/software-manual/laser-workflow-开始位置.gif" alt="開始位置" style="width: 100%; height: auto; border-radius: 8px;" /></td>
    </tr>
  </tbody>
</table>

#### 座標モード

| モード | 説明 |
|------|------|
| **絶対座標モード** | グラフィックが配置されている機械座標位置に基づいて加工。加工位置はグラフィックとともに変化 |
| **現在位置モード** | 機械ヘッドが配置されている位置に基づいて加工。加工位置は機械ヘッドとともに変化 |

---

## ショートカットリファレンス

| ショートカット | 機能 |
|---------------|------|
| Ctrl + Z | 元に戻す |
| Delete | 選択した要素を削除 |
| Esc | 選択を解除 |

---