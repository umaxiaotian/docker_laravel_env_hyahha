# docker_laravel_env_hyahha
簡単に言うと、速攻でLaravelの環境が手に入ります。</br>

</br>


## 説明
Windows10で構成しました、Laravelドッカー環境です。</br>
内容物
nginx</br>
php </br>
mysql</br>
</br>
ポート　NGINX -> 80</br>
	MYSQL -> 3306</br>
※もしポートが他と競合してたらエラーになります。</br>
</br>
◇トラブルシューティング</br>
Laravel 5.4: Fatal error: Uncaught Error: Class 'Illuminate\Foundation\Application' のエラー</br>
http://kz-engineer-scrap.hatenablog.com/entry/2017/03/14/000158
</br>
$ composer install</br>
$ composer dump-autoload</br>
で解決
</br>
</br>
500エラーが出る</br>
envがないかも。。。</br>
なければ.env.exampleをコピーして同じ位置に.envにリネームして貼り付け</br>
https://www.kabanoki.net/2524#env
</br>
RuntimeException がでる</br>
key を生成する</br>
php artisan key:generate</br>

</br>


## 使い方


</br>
ファイル位置は、Laravelファイルをiotとしておいてください</br>
</br>
laravel_project</br>
├── iot (Laravelファイル)</br>
├── docker-compose.yml</br>
├── docker-nginx</br>
│   ├── Dockerfile</br>
│   └── default.conf</br>
└── docker-php</br>
    └── Dockerfile</br>
</br>


### Install
```sh
git clone https://github.com/umaxiaotian/docker_laravel_env_hyahha.git
cd docker_laravel_env_hyahha
docker-compose build
docker-compose up -d

これで使えるはずです。
