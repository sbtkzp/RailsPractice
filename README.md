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
以下のコマンドの入力で、Rails自身が持つWebサーバWEBrickが起動し、http://localhost:3000 でアプリケーションにアクセスできます。
```
$ rails s -b 0.0.0.0
```
-bオプションがないと、起動端末のみからしかアクセスできない(フォワード等ができない)ので注意してください。
- フォワードする場合
 - ゲストOSの3000番へフォワードする設定を行う
 - ファイアウォールでゲストOSの3000番ポートの開放をしておく

##ルーティング一覧
現時点でアクセスできるURIの一覧です。

|Prefix|Verb|URI Pattern|Controller#Action|
|-|:-:|-|:-:|
|static_pages_home| GET | /static_pages/home(.:format) |   static_pages#home|
|static_pages_help| GET | /static_pages/help(.:format)  |  static_pages#help|
|static_pages_about |GET | /static_pages/about(.:format)  | static_pages#about|
|static_pages_contact |GET | /static_pages/contact(.:format)| static_pages#contact|
