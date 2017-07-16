# 本アプリについて

本アプリは、次の教材を基に作られたサンプルアプリケーションです。
Twitterのようなつぶやきを投稿できるアプリケーションです。
[*Ruby on Rails チュートリアル: 実例を使って Rails を学ぼう*](http://railstutorial.jp/)
[Michael Hartl](http://www.michaelhartl.com/) 著


# モデルについて
本アプリでは三つのモデルがあります。

1. User
ユーザー情報を扱うモデルです。

2. Micropost
ユーザーが投稿するつぶやきを扱うモデルです。

3. Relationship
ユーザー間のフォロー情報を扱うモデルです。


# 使い方
このアプリケーションを動かす場合は、まずはリポジトリを手元にクローンしてください。
その後、次のコマンドで必要になる Ruby Gems をインストールします。

```
$ bundle install --without production
```

その後、データベースへのマイグレーションを実行します。

```
$ rails db:migrate
```

その後、サンプルデータを追加します。

```
be rake db:seed
```

Railsサーバーを立ち上げます。

```
$ rails server
```

