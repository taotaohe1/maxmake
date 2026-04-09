# 📋 ソフトウェアエラークエリ

> このページでは、HiMill D1/D1s機器のすべてのソフトウェアエラー情報を整理し、ユーザーが機器の故障問題を迅速に特定して解決するのを支援します。

---

## 📊 概要情報

| エラータイプ | 件数 | 説明 |
|-----------|-------|-------------|
| 🚨 **アラームエラー（ALARM）** | 14 | 機器のハードウェアまたは安全関連のアラーム情報 |
| ❌ **エラーメッセージ（ERROR）** | 85 | ソフトウェアコマンド、パラメータ設定関連のエラー |

---

## 🚨 アラームエラー（ALARM）

> **説明**：これらのエラーは通常、機器のハードウェア状態、安全設定、センサー機能に関連しており、優先的に処理する必要があります。

| エラーコード | エラー名 | 故障原因 | 解決策 |
|------------|------------|-------------|----------|
| ALARM | Please home the machine. |  |  |
| ALARM1 | Hard limit has been triggered. | 1.衝突によりモーターの位置同期が失われ、その後の移動中にリミットスイッチがトリガーされる。<br>2.手や異物が誤ってリミットスイッチに接触する。<br>3.モーターの動作異常によりリミットスイッチが誤トリガーされる。<br>4.リミットスイッチの故障。 | 1.原点復帰が必要です。同時に、治具、ワークピースの取り付け、主軸の取り付け高さ、加工ファイルのパスを確認してください。<br>2.原点復帰が必要です。物体の衝突によりリミットスイッチが誤ってトリガーされた場合は、異物を取り除いてください。使用中は安全に注意し、機器が動いている間に手やその他の物体を機器内に挿入しないでください。<br>3.モーターの動作が異常かどうか（異常な振動、完全な停止、一方向のみの移動など）を確認してください。詳細については、ヘルプドキュメントを参照してください。<br>4.「デバイス設定」-「検出」インターフェースに入り、リミットスイッチが故障しているかどうかを判断してください。故障している場合は、適切な時期に交換してください。 |
| ALARM2 | Motion target exceeds machine travel. Alarm during streaming of SD file at line: XXX | 実行された動作コードの目標位置が機器のストロークを超えている。 | GコードのXYZ軸の移動パラメータが移動範囲を超えていないか確認してください。原点復帰を行ってください。 |
| ALARM2 | Motion target exceeds machine travel. | 実行された動作コードの目標位置が機器のストロークを超えている。 | GコードのXYZ軸の移動パラメータが移動範囲を超えていないか確認してください。原点復帰を行ってください。 |
| ALARM3 | Reset/E-stop while in motion. | 1.非常停止ボタンが押された。<br>2.移動中にリセットされた。 | 1.非常停止を解除し、原点復帰が必要です。<br>2.原点復帰後に操作を続けてください |
| ALARM4 | Probe fail, The tool setter was triggered before probing. | 1.プロービング前にツールセッターが押された。<br>2.ツールセッターが損傷している。 | 1.異物を取り除いてツールセッターを解放してください。操作の安全性に注意し、機器の動作中に手やその他の物体を機器内に入れないでください。<br>2.「デバイス設定」-「検出」インターフェースに入り、ツールセッターが故障しているかどうかを判断してください。故障している場合は、適切な時期に交換してください。 |
| ALARM4 | Probe fail, The 3D Probe was triggered before probing. | 1.プローブのワイヤーインターフェースが適切に挿入されていない<br>2.3Dプローブの故障。<br>3.プロービング前に3Dプローブが既にトリガー状態にある（インジケーターライトが赤色）。 | 1.3Dプローブの接続ケーブルがしっかりと接続されているか確認してください（完全に挿入されていることを確認）。<br>2.「デバイス設定」-「検出」インターフェースに入り、3Dプローブが故障しているかどうかを判断してください。<br>3.プロービングを開始する前に、3Dプローブが非トリガー状態（インジケーターライトが緑色）であることを確認してください。注意！プローブが現在物体に接触している場合は、まず物体を取り除いてから再ゼロ設定を行ってください。3Dプローブの損傷を避けるためです。 |
| ALARM5 | Probe fail. The tool setter was not triggered within the probing travel. | 1.工具が短すぎるか、主軸の取り付け位置が高すぎて、検出範囲内でツールセッターをトリガーできない。<br>2.ツールセッターの損傷。 | 1.主軸の高さまたは工具の取り付け高さを調整することができます。<br>2.「デバイス設定」-「検出」インターフェースに入り、ツールセッターが故障しているかどうかを判断してください。故障している場合は、適切な時期に交換してください。 |
| ALARM5 | Probe fail. The 3D Probe was not triggered within the probing travel. | 1.プローブがワークピースから離れすぎているか、設定されたプロービング距離が短すぎる。<br>2.3Dプローブが故障している。 | 1.プローブをワークピースに近づけるか、プロービング距離を増やしてください。<br>2.「デバイス設定」-「検出」インターフェースに入り、3Dプローブが故障しているかどうかを判断してください。 |
| ALARM6 | Homing fail. The active homing cycle was reset. |  |  |
| ALARM7 | Homing fail. Safety door was opened during homing cycle. | 原点復帰プロセス中に誤って安全ドアを開けた | 原点復帰プロセス中は安全ドアを閉じたままにしてください |
| ALARM8 | Homing fail. Pull off travel failed to clear limit switch. | 1.リミットスイッチが故障している。<br>2.モーターの動作が異常。 | 1.「デバイス設定」-「検出」インターフェースに入り、リミットスイッチが故障しているかどうかを判断してください。故障している場合は、適切な時期に交換してください。<br>2.モーターの動作が異常かどうか（大きな音と共に激しい振動、完全な停止、一方向のみの移動など）を確認してください。詳細については、「ヘルプ」ページの「モーターが正常かどうかの確認方法」を参照してください。<br>3.もう一度原点復帰を試みることができます。 |
| ALARM9 | Homing fail. Could not find limit switch within search distances. | 1.衝突が発生し、動きが妨げられた。<br>2.リミットスイッチが故障している。<br>3.モーターの動作が異常。 | 1.障害物を取り除いてから、もう一度原点復帰を行ってください。<br>2.「デバイス設定」-「検出」インターフェースに入り、リミットスイッチが故障しているかどうかを判断してください。故障している場合は、適切な時期に交換してください。<br>3.モーターの動作が異常かどうか（大きな音と共に激しい振動、完全な停止、一方向のみの移動など）を確認してください。詳細については、「ヘルプ」ページの「モーターが正常かどうかの確認方法」を参照してください。 |
| ALARM10 | EStop asserted. | 非常停止ボタンが押されている。 | 非常停止ボタンを解除した後、原点復帰が必要です。 |
| ALARM11 | Homing required. | 現在の位置に同期ずれがある可能性がある。 | 原点復帰が必要です。 |
| ALARM12 | Limit switch engaged. Clear before continuing. | 1.リミットスイッチが故障している。<br>2.モーターの動作が異常。 | 1.「デバイス設定」-「検出」インターフェースに入り、リミットスイッチが故障しているかどうかを判断してください。故障している場合は、適切な時期に交換してください。<br>2.モーターの動作が異常かどうか（大きな音と共に激しい振動、完全な停止、一方向のみの移動など）を確認してください。詳細については、「ヘルプ」ページの「モーターが正常かどうかの確認方法」を参照してください。<br>3.もう一度原点復帰を試みることができます。 |
| ALARM13 | Probe protection triggered. Clear before continuing. |  |  |

---

## ❌ エラーメッセージ（ERROR）

> **説明**：これらのエラーは主にGコードコマンド、パラメータ設定、ファイル操作などに関わり、プログラムコードとパラメータ設定の確認が必要です。

### 📝 Gコード関連エラー（ERROR1-ERROR39）

| エラーコード | エラー名 | 故障原因 | 解決策 |
|------------|------------|-------------|----------|
| ERROR1 | G-code words consist of a letter and a value. Letter was not found. Error in SD file at line XXX. | Gコードの形式が正しくなく、文字が欠落している。 | Gコードの形式が正しいか確認してください。 |
| ERROR1 | G-code words consist of a letter and a value. Letter was not found. |  |  |
| ERROR2 | Missing the expected G-code word value or numeric value format is not valid. Error in SD file at line XXX. | 1.入力値の形式が正しくない。<br>2.Gコードの記述時に値が欠落している。 | 1.Gコードの値の範囲と形式が正しいか確認してください。<br>2.Gコードを注意深く確認し、欠落している値を補完してください。 |
| ERROR2 | Missing the expected G-code word value or numeric value format is not valid. |  |  |
| ERROR3 | '$' system command was not recognized or supported. |  |  |
| ERROR4 | Negative value received for an expected positive value. Error in SD file at line XXX. | Gコードに負の値が誤って入力された。 | 1.Gコードの値の入力を確認し、要件を満たしていることを確認してください。<br>2.関連する計算ロジックを確認し、計算エラーを修正してください。 |
| ERROR4 | Negative value received for an expected positive value. |  |  |
| ERROR5 | Homing cycle failure. Homing is not configured via settings. |  |  |
| ERROR6 | Step pulse time must be greater or equal to 2 microseconds. |  |  |
| ERROR7 | A settings read failed. Auto-restoring affected settings to default values. |  | もう一度お試しください |
| ERROR8 | '$' command cannot be used unless controller state is IDLE. |  |  |
| ERROR9 | G-code locked out during alarm or jog state. |  |  |
| ERROR10 | Soft limits cannot be enabled without homing also enabled. |  |  |
| ERROR11 | Max characters per line exceeded. Line was not processed and executed. | 1.Gコードの1行の文字数が過多。<br>2.ファイルが破損している。<br>3.互換性のないポストプロセッサが使用されている。 | 1.長さを短くし、コードを合理化してください。<br>2.ファイルの正確性を確認してください。<br>3.ポストプロセッサを確認または交換してください。 |
| ERROR12 | '$' setting value cause the step rate to exceed the maximum supported. |  |  |
| ERROR13 | Safety door detected as opened and door state initiated. |  |  |
| ERROR14 | Build info or startup line exceeded EEPROM line length limit.Line not stored. |  |  |
| ERROR15 | Jog target exceeds machine travel. Command ignored. |  |  |
| ERROR16 | Jog command with no '=' or contains prohibited g-code. |  |  |
| ERROR17 | Laser mode requires PWM output. |  |  |
| ERROR18 | Reset asserted |  |  |
| ERROR19 | Non positive value |  |  |
| ERROR20 | Unsupported or invalid g-code command found in block. Error in SD file at line XXX. | 1.サポートされていないGコードコマンドが使用されている。<br>2.Gコードコマンドが誤って記述されている。 | 1.ポストプロセッサを確認または交換してください。<br>2.ファイルが破損している場合は、ファイル内容の整合性を確認してください。 |
| ERROR20 | Unsupported or invalid g-code command found in block. |  |  |
| ERROR21 | More than one g-code command from same modal group found in block. Error in SD file at line XXX. | コードブロック内で同じモーダルグループからの複数のコマンドが誤って使用されている（例：G1とG0が同じ行に存在する）。 | 1.同じモーダルグループでは1つのコマンドのみを使用するようにコードを確認してください。<br>2.モーダルグループの概念と使用ルールを学び、理解してください。<br>3.ポストプロセッサを確認または交換してください。 |
| ERROR21 | More than one g-code command from same modal group found in block. |  |  |
| ERROR22 | Feed rate has not yet been set or is undefined. Error in SD file at line XXX. | Gコードの記述時に送り速度の設定が省略された。 | 1.Gコードを確認し、送り速度F値が追加されているか確認してください（例：G1 X10 Y10 Z10 F500）。<br>2.ポストプロセッサを確認または交換してください |
| ERROR22 | Feed rate has not yet been set or is undefined. |  |  |
| ERROR23 | G-code command in block requires an integer value. Error in SD file at line XXX. | 値が整数でない。 | 1.Gコードの形式が正しいか確認してください。<br>2.コードを記述する際は、コマンドで指定された値の種類の要件に注意してください。<br>3.ポストプロセッサを確認または交換してください。 |
| ERROR23 | G-code command in block requires an integer value. |  |  |
| ERROR24 | More than one g-code command that requires axis words found in block. Error in SD file at line XXX. | XYZ軸を必要とする複数のコマンドが同時に誤って使用されている。 | 1.Gコードの形式を確認し、G0またはG1コマンドが分離されているか確認してください<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR24 | More than one g-code command that requires axis words found in block. |  |  |
| ERROR25 | Repeated g-code word found in block. Error in SD file at line XXX. | コードの記述中にGコードコマンドが繰り返されている。 | 1.Gコードの形式を確認し、重複したXYZ、F、Sコマンドを削除してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR25 | Repeated g-code word found in block. |  |  |
| ERROR26 | No axis words found in block for g-code command or current modal state which requires them. Error in SD file at line XXX. | コードの記述中にXYZ軸コマンドが省略されている。この問題は、弧命令G2とG3でよく発生する。 | 1.Gコードの形式を確認し、XYZ軸コマンドを補完してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR26 | No axis words found in block for g-code command or current modal state which requires them. |  |  |
| ERROR27 | Line number value is invalid. | 1.コードの記述時に設定されたN行番号が範囲外。<br>2.プログラムがN行番号を生成する際にエラーが発生した。 | 1.N行番号を有効な範囲内に調整してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR28 | G-code command is missing a required value word. Error in SD file at line XXX. |  | 1.Gコードの形式を確認し、欠落している値を補完してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR28 | G-code command is missing a required value word. |  |  |
| ERROR29 | G59.x work coordinate systems are not supported. |  |  |
| ERROR30 | G53 only allowed with G0 and G1 motion modes. Error in SD file at line XXX. |  | 1.Gコードの形式を確認し、G53が現在のモーダル状態がG0またはG1の場合にのみ使用されていることを確認してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR30 | G53 only allowed with G0 and G1 motion modes. |  |  |
| ERROR31 | Axis words found in block when no command or current modal state uses them. Error in SD file at line XXX. |  | 1.Gコードの形式を確認し、G80の後に軸コマンドがあるか確認してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR31 | Axis words found in block when no command or current modal state uses them. |  |  |
| ERROR32 | G2 and G3 arcs require at least one in-plane axis word. Error in SD file at line XXX. | 弧命令の記述時にXYZ軸パラメータが省略されている。 | 1.Gコードの形式を確認し、弧命令のXYZ軸パラメータを補完してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR32 | G2 and G3 arcs require at least one in-plane axis word. |  |  |
| ERROR33 | The motion command has an invalid target. Error in SD file at line XXX. | 1.G2/G3弧を生成できない。<br>2.プローブの目標が現在の位置と一致している。 | 1.弧パラメータを確認し、弧を生成できるようにしてください。<br>2.プローブの目標をリセットし、現在の位置と一致しないようにしてください。<br>3.ポストプロセッサを確認または交換してください。 |
| ERROR33 | The motion command has an invalid target. |  |  |
| ERROR34 | A G2 or G3 arc, traced with the radius definition, had a mathematical error when computing the arc geometry. Error in SD file at line XXX. | 弧の半径パラメータが正しくない。 | 1.半径設定を調整し、計算が合理的になるようにしてください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR34 | A G2 or G3 arc, traced with the radius definition, had a mathematical error when computing the arc geometry. |  |  |
| ERROR35 | A G2 or G3 arc, traced with the offset definition, is missing the IJK offset word in the selected plane to trace the arc. Error in SD file at line XXX. | オフセット定義を使用した弧命令の記述時にIJKパラメータが省略されている。 | 1.Gコードの形式を確認し、IJKオフセットパラメータを補完してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR35 | A G2 or G3 arc, traced with the offset definition, is missing the IJK offset word in the selected plane to trace the arc. |  |  |
| ERROR36 | There are unused, leftover G-code words that aren't used by any command in the block. Error in SD file at line XXX. | 1.高速移動命令G00に余分なHパラメータが含まれている。<br>2.主軸起動命令M3に余分なDパラメータが含まれている。<br>3.単位設定命令G21に余分なPパラメータが含まれている。<br>4.円弧補間命令G02に余分なSパラメータが含まれている。 | 1.Gコードの形式を確認し、不要なGコードパラメータを削除してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR36 | There are unused, leftover G-code words that aren't used by any command in the block. |  |  |
| ERROR37 | The G43.1 dynamic tool length offset command cannot apply an offset to an axis other than its configured axis. The Grbl default axis is the Z-axis. |  |  |
| ERROR38 | Tool number greater than max supported value or undefined tool selected. Error in SD file at line XXX. | 入力された工具番号が存在しないか、形式が正しくない。 | 1.入力された工具番号が有効で形式が正しいことを確認してください。<br>2.工具番号はT0〜T8の範囲に設定することをお勧めします。 |
| ERROR38 | Tool number greater than max supported value or undefined tool selected. |  |  |
| ERROR39 | Value out of range. Error in SD file at line XXX. |  |  |
| ERROR39 | Value out of range. |  |  |

### 🔧 機器関連エラー（ERROR40-ERROR58）

| エラーコード | エラー名 | 故障原因 | 解決策 |
|------------|------------|-------------|----------|
| ERROR40 | G-code command not allowed when tool change is pending. Error in SD file at line XXX. |  |  |
| ERROR40 | G-code command not allowed when tool change is pending. |  |  |
| ERROR41 | Spindle not running when motion commanded in CSS or spindle sync mode. Error in SD file at line XXX. |  |  |
| ERROR41 | Spindle not running when motion commanded in CSS or spindle sync mode. |  |  |
| ERROR42 | Plane must be ZX for threading. Error in SD file at line XXX. |  |  |
| ERROR42 | Plane must be ZX for threading. |  |  |
| ERROR43 | Max. feed rate exceeded. Error in SD file at line XXX. |  |  |
| ERROR43 | Max. feed rate exceeded. |  |  |
| ERROR44 | RPM out of range. Error in SD file at line XXX. |  |  |
| ERROR44 | RPM out of range. |  |  |
| ERROR45 | Only homing is allowed when a limit switch is engaged. |  |  |
| ERROR46 | Home machine to continue. |  |  |
| ERROR47 | ATC: current tool is not set. Set current tool with M61. |  |  |
| ERROR48 | Value word conflict. |  |  |
| ERROR49 | Power on self test failed. A hard reset is required. |  |  |
| ERROR50 | Emergency stop active. |  |  |
| ERROR51 | Motor fault. |  |  |
| ERROR52 | Setting value is out of range. |  |  |
| ERROR53 | Setting is not available, possibly due to limited driver support. |  |  |
| ERROR54 | Retract position is less than drill depth. |  | 1.Gコードの形式を確認し、R座標がZ座標より大きいことを確認してください。<br>2.ポストプロセッサを確認または交換してください。 |
| ERROR54 | Retract position is less than drill depth. |  |  |
| ERROR55 | Attempt to home two auto squared axes at the same time. |  |  |
| ERROR56 | Coordinate system is locked. |  |  |
| ERROR57 | Unexpected file demarcation. |  |  |
| ERROR58 | Port is not available |  |  |

### 💾 SDカード関連エラー（ERROR60-ERROR66）

| エラーコード | エラー名 | 故障原因 | 解決策 |
|------------|------------|-------------|----------|
| ERROR60 | Status_SDMountError | 1.SDカードの接触不良。<br>2.SDカードの損傷<br>3.SDカードの形式がサポートされていない<br>4.ファームウェアがSDカードを認識してマウントできない | 1.機器を再起動してください。問題が解決しない場合は、SDカードのフォーマットを試してください。<br>2.SDカードが損傷している場合は、SDカード交換のチュートリアルを参照してください。 |
| ERROR61 | Status_FileReadError | 1.対象ファイルが破損している。<br>2.ファイルパスが正しくない。<br>3.読み取り中にSDカードの接続が中断された。<br>4.ファイル内容が期待される形式に準拠していない。 | 1.機器を再起動してもう一度試してください。<br>2.問題が解決しない場合は、SDカードのフォーマットを試してください。<br>3.フォーマットが効果がない場合は、SDカード交換のチュートリアルを参照してください。 |
| ERROR62 | Status_FsFailedOpenDir | 1.ディレクトリ名が正しくない。<br>2.ディレクトリ自体が破損している。 | 1.機器を再起動してもう一度試してください。<br>2.問題が解決しない場合は、SDカードのフォーマットを試してください。<br>3.フォーマットが効果がない場合は、SDカード交換のチュートリアルを参照してください。 |
| ERROR63 | Status_FSDirNotFound | 1.ディレクトリパスが正しくない。<br>2.ディレクトリが誤って削除された。 | 1.機器を再起動してもう一度試してください。<br>2.問題が解決しない場合は、SDカードのフォーマットを試してください。<br>3.フォーマットが効果がない場合は、SDカード交換のチュートリアルを参照してください。 |
| ERROR64 | Status_SDNotMounted | 1. SDカードが挿入されていない。<br>2.SDカードが挿入された後、マウントプロセスがトリガーされなかった。<br>3.以前のマウント試行が失敗した後、再マウントが実行されなかった。<br>4.この時点でSDカードに対する操作（ファイルの読み取り、ディレクトリの一覧表示など）を実行すると、このエラーがトリガーされます。 | 1.機器を再起動してもう一度試してください。<br>2.問題が解決しない場合は、SDカードのフォーマットを試してください。<br>3.フォーマットが効果がない場合は、SDカード交換のチュートリアルを参照してください。 |
| ERROR65 | Status_FsNotMounted | ファームウェアがアクセスする必要のあるファイルシステムが完全にマウントされていないため、ファイル/ディレクトリ操作を実行できない。 | 1.機器を再起動してもう一度試してください。<br>2.問題が解決しない場合は、SDカードのフォーマットを試してください。<br>3.フォーマットが効果がない場合は、SDカード交換のチュートリアルを参照してください。 |
| ERROR66 | Status_FsReadOnly | ファイルシステムが破損している。 | 1.機器を再起動してもう一度試してください。<br>2.問題が解決しない場合は、SDカードのフォーマットを試してください。<br>3.フォーマットが効果がない場合は、SDカード交換のチュートリアルを参照してください。 |

### 🔍 その他のシステムエラー（ERROR71-ERROR84, ERROR253）

| エラーコード | エラー名 | 故障原因 | 解決策 |
|------------|------------|-------------|----------|
| ERROR71 | Unknown operation found in expression. |  |  |
| ERROR72 | Divide by zero in expression attempted. |  |  |
| ERROR73 | Too large or too small argrument provided. |  |  |
| ERROR74 | Argument is not valid for the operation |  |  |
| ERROR75 | Expression is not valid. |  |  |
| ERROR76 | Either NAN (not a number) or infinity was returned from expression. |  |  |
| ERROR77 | Authentication required. |  |  |
| ERROR78 | Access denied. |  |  |
| ERROR79 | Not allowed while critical event is active. |  |  |
| ERROR80 | Flow statement only allowed in filesystem macro. |  |  |
| ERROR81 | Unknown flow statement. |  |  |
| ERROR82 | Stack overflow while executing flow statement. |  |  |
| ERROR83 | Out of memory while executing flow statement. |  |  |
| ERROR84 | Could not open file. |  |  |
| ERROR253 | User defined error occured. |  |  |

---

## 🛠️ トラブルシューティングガイド

### 🔴 優先順序
1. **ALARMエラー** - 優先的に処理、機器の安全な操作に影響
2. **ERROR40-ERROR58** - 機器関連エラー
3. **ERROR1-ERROR39** - Gコード関連エラー
4. **ERROR60-ERROR66** - SDカード関連エラー
5. **ERROR71-ERROR84, ERROR253** - その他のシステムエラー

### 💡 一般的な解決策
- 機器の状態と接続を確認する
- Gコード形式の正確性を確認する
- パラメータ設定範囲を確認する
- 機器を再起動または再初期化する
- ハードウェアセンサーの状態を確認する

---

*📝 このドキュメントは継続的に更新されています。ここに記載されていないエラーに遭遇した場合は、技術サポートにお問い合わせください。*