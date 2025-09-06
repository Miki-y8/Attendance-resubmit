# Attendance-resubmit
## Dockerビルド

1.git clone

git@github.com:Miki-y8/Attendance-resubmit.git

2.DockerDesktopアプリを立ち上げる

3.docker-compose up -d --build

MacのM1・M2チップのPCでエラーが出る場合、docker-compose.ymlファイルのmysqlに

platform: linux/x86_64

を追加する



## Laravel環境構築

1.docker-compose exec php bash

2.composer install

3.「.env」ファイルを作成

### .envに以下の環境変数を追加

DB_CONNECTION=mysql

DB_HOST=mysql

DB_PORT=3306

DB_DATABASE=laravel_db

DB_USERNAME=laravel_user

DB_PASSWORD=laravel_pass

## アプリケーションキーの作成

php artisan key:generate

## マイグレーションの実行

php artisan migrate

## シーディングの実行

php artisan db:seed

## 使用技術(実行環境)

PHP8.3.0

Laravel8.83.27

MySQL8.0.26

## ER図
<img width="929" height="579" alt="スクリーンショット 2025-09-06 21 31 17" src="https://github.com/user-attachments/assets/fddab223-167a-450f-92f1-4c3896e8d937" />


## URL
開発環境：http://localhost/
phpMyAdmin:：http://localhost:8080/

