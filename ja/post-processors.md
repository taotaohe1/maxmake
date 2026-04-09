# HiMillシリーズのポストプロセッサーダウンロード

このドキュメントは、MAXMAKE HiMillシリーズCNC機械と互換性のあるポストプロセッサーのダウンロードサービスを提供します。主流のCAMソフトウェア用に最適化されたポストプロセッサーを継続的に追加しています。このページでリアルタイムに更新が可能です。

## 3軸ポストプロセッサー一覧

| 名前 | 互換ソフトウェア | ダウンロードリンク |
|------|-------------------|---------------------|
| Fusion360ポストプロセッサー | Autodesk Fusion 360 | <a href="/eng/himill-d1-d1s/media/post/fusion360.zip" target="_blank" rel="noopener noreferrer">ダウンロード</a> |
| Vectricポストプロセッサー | Vectric VCarve / Aspire / Cut2D | <a href="/eng/himill-d1-d1s/media/post/vectric.zip" target="_blank" rel="noopener noreferrer">ダウンロード</a> |
| Kiri:motoポストプロセッサー | Kiri:moto | <a href="/eng/himill-d1-d1s/media/post/kiri-moto.zip" target="_blank" rel="noopener noreferrer">ダウンロード</a> |
| Estlcamポストプロセッサー | Estlcam | <a href="/eng/himill-d1-d1s/media/post/estlcam-maxmake.zip" target="_blank" rel="noopener noreferrer">ダウンロード</a> |
| NXポストプロセッサー | Siemens NX | <a href="/eng/himill-d1-d1s/media/post/nx.zip" target="_blank" rel="noopener noreferrer">ダウンロード</a> · <a href="/ja/himill-d1-d1s/hmd1-nx-postprocessor-installation.md" target="_blank" rel="noopener noreferrer">インストールガイド</a> |

## 4軸ポストプロセッサー一覧

| 名前 | 互換ソフトウェア | ダウンロードリンク |
|------|-------------------|---------------------|
| Fusion360 4軸ポストプロセッサー | Autodesk Fusion 360 | <a href="/eng/himill-d1-d1s/media/post/fusion360-4axis.zip" target="_blank" rel="noopener noreferrer">ダウンロード（ベータ版）</a> |
| Vectric 4軸ポストプロセッサー | Vectric VCarve / Aspire / Cut2D | <a href="/eng/himill-d1-d1s/media/post/vectric-y2a.zip" target="_blank" rel="noopener noreferrer">ダウンロード</a> |

## 使用方法

1. お使いのCAMソフトウェアに対応するポストプロセッサーの圧縮ファイルをダウンロードします
2. ダウンロードした圧縮ファイルを解凍して、ポストプロセッサーファイルを取得します
3. お使いのCAMソフトウェアのポストプロセッサー追加方法に従って、ポストプロセッサーファイルをインストールします
4. Gコードを生成する際に、「MAXMAKE HiMill」ポストプロセッサーを選択します
5. 生成されたGコードは、HiMillシリーズ機械でそのまま使用できます

## 注意事項

HiMillシリーズ機械は、ツール交換コマンドに特定の要件があります：

- 機械は、`T*M6`形式のツール交換コマンドのみを**サポート**します
- `G43H**`形式のツール長補正コマンドは**サポートしません**

したがって、**公式以外のポストプロセッサー**または**カスタムポストプロセッサー**（このページで提供されていないもの）を使用する場合は、生成されたGコードを確認してください：

1. すべてのツール交換コマンド（`T*M6`）を見つけます
2. これらのツール交換コマンドの後に`G43H**`コマンドがあるかどうかを確認します
3. このようなコマンドが存在する場合は、Gコードを使用する前に手動で削除してください

このページで提供されている公式ポストプロセッサーを使用して生成されたGコードは、HiMill機械用に最適化されており、追加の変更は必要ありません。

### 半自動ツール交換機構

HiMillシリーズ機械は、**半自動ツール交換**システムを使用しています。以下の特徴があります：

- Gコードでは`T1M6`、`T2M6`、`T3M6`などのコマンドを使用して異なるツールを区別しますが、機械ファームウェアの処理ロジックでは常に単一のツールとして扱います
- 各ツール交換コマンドの後、機械は自動的にツール高さ測定を実行し、測定結果に基づいてツール高さ補正値を調整します

#### 操作ルール

正しいツール補正の適用を確保するために、加工前に以下の手順を厳密に実行してください：

1. まず「ツール交換」ボタンをクリックしてツール交換モードに入ります
2. 最初のツールを取り付けて確認します
3. 機械が自動高さ測定を完了するのを待ちます
4. **高さ測定が完了した後**、Z軸のゼロ点（Z0）を設定します

詳細なツール交換操作手順については、[ツール取り付けページ](/ja/himill-d1-d1s/hmd1-tool-installation.md)を参照してください。