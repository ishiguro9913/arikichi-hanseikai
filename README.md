# 有吉反省会 on Web(仮)

## サービス概要
１人で抱えている反省をアウトプットして、前を向くことを助けるアプリ<br>
（某バラエティ番組の冒頭で、反省文を読み上げるコンセプトを参考にしています。）
## メインのターゲットユーザー
１人反省会を開いて悩みを抱えてしまう人
　
## ユーザーが抱える課題
・細かいことを気にしてしまい１人で反省を抱え続けてしまう<br>
・友達と会った帰りや飲み会の帰り道に、「何であんなこと言ってしまったんだろうか」「あの発言で実は嫌われていたりしないだろうか」と悩んでしまう<br>

## 解決方法
日々の反省していることへの<br>
１.反省文を作成して投稿<br>
２.投稿後にユーザー自身で反省文を読み上げる<br>
↓　そこから、<br>
・反省文が気持ちのこもっている文章になっているか<br>
・反省文をきちんと読み上げることが出来ているか<br>
上記の２要素で反省度合いを採点する。<br>
反省度が高ければ、反省を受け止めて激励のメッセージが表示される。<br>
反省度が低ければ、より反省していくよう叱責のメッセージが表示される。

## 実装予定の機能
・反省文を作成して投稿出来る機能<br>
・反省文を採点する機能<br>
 ※[Natural Language AI](https://cloud.google.com/natural-language?hl=ja) 等の文章解析APIを利用して、文章から感情を読み取れるか判定する。<br>
・反省文を読み上げた際の音声認識機能<br>
  ※[Web Audio API](https://developer.mozilla.org/ja/docs/Web/API/Web_Audio_API) 等の音声認識APIを利用する。<br>
・反省文の原文と、音声認識によるテキストがどのくらい一致しているか判定して採点<br>
・判定結果をTweetする機能<br>
## なぜこのサービスを作りたいのか
・自分自身が色々細かいことで、悩んで抱え続けてしまう性格<br>
・ひとりで悩んでも仕方ないので、反省の吐口があるといいと考えたため<br>
・「１人反省会」と検索したところ、6700万件ほどヒットする。このため、自分と似たようなことで悩んでしまう人は多いのではないかと考えている。
## スケジュール
README〜ER図作成：〜5/1<br>
機能実装：5/1-5/7<br>
MVPリリース：5/8<br>
本リリース：6/5