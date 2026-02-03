project pageを作成したい
タイトルは
ELSA: Acoustic Event-Level Semantic Alignment for Fine-Grained Reference-Free Text-to-Audio Evaluation
論文の内容は
ELSA__Acoustic_Event_Wise_Semantic_Alignment_forFine_Grained_Reference_Free_Text_to_Audio_Evaluation.pdf

動画や音声，スコア数値のテンプレートは用意可能
モデル図や表はstatics/imagesにある
github pagesで公開したい

- タイトルのフォントサイズを統一する
- デモはパイプラインがわかるようにする
- 画像をクリックしたら拡大表示（ライトボックス）できるようにする
- 実験結果はカルーセルで表示する
- [Done] 背景に雪のエフェクトを追加する（コンテンツの背面に配置）
- [Done] 「Samples」という表記を「Demo」に変更する
- [Done] ディズニーの「エルサ」を彷彿とさせるデザインテーマ（色使い、雰囲気）にする
- [Done] 降った雪がページ下部に積もるようにする
- [Done] タイトルの先頭に雪だるまのアイコンを追加する
- Methodセクションは `model.png` を使用して説明する（アイコンパイプラインはDemoで使用する）
- DemoセクションをJSON駆動のインタラクティブな形式にする
  - ユーザーがサンプルを選択できる
  - 選択されたサンプルに基づいて、パイプライン（Text -> LLM -> Parsed / Audio -> LASS -> Separated -> Score）の内容が動的に変化する
  - データは `demo.json` で管理する
- Analysisセクションもカルーセルにする
- カルーセルは7秒ごとに自動で切り替わるようにする
- [Done] JSの最適化（雪のアニメーションの軽量化）
- [Done] 画像の< >（カルーセルボタン）の曲率を修正
- [Done] 画像の説明（表のタイトル）の重複を削除
- [Done] CitationをInterspeech 2026形式（Proc. Interspeech 2026）に修正
- [Done] Copyrightsの削除
