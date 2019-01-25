# Google Formマニュアル
---
### 概要
---
Google Formの作り方及び運用方法のマニュアル
これからアンケートなどを制作する上で必要になってくるであろう知識を記す


### Google Formとは
---
Google Drive上で動く、集計フォーム・お問い合わせフォームを制作・運用できるツール
デフォルトでスプレッドシートと連携出来る他、Google app script等を用いて色々なツールと連携することが出来る。


### 使用方法
---
今回は試しに作った
[澤さん目安箱 https://docs.google.com/forms/d/e/1FAIpQLSe1tjYjyz7RB3FCJkIZnS-RrV0HSw9fn7v4qo1BEZpu0TI9iA/viewform](https://docs.google.com/forms/d/e/1FAIpQLSe1tjYjyz7RB3FCJkIZnS-RrV0HSw9fn7v4qo1BEZpu0TI9iA/viewform)


[編集ページ https://docs.google.com/forms/d/1zMCUJmnTGIYg7kPaVkzYBEpC5KoHgcMg8nzFrX4ZsEU/edit?usp=sharing](https://docs.google.com/forms/d/1zMCUJmnTGIYg7kPaVkzYBEpC5KoHgcMg8nzFrX4ZsEU/edit?usp=sharing)
を例にとって解説していく。


#### 作成

[Google Form](https://www.google.com/intl/ja_jp/forms/about/)　https://www.google.com/intl/ja_jp/forms/about/

から画面中央部
[Google Formを使う]->新しいFormを作成よりその状況にあったテンプレートを選択(例では空白からスタート)

制作画面になるのでユーザ目線になりながら
- フォームタイトル
- 説明

を記入

フォーム右のメニュー(+)より質問項目を増やすことができる
※注意点としてどの質問を必須か否かをしっかり判断しないと欲しい情報が手に入らない
回答方法としては大まかに
- 記述式
- チェックボックス式
- プルダウン式
- ラジオボタン式

があり、状況によって使い分ける。

ざっくりと以上のことだけで運用することは可能である。

#### スプレッドシート

[回答]タブ右上の緑色のアイコンより集計先のスプレッドシートに飛ぶことができる

[澤さん目安箱のスプレッドシート](https://docs.google.com/spreadsheets/d/19o41TwlcJvRIOHHE7HfmzYraEhp1nIt1RJcRb4dy6IA/edit#gid=1967022244)

※注意点：新しく項目を間に差し込んでもスプレッドシートでは一番右の行に差し込まれる

- 実際に動かしてみる
澤さん目安箱に質問項目を一つ増やしてみる


#### 応用編
---
澤さん目安箱はChatworkと連携してある
[澤さん目安箱のスクリプトエディタ](https://script.google.com/a/neo-career.co.jp/macros/d/Mm36OmuhbWl6EdGK_76nfyMi9tyR_1_cq/edit?uiv=2&mid=ACjPJvElAJ-_v78hPRAGZuHJ4suMRclmYs-1VdRY0Gw8VCfQ8CIngiL2rmXa8RNPrWsenHQepW5z7818BMNaLRslBieZdhQXw8DXomxIxqk8PX7DwGz3kKwWgKWCMq6d1wEILNajGdafqkKd)
コードの詳細はスクリプトエディタの方に記載してある。

他のフォームのスプレッドシートで使う場合は
以上のコードを記載の上
メニューの時計マークより[＋トリガーの追加]
実行する関数を設定(サンプルではsendcw)　イベントの種類を[フォーム送信時]に設定
後は初期状態のままで問題なし



