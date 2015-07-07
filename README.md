#RailsTutorial演習用アプリ
[railstutorial.jp](http://railstutorial.jp)の「演習」をやっていくために作成したアプリケーションです。

##動作環境
- Ruby 2.2.2p95 (2015-04-13 revision 50295) [x86_64-linux]
- rvm 1.26.11 (master)
- rubygems 2.4.8
- Rails 4.2.3
- SQLite 3.7.17

##デプロイ方法
このコマンドの入力で、
```
$ rails s -b 0.0.0.0
```
Rails自身が持つWebサーバWEBrickが起動し、アプリケーションにアクセスできます。-bオプションがないと、起動端末のみからしかアクセスできない(フォワード等ができない)ので注意してください。
