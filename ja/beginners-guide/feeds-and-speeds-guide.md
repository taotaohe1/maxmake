# デスクトップCNCの送りと速度の専門ガイド：アルミニウム、アクリル、PCB版

以下の動画は、デスクトップCNC機械でアルミニウム、アクリル、パターンウッド、PCB材料を加工するための最適な送りと速度設定をマスターするのを助ける包括的なビジュアルガイドを提供します。

<a href="https://youtu.be/z5gLhoAfKHs?si=HwYS7Ze0VyiGUzsy" target="_blank">
    <img src="https://img.youtube.com/vi/z5gLhoAfKHs/0.jpg" alt="動画を見るにはクリック" style="width: 50%; border-radius: 8px;">
</a>

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/标题.png" alt="デスクトップCNCの送りと速度の専門ガイド" style="width: 80%; height: auto; border-radius: 10px;" />

CNC加工中に工具の折れ、ワークのエッジの溶融、または加工表面のビビリマークに常に直面していませんか？Maxmaker D1SなどのデスクトップCNC機器でプロ級の結果を得るには、技術的なトリックに依存するのではなく、送り速度と主軸速度の精密な制御に核心的な鍵があります。

この包括的なガイドでは、アルミニウム、アクリル、パターンウッド、PCBボードを含む4つの主流加工材料について、テスト済みで検証されたパラメーターを解説します。

---

## 1. CNCアルミニウム加工：表面の滑らかさを実現し、工具の詰まりと切りくずの堆積を防止

アルミニウム加工は、すべてのデスクトップCNC彫刻機にとって究極の課題です。核心的な難しさは、金属の切りくずがカッターにくっつくのを防ぐことにあります。

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/cnc铝材加工.png" alt="CNCアルミニウム加工" style="width: 50%; height: auto; border-radius: 10px;" />

### 工具選択

**3刃タングステン鋼フライスカッター**の使用を強く推奨します。このカッターは優れた剛性と、切りくず排出効率を最適化するための十分なフルートスペースを提供します。

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/三刃钨钢铣刀.png" alt="3刃タングステン鋼フライスカッター" style="width: 50%; height: auto; border-radius: 10px;" />

### 核心加工パラメーター

| パラメーター | 推奨値 |
|-----------|--------|
| 主軸速度 | 12000-13000 RPM |
| 送り速度 | 100-200 mm/min |
| 1刃あたりの切り込み深さ（Ap） | 0.1-0.3 mm |

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/铝材加工参数.png" alt="アルミニウム加工パラメーター" style="width: 100%; height: auto; border-radius: 10px;" />

### 専門的な実用的なヒント

金属加工中は、常に切りくずの除去に注意してください。真空装置または高圧エアブラストを使用して切りくずを除去し、切りくずの再切削を避けるようにします。

---

## 2. CNCアクリル加工：鏡面の滑らかな切断表面を作成

アクリル加工におけるエッジの溶融と割れの問題を避けるための鍵は、高い送り速度を使用し、鋭い切削エッジを確保することです。

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/cnc亚克力加工.png" alt="CNCアクリル加工" style="width: 50%; height: auto; border-radius: 10px;" />

### 工具選択

**単刃スパイラルフライスカッター**を使用します。単刃の構造設計により、加工中に発生する熱をより速く放散させることができます。

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/单刃螺旋铣刀.png" alt="単刃スパイラルフライスカッター" style="width: 20%; height: auto; border-radius: 10px;" />

### 核心加工パラメーター

| パラメーター | 推奨値 |
|-----------|--------|
| 主軸速度 | 10000-13000 RPM |
| 送り速度 | 600-800 mm/min（高送り速度が熱の蓄積を効果的に防止！） |
| 1刃あたりの切り込み深さ | 0.5-1.0 mm |

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/亚克力加工参数.png" alt="アクリル加工パラメーター" style="width: 100%; height: auto; border-radius: 10px;" />

### 専門的な実用的なヒント

加工中にアクリルに溶融の兆候が現れた場合は、送り速度を適切に上げるか、主軸速度を下げてください。

---

## 3. パターンウッドと合成材料の加工

高詳細なモデルと金型加工の要件に対して、パターンウッドは好ましい加工材料です。

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/模具木加工.png" alt="パターンウッド加工" style="width: 50%; height: auto; border-radius: 10px;" />

### 工具選択

**2刃ソリッドカーバイドフラットエンドミル**

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/双刃平底立铣刀.png" alt="2刃フラットエンドミル" style="width: 50%; height: auto; border-radius: 10px;" />

### 核心加工パラメーター

| パラメーター | 推奨値 |
|-----------|--------|
| 主軸速度 | 12000-13000 RPM |
| 送り速度 | 1000 mm/min |
| 1刃あたりの切り込み深さ（Ap） | 1.0-3.0 mm（これらの材料は切削抵抗が低い） |

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/模具木加工参数.png" alt="パターンウッド加工パラメーター" style="width: 100%; height: auto; border-radius: 10px;" />

### 専門的な実用的なヒント

加工中は、D1Sの内蔵磁気ブラシを有効にするか、家庭用掃除機を接続して補助的な切りくず除去を行ってください。これにより、微細な粉塵がボールネジに付着するのを防ぎ、機器の長期的な加工精度への影響を回避します。

---

## 4. PCBボードの精密彫刻：ミクロンレベルの加工精度を実現

Maxmaker D1Sは±0.02mmの繰り返し精度を実現し、PCBボードのプロトタイプ加工において優れたパフォーマンスを発揮します。

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/pcb板雕刻.png" alt="PCBボード彫刻" style="width: 50%; height: auto; border-radius: 10px;" />

### 工具選択

**フラットボトムポインテッドカッター**（≤45°、精密なルーティング用）
**コーンフライスカッター**（容易な切断用）

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/玉米铣刀.png" alt="コーンフライスカッター" style="width: 50%; height: auto; border-radius: 10px;" />

### 核心加工パラメーター

| パラメーター | 推奨値 |
|-----------|--------|
| 主軸速度 | 12000-13000 RPM |
| 送り速度 | 800-1000 mm/min |
| 1刃あたりの切り込み深さ（Ap） | 0.05-0.2 mm |

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/pcb加工参数.png" alt="PCB加工パラメーター" style="width: 100%; height: auto; border-radius: 10px;" />

### 核心加工技術

機器の**オートレベリング機能**を有効にします。彫刻前に、PCBボードの表面プロービング検出を実行します。ソフトウェアは表面の平坦度エラーを自動的に補償し、彫刻深さを一貫して0.05mmに安定させ、加工精度の一貫性を実現します。

---

## まとめ：デスクトップCNC加工の核心パラメーター要約表

<img src="/eng/beginners-guide/media/feeds-and-speeds-guide/参数汇总表.jpg" alt="パラメーター要約表" style="width: 100%; height: auto; border-radius: 10px;" />

| 材料 | 主軸速度（RPM） | 送り速度（mm/min） | 1刃あたりの切り込み深さ（mm） | 推奨工具 |
|------|----------------|-------------------|-------------------|----------|
| **アルミニウム** | 12000-13000 | 100-200 | 0.1-0.3 | 3刃タングステン鋼フライスカッター |
| **アクリル** | 10000-13000 | 600-800 | 0.5-1.0 | 単刃スパイラルフライスカッター |
| **パターンウッド** | 12000-13000 | 1000 | 1.0-3.0 | 2刃フラットエンドミル |
| **PCBボード** | 12000-13000 | 800-1000 | 0.05-0.2 | コーンフライスカッター |

---

## デスクトップスマート製造ワークショップをアップグレードし、効率的な加工体験を解き放て！

CNC加工のマスターは一日で達成されるものではありませんが、適切な専門機器を選択することで、加工の旅を2倍効率的にすることができます。

- [D1SデスクトップCNC機械](/eng/himill-d1s.md)を探索
- [CNC工具パラメーター表](/eng/tool-parameters.md)を参照

---

*📝 このドキュメントは継続的に更新されています。ご意見や質問がある場合は、お気軽にお問い合わせください。*