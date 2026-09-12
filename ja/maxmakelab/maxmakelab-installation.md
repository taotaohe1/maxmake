# MaxmakeLabソフトウェアのインストール

## 📖 ソフトウェアの紹介
MaxmakeLabは、HiMillシリーズCNC機器専用に設計されたインテリジェント制御ソフトウェアであり、直感的な操作インターフェースと豊富な加工機能を提供し、ユーザーが様々なクリエイティブな加工タスクを簡単に完成させるのを助けます。

## 🖥️ システム要件

### Windowsシステム
- **オペレーティングシステム**：Windows 10/11（64ビット）以上
- **プロセッサ**：Intel i3または同等のパフォーマンスのCPU（非ARMアーキテクチャ）
- **メモリ**：4GB以上
- **ストレージスペース**：1GB以上の空きスペース
- **ディスプレイ**：解像度1920x1080以上
- **USBポート**：USB 2.0以上のバージョン

### macOSシステム
- **オペレーティングシステム**：macOS 14（Sonoma）以上
- **プロセッサ**：Apple Silicon
- **メモリ**：4GB以上
- **ストレージスペース**：1GB以上の空きスペース
- **ディスプレイ**：解像度1920x1080以上
- **USBポート**：USB 2.0以上のバージョン

> ⚠️ **プロセッサ互換性の注意**：
> Apple Silicon Mシリーズチップのみをサポートし、Intelシリーズチップはサポートしていません。
> {.is-warning}

## 📥 ソフトウェアのダウンロード
以下のリンクからMaxmakeLabソフトウェアをダウンロードすることができます。お使いのオペレーティングシステムとニーズに応じて適切なバージョンを選択してください：

> ℹ️ **バージョン0.9.20更新内容**：
> 
> **一、Probe機能**
> 1. 工具設定画面にプローブステータスランプ表示を追加
> 2. プローブ高さマップ適用時のGCodeのM3/M4コマンド後にF値を追加
> 
> **二、工具パラメータとパス**
> 1. オフセット輪郭フライス加工の複雑な工具パスエラー問題を修正
> 2. 工具パラメータライブラリデータベース機能調整：ソフトウェア更新後にユーザー変更した工具パラメータを上書きしない。デフォルトでtoolbase_user.db3を読み込み（存在しない場合はtoolbase.db3から自動コピー）、ユーザーパラメータはこのファイルに保存
> 3. 工具パラメータライブラリリセットのポップアップヒントを追加
> 
> **三、レイヤー管理**
> 1. CNCモードで図形追加後、レーザーモードでレイヤーが表示される問題を修正
> 2. レーザーモードでレイヤーに図形がない場合でもレイヤー情報が表示される問題を修正
> 
> **四、図形操作とレンダリング**
> 1. 図形の幅・高さレンダリング、ルーラーの幅・高さハイライトレンダリングを追加
> 2. 整列操作でShift単一選択図形を基準図元としてサポート
> 3. 2Dキャンバスで図形移動時のスナップ整列機能を新規追加
> 4. 複数回のグループ解除後に図形が消失する問題を修正
> 5. クリップ機能を追加
> 
> **五、テキスト編集**
> 1. テキスト追加操作中にESCキー押下時のUI問題を修正
> 2. ダブルクリックでのテキスト再編集中にESCキー押下時のレンダリング問題を修正
> 3. テキスト追加時に選択フォントが文字をサポートしない場合、候補フォント（プロジェクト内フォント）でグリフを読み込み
> 4. テキスト操作のESCキー取消機能を送信機能に変更、テキスト再編集後にESCキーで送信をトリガー
> 5. ノード編集機能を再設計：現在はコントロールポイントの移動のみサポート、今後ノード追加・削除などの機能を追加予定
> 
> **六、エラー処理と安定性**
> 1. アラームエラーの3、4、5、8、9の原点復帰と検出ボタンでソフトウェアがクラッシュする問題を修正
> 2. アラームポップアップ表示をAbout画面表示と一致させ、個別ウィンドウ表示しない
> 
> **七、UI/UX最適化**
> 1. ソフトウェア起動後のユーザーヒントをデフォルトで閉じる
> 2. 工具交換ポップアップを3秒後に自動的に閉じる
> 3. クリップ操作からノード編集操作に切り替える際のカーソル問題を修正
> 
> ソフトウェアの問題がある場合は、Discordのソフトウェアフィードバック専用チャンネルでお問い合わせください。皆様のご意見を積極的に参考にし、問題を速やかに修正いたします：[Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)
> {.is-info}

### 最新バージョン（v0.9.20）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.20.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.20.dmg)**

### 以前のバージョン（v0.9.19）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.19.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.19.dmg)**

### 以前のバージョン（v0.9.18）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.dmg)**

> 推奨：常に最新バージョンのソフトウェアをダウンロードして、最高の機能体験と安定性を享受してください。
{.is-info}

## 🎬 インストールと使用のプロセス

### Windowsシステムのインストールと使用手順

#### 1. インストーラーをダブルクリックしてソフトウェアをインストールする

<img src="/eng/maxmakelab/media/maxmakelab-installation/1-双击安装软件.webp" alt="インストーラーをダブルクリックしてソフトウェアをインストール" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 2. ソフトウェアを開く

<img src="/eng/maxmakelab/media/maxmakelab-installation/2-打开软件.webp" alt="ソフトウェアを開く" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 3. 自動接続をクリックしてデバイスを見つけ、接続後に原点復帰をクリックする

<img src="/eng/maxmakelab/media/maxmakelab-installation/3-自动连接，点击回零.webp" alt="自動接続してデバイスを見つける" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

#### 4. デバイスを選択し、シリアルポートを手動で選択して接続することもできます

<img src="/eng/maxmakelab/media/maxmakelab-installation/4-手动连接.webp" alt="手動でデバイスを接続" style="width: 800px; height: auto; margin-bottom: 8px; border-radius: 16px;" />

<!-- ### macOS System Installation and Usage Steps

#### 1. Download and install the software

> 📥 **Download and Install**:
> 
> - Download the Mac version installer from the official website
> - Double-click the .dmg file to open the image
> - Drag MaxmakeLab to the Applications folder
> - Authorization required in system preferences during first run

#### 2. Open the software

> 🚀 **Start Software**:
> 
> - Open MaxmakeLab from Launchpad or Applications folder
> - If security prompt appears, hold Control key and click to select "Open"
> - Wait for software to fully load

#### 3. Click auto-connect to find device, and click return to zero after connection

> 🔌 **Device Connection**:
> 
> - Click the "Auto Connect" button
> - Wait for software to search for devices
> - After successful connection, click "Return to Zero" operation
> - Confirm device status is normal

#### 4. You can also select device and manually select serial port to connect

> ⚙️ **Manual Connection**:
> 
> - Select your device from the device list
> - Manually enter or select the serial port number
> - Click the connect button to establish connection
> - Verify connection status -->

## ⚠️ 重要な注意事項

> 🔍 **デバイス接続の問題**：
> 
> デバイスが見つからない場合：
> 1. ソフトウェアを再起動してみてください
> 2. USBデータケーブルを抜いて再接続してみてください
> 3. デバイスの電源が適切に入っているか確認してください
> 4. 正しいドライバーがインストールされていることを確認してください
> 
> {.is-warning}

> ⚡ **電気的安全性**：
> 
> - USBデータケーブルの接続がしっかりしていることを確認してください
> - データ転送中の切断を避けてください
> - USBポートが正常に動作しているか確認してください
> 
> 🛡️ **システム互換性**：
> - オペレーティングシステムのバージョンが要件を満たしていることを確認してください
> - （必要な場合）管理者としてソフトウェアを実行してください
> - 同種の潜在的に競合するソフトウェアを閉じてください
> 
> 🔧 **トラブルシューティング**：
> - ソフトウェアと機器を再起動してから再試行してください
> - デバイスマネージャーでドライバーの状態を確認してください
> - 異なるUSBポートを試してみてください
> {.is-info}

## ❓ よくある質問

### Windowsシステムの問題

### Q: インストール中にエラーが発生した場合はどうすればよいですか？
A: コンピュータがシステム要件を満たしていることを確認し、他の潜在的に競合するソフトウェアを閉じ、インストーラーを再ダウンロードして再インストールしてみてください。

### Q: 起動後にソフトウェアが応答しないのはなぜですか？
A: コンピュータに最新のグラフィックドライバーがインストールされているか確認し、管理者としてソフトウェアを実行してみてください。

### macOSシステムの問題

### Q: macOSシステムで「未確認の開発者からのため開くことができません」と表示されるのはなぜですか？
A: Controlキーを押しながらアプリケーションアイコンをクリックし、「開く」を選択してから、ポップアップダイアログでもう一度「開く」をクリックしてください。

### Q: macOSシステムでデバイスが認識されないのはなぜですか？
A:
1. 最新バージョンのmacOSがインストールされていることを確認してください
2. USBデータケーブルの接続が安定しているか確認し、USBポートを変更してみてください
3. 「システム環境設定」→「セキュリティとプライバシー」→「一般」を開き、MaxmakeLabのUSBアクセス権限が承認されていることを確認してください
4. ソフトウェアと機器を再起動してみてください

### 一般的な問題

### Q: デバイスが正常に接続されるが制御できないのはなぜですか？
A: USBデータケーブルが intact であるか確認し、データケーブルまたはUSBポートを交換してみてください、デバイスの電源が適切に入っていることを確認してください。

### Q: ソフトウェアのインターフェースが異常に表示されるのはなぜですか？
A: コンピュータに最新のグラフィックドライバーがインストールされているか確認するか、表示解像度を推奨値に調整してください。

---