fizzbuzz (in C)
===============
Cで1〜100の範囲でFizzBuzz。手垢付きまくりの題材。
なのにどうして2時間もかかっちゃたんだろーなー。
どうして150行超えちゃってるんだろーなー (棒

999までの出力に対応できる構造なので、プリプロセッサの#includeネスト数
限界にさえ引っ掛からなければソース行数よりも長い出力も得られるはず。

dec-basedブランチ、masterブランチは、プリプロセス後の出力が綺麗なコードに
なるようにしているが、mastre-shorterブランチはプリプロセス後の出力の
可読性を二の次として短いコードを書くようにしている。

ただし、本気で短いコードを書こうとすると真っ当にプログラミングした方が
有利なので、以下の縛りを付けた。

* ループ構造は用いない。
* ループ以外の制御文は使ってもよい。ただし使わずに済むならばできるだけ
  使わない。
* 文字列出力部はプログラム中一箇所のみ。
* 1行には高々1文のみ。ただし制御文 + 1文 (非ブロック) を一行に書くのはOK。
* 中括弧 {} は、開き、閉じ共に独立した行に書く。
* gcc -Wallで警告が出力されないこと。(現在のgccバージョン: 4.7.2)
