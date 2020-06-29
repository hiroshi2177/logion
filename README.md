# ログイン機能

==

##　概要
-会員でない方は新規登録し、データベースに保存する。
-会員登録がお済の場合、データベースに参照し一致するデータがあれば、ログイン画面からログインできる。

##概要詳細
-新規登録画面(名前、メールアドレス、パスワード、パスワード再確認)
-ログイン画面(メールアドレス、パスワード)
 --どの画面においても、ユーザーが理解しやすいようにミス表示される設定である。
 --(例：メールアドレスが入力されていません/パスワードと確認パスワードが一致しません。)


##動作環境
-Windows10 Pro
※上記内容で動作を確認しています。

##使い方
1.新規登録・ログインまでの流れ
-下記のリンクから会員登録(無料)します。
　--https://github.com/hiroshi2177/login/signup_form.php
-登録ができたら下記のリンクからログインします。
　--https://github.com/hiroshi2177/login/login_form.php


##データベース内容
 -テーブル名
 --[users]
 -カラム名/設定
 --[id]        INT　AI(自動的に番号振り分け)
 --[name]      VARCHARS　64字　
 --[email]     VARCHARS　191字　UNIQE(重複がないようにする)
 --[password]  VARCHARS　191字　
