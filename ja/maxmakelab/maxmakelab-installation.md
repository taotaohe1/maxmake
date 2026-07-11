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

> ℹ️ **バージョン0.9.18更新内容**：
> 1. テキスト機能のアップグレード：テキスト作成機能の最適化
> 2. 新しいツールライブラリ機能：ツールライブラリにツールを追加可能、ツールパス生成時にパラメータを再編集可能
> 3. ストック設定機能の最適化：ストック設定後、機械の加工領域内にストックサイズを表示する2D領域を追加、領域内に図形を追加可能
> 4. 新しいプロファイルミリング、ポケットミリング、グレースケールレリーフ戦略を追加
> 5. 新しいシミュレーションプレビュー：ツールパス生成後に加工シミュレーションをサポート
> {.is-info}


>  ⚠️ **注意事項**：
>  1. ツールパラメータライブラリは現在、ツールが1つの材料にのみ対応しています。複数材料切り替え機能は今後更新されます。ソフトウェアには現在、軟材加工用のパラメータセットが組み込まれています。
>  2. ツールパラメータライブラリは現在、以下のツールをサポートしています：フラットエンドミル、ボールノーズエンドミル、フラットチップVビット、Vビット。他のツール種類は今後追加されます。
>  3. 現在、ツールパスは材料表面を起点として生成されます。開始高さ設定機能は今後更新されます。
>  4. ブリッジ機能は今後更新されます。
>  5. ランプ機能は今後更新されます。したがって、現在は軟材などの材料の加工のみサポートされています。硬材や金属の加工は推奨されません。
>  6. レリーフ機能は現在、粗加工の余裕代が多めに設定されています。檀木などの硬材での加工は推奨されません。今後この機能は最適化されます。
>  7. Gコード生成：生成されたコードには最初のツール交換コードが含まれます。したがって、加工前にはソフトウェア内でツール交換をクリックし、高さ測定後にZ0を設定してから加工を開始してください。（必ず実行してください。そうしないと加工エラーまたは加工高さエラーが発生します）
>  8. ソフトウェアの問題がある場合は、Discordのソフトウェアフィードバック専用チャンネルでお問い合わせください。皆様のご意見を積極的に参考にし、問題を速やかに修正いたします：[Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)
>  {.is-warning}

### 最新バージョン（v0.9.18）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.18.dmg)**

### 以前のバージョン（v0.9.17）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.17.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.17.dmg)**

### 以前のバージョン（v0.9.16）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.16.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.16.dmg)**

### 以前のバージョン（v0.9.15）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.15.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.15.dmg)**

### 以前のバージョン（v0.9.14）
**[MaxmakeLabソフトウェアダウンロードリンク(Windows)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.14.exe)**
**[MaxmakeLabソフトウェアダウンロードリンク(macOS)](https://assets.maxmake.com/Maxmakelab/software/MaxmakeLAB_v0.9.14.dmg)**

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