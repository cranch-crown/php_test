# Docker PHP-nginx-MariaDB

## 概要
PHP-FPM, nginx, MariaDBのPHP用開発環境です。

## 前提
* Docker
* Docker Compose

## 使い方
まず `.env`ファイル内の下記変数を設定してください
* DB_NAME: Database名。立ち上げる時に、MariaDB内にこの名前のデータベースを作成します。
* DB_USER: MariaDBに作成するユーザー名です。 
* DB_PASS: rootユーザーと、上記のユーザーにこの値のパスワードを設定します。
* TZ: MariaDBとPHPに設定するタイムゾーンです。

設定し終わったら`docker-compose up`で立ち上げます。`app`ディレクトがnginxのドキュメントルートになっています。