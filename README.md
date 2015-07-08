#RailsTutorial演習用アプリ
[railstutorial.jp](http://railstutorial.jp)の「演習」をやっていくために作成したアプリケーションです。

##動作環境
- CentOS 7
- Ruby 2.2.2p95 (2015-04-13 revision 50295) [x86_64-linux]
- rvm 1.26.11 (master)
- rubygems 2.4.8
- Rails 4.2.3
- SQLite 3.7.17

##デプロイ方法
プロジェクトディレクトリ直下で以下のコマンドを入力することで、Rails自身が持つWebサーバWEBrickが起動し、[http://localhost:3000](http://localhost:3000) でアプリケーションにアクセスできます。
```
$ rails s -b 0.0.0.0
```
-bオプションがないと、起動端末のみからしかアクセスできない(フォワード等ができない)ので注意してください。
- フォワードする場合
 - ゲストOSの3000番へフォワードする設定を行う
 - ファイアウォールでゲストOSの3000番ポートの開放をしておく

