# NXポストプロセッサのインストールガイド

この文書では、Siemens NXソフトウェアにHiMillシリーズのポストプロセッサをインストールするための詳細な手順を提供します。

---

## 📋 インストール手順

### ステップ1：ポストプロセッサファイルを解凍する

1. [ポストプロセッサダウンロードページ](/en/post-processors.md)からNXポストプロセッサパッケージをダウンロードします
2. 圧縮パッケージを解凍すると、3つのファイルが得られます

<img src="/eng/himill-d1-d1s/media/post/1解压.png" alt="ポストプロセッサファイルを解凍" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ2：ポストプロセッサファイルをNXインストールディレクトリにコピーする

1. Siemens NXソフトウェアのインストールパスを開きます
2. ポストプロセッサのデフォルトインストール場所を見つけます：
   ```
   X:\Program Files\Siemens\NX 12.0\MACH\resource\postprocessor
   ```
   *注：XはNXソフトウェアをインストールしたドライブ文字を表し、12.0はNXソフトウェアのバージョンを表します*
3. 解凍した3つのポストプロセッサファイルをこのディレクトリに貼り付けます

<img src="/eng/himill-d1-d1s/media/post/2复制.png" alt="ポストプロセッサファイルをコピー" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ3：template_post.datファイルを編集する

1. postprocessorディレクトリで`template_post.dat`ファイルを見つけて右クリックします
2. 「プログラムを指定して開く」→「メモ帳」を選択します

<img src="/eng/himill-d1-d1s/media/post/3添加命令.png" alt="template_post.datファイルを編集" style="width: 80%; height: auto; margin-bottom: 8px; border-radius: 16px;" />

### ステップ4：ポストプロセッサの設定を追加する

1. `template_post.dat`ファイルの末尾に新しい行を追加します
2. 以下の内容を貼り付けます：
   ```
   HiMill,${UGII_CAM_POST_DIR}HiMill.tcl,${UGII_CAM_POST_DIR}HiMill.def
   ```
3. ファイルを保存して閉じます

---

## ✅ インストールの確認

上記の手順を完了した後、NXソフトウェアのポストプロセッサリストから「HiMill」ポストプロセッサを選択して、HiMillシリーズの機械に適したGコードを生成することができます。

---

## 💡 注意事項

- お使いのNXソフトウェアのバージョンと互換性のあるポストプロセッサを使用してください
- NXソフトウェアのデフォルトインストールパスを変更した場合は、実際のパスに従って操作してください
- ポストプロセッサをインストールするときは、ファイルの占有を避けるためにNXソフトウェアが実行されていないことを確認してください

---

## 🔗 関連リンク

- [ポストプロセッサダウンロードページ](/en/post-processors.md)
- [HiMillシリーズ機械の使用ガイド](/en/himill-d1-d1s/hmd1-first-use.md)