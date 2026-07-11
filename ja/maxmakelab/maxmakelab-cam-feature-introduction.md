# MaxmakeLab CAM機能紹介ページ

MaxmakeLAB-0.9.18バージョンアップデートでは、CAM関連機能が新たに追加されました：ストック設定、ツールライブラリ管理、プロファイルミリング、ポケットミリング、レリーフ加工の3つのツールパス戦略、およびシミュレーション機能です。各機能の紹介は以下の通りです。

## 1. ストック設定（Job Step）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/毛坯设置.webp" alt="ストック設定デモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- ストックの幅、奥行き、高さを設定可能
- 加工原点は現在、頂点がデフォルトです。底面を原点とする機能は今後追加されます
- 原点位置を設定：中心点または左下隅点
- 加工安全高さを設定可能

## 2. ツールライブラリ（Tool Library）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/刀具库.webp" alt="ツールライブラリデモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- ツールパラメータを変更可能：
  - ツール番号、単位、直径など
  - ステップダウン、ステップオーバー、スピンドル速度、送り速度、プランジ速度など
- グループの追加、ツールの追加、ツールまたはグループのコピー/削除が可能

> ⚠️ **注意事項**：
>
> - インポート/エクスポート機能は現在問題があり、今後修正されます
> - 現在サポートされているツール：フラットエンドミル、ボールノーズエンドミル、フラットチップVビット、Vビット。他のツール種類は今後追加されます
> - 現在1つの材料しか表示されません。今後追加されます
>
> {.is-warning}

## 3. プロファイルミリング（Profile Toolpath）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/轮廓铣.webp" alt="プロファイルミリングデモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- ベクターを選択後、プロファイルパスを生成可能
- 加工深度を設定可能。加工開始高さは今後追加されます
- ツールライブラリからツールを選択可能で、一時的なパラメータ変更もサポート（ツールライブラリのパラメータには影響しません）
- ベクター外側、ベクター上、ベクター内側の3つの方式を選択可能
- クライムミリングまたはコンベンショナルミリングを選択可能
- ランプ機能、ブリッジ機能は今後追加されます

## 4. ポケットミリング（Pocket Toolpath）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/平面铣.webp" alt="ポケットミリングデモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- ベクターを選択後、ポケットパスを生成可能
- 加工深度を設定可能。加工開始高さは今後追加されます
- ツールライブラリからツールを選択可能で、一時的なパラメータ変更もサポート（ツールライブラリのパラメータには影響しません）
- ランプ機能、第2ツール残材加工機能は今後追加されます

## 5. レリーフ加工（Relief Toolpath）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/浮雕加工.webp" alt="レリーフ加工デモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- 画像を選択後、レリーフパスを生成可能
- 加工深度を設定可能。現在設定後、レリーフの高さとなります
- ツールライブラリからツールを選択可能で、一時的なパラメータ変更もサポート（ツールライブラリのパラメータには影響しません）
- デフォルトで図形のエッジをオフセットした後に粗加工を行います。境界制限オプションは今後追加されます
- ランプ機能は今後追加されます

> ⚠️ **注意事項**：
>
> - レリーフ機能は現在、粗加工の余裕代が多めに設定されています。檀木などの硬木での加工は推奨されません。今後この機能は最適化されます
>
> {.is-warning}

## 6. シミュレーション（Simulate）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/仿真加工.webp" alt="シミュレーションデモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- パス生成後、シミュレートボタンをクリックして加工シミュレーションを表示可能
- パスの表示をオン/オフ可能
- 再生速度を調整し、プログレスバーをドラッグして素早く確認可能
- ドラッグ時にパスがレンダリングされない問題があります。今後修正されます

## 7. エクスポート（Export）

<img src="/eng/maxmakelab/maxmakelab-cam-feature-introduction/导出.webp" alt="エクスポートデモ" style="width: 100%; height: auto; margin-bottom: 4px; border-radius: 16px;" />

- パス生成後、エクスポートボタンをクリックしてGコードをNC形式でエクスポート可能
- 機械に接続してゼロリターンした状態で、直接機械にインポート可能

> ⚠️ **注意事項**：
>
> - エクスポート時、パスは現在分散しています。変更しないことを推奨します。今後この機能は最適化されます
> - コードには常にツール交換コードT\*M6が含まれているため、ツール交換をクリックし、高さ測定後にゼロ点を設定してからコードを実行する必要があります
>
> {.is-warning}

## 8. 問題フィードバック

ソフトウェアの問題がある場合は、Discordのソフトウェアフィードバック専用チャンネルでお問い合わせください。皆様のご意見を積極的に参考にし、問題を速やかに修正いたします：

- [Discord](https://discord.com/channels/1436232802227064903/1436232803061600351)