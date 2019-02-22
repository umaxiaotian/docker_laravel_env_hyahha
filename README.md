# docker_laravel_env_hyahha
簡単に言うと、速攻でLaravelの環境が手に入ります。


## 説明
Windows10で構成しました、Laravelドッカー環境です。
内容物
nginx
php 
mysql

ポート　NGINX -> 80
	MYSQL -> 3306
※もしポートが他と競合してたらエラーになります。

◇トラブルシューティング
Laravel 5.4: Fatal error: Uncaught Error: Class 'Illuminate\Foundation\Application' のエラー
$ composer install
$ composer dump-autoload
で解決


500エラーが出る
envがないかも。。。
なければ.env.exampleをコピーして同じ位置に.envにリネームして貼り付け

RuntimeException がでる
key を生成する
php artisan key:generate


## 使い方
ファイル位置は、Laravelファイルをiotとしておいてください
laravel_project
├── iot (Laravelファイル)
├── docker-compose.yml
├── docker-nginx
│   ├── Dockerfile
│   └── default.conf
└── docker-php
    └── Dockerfile

### Install
```sh
git clone https://github.com/umaxiaotian/docker_laravel_env_hyahha.git
cd docker_laravel_env_hyahha
docker-compose build
docker-compose up -d

これで使えるはずです。